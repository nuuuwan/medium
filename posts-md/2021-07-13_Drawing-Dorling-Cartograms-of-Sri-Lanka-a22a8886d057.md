#### Article 330 · July 13, 2021

# Drawing Dorling Cartograms of Sri Lanka

### A Tutorial with Python, MatPlotLib and GeoPandas

Consider the following map of Sri Lanka, presenting the results of the 2019 Sri Lankan Presidential Election.

![Image](https://cdn-images-1.medium.com/max/800/1*LEYyVKBHh0VWwP965mZZ0A.png)

In my previous article, The "Map", I wrote about two problems with this representation.

* It assumes everyone in a polling division voted for one party. For example, 42.45% of valid votes in the Ratmalana Polling Division were for the NDF. However, on the map it is colored maroon.

* It gives more sparsely populated polling divisions disproportionately more visual space. For example, some of the most densely populated polling divisions in the Colombo District are barely visible.

I described "progressive coloring" as a solution to the first problem, where we color polling divisions where the winning party got a larger proportion of the votes in a stronger color. I proposed Dorling Cartograms as a solution to the second problem.

This article is a tutorial, where will will discuss how we can draw Dorling Cartograms for Sri Lankan Election Results. You can easily extend the ideas to other data.

[You can find the complete source code for this tutorial, including examples at github.com/nuuuwan/infographics.]

## What is a Dorling Cartogram?

A "Cartogram" is a special type of diagram, that modifies a geographical map to better represent statistical informaiton (like the distribution of populations of the results of elections).

A "Dorling Cartogram" represents each area with a geometric shape (e.g. a Circle, a Rectangle or a Hexagon), and the area of the shape is proportional to the statistical data we want to represent (e.g. Population or Valid Votes).

## (Before we begin)

This tutorial assumes you have python 3.7 installed. You also need MatPlotLib and GeoPandas.

```
pip install matplotlibpip install geopandas
```

I've implemented Dorling Cartograms, and a few other convinience functions in PyPI Package infographics-nuuuwan.

```
pip install infographics-nuuuwan
```

Also, you can access data about Sri Lankan elections from PyPI Package elections_lk-nuuuwan.

```
pip install elections_lk-nuuuwan
```

## Example 1: True-Area Map

In all our examples, we will be drawing maps for the 2019 election, and drawing these maps for the entire country.

```
year = 2019region_id = 'LK'
```

Let's first draw a true-area map of Sri Lanka with LKMap, and color each polling division by the winning party.

```
true_map = LKMap(   region_id=region_id,   sub_region_type='pd',   figure_text='a) True-Area Map',​   func_get_color_value=_func_get_color_value,   func_value_to_color=_func_value_to_color,   func_format_color_value=_func_format_color_value,   func_render_label=_func_render_label,​   left_bottom=(0.1, 0.1),   width_height=(0.8, 0.8),)
```

Each of the "func" parameters, pass functions that determine how the map should be colored, and how labels should be rendered.

```
def _func_get_color_value(row):   result = pd_to_result[row.id]   return presidential.get_winning_party_info(result)['party_id']​​def _func_value_to_color(party_id):   return party_color.get_rgb_color(party_id)​​def _func_format_color_value(party_id):   return party_id​​def _func_render_label(row, x, y, spany):   pass
```

We embed the map inside an infographic with Infographic as follows:

```
Infographic(   title='%d Sri Lankan Presidential Election' % year,   subtitle='By Winning Party',   footer_text='\n'.join(      [           'data from https://elections.gov.lk',           'visualization by @nuuuwan',      ]  ),   children=[       true_map,  ],).save('/tmp/infographics.%d.png' % year)
```

The saved image looks like this:

![Image](https://cdn-images-1.medium.com/max/800/1*LEYyVKBHh0VWwP965mZZ0A.png)

## Example 2: Dorling Cartogram

We can represent the election results on a Dorling Cartogram with LKDorlingCartogram, as follows.

```
dorling = LKDorlingCartogram(   region_id=example3.region_id,   sub_region_type='pd',   figure_text='b) Dorling Cartogram',​   func_get_color_value=_func_get_color_value,   func_value_to_color=_func_value_to_color,   func_format_color_value=_func_format_color_value,   func_render_label=_func_render_label,   func_get_area_value=_func_get_area_value,   func_format_area_value=_func_format_area_value,​   left_bottom=(0.55, 0.1),   width_height=(0.4, 0.8),)
```

LKDorlingCartogram is very similar to LKMap, with the exception of the two functions that define the area of the Dorling Cartogram Circles; note, we want to make the area of the circle proportional to the number of valid votes in the polling division.

```
def _func_get_area_value(row):    result = pd_to_result[row.id]    return result['summary']['valid']
```

```
def _func_format_area_value(area_value):    return '{:,.0f}\nvalid votes'.format(area_value)
```

We can display the previous True-Area Map, and the Dorling Cartogram, side-by-side, as follows:

```
true_map.set_position(    left_bottom=(0.05, 0.1),    width_height=(0.4, 0.8),)
```

```
Infographic(    title='%d Sri Lankan Presidential Election' % year,    subtitle='By Winning Party',    footer_text='\n'.join(        [            'data from https://elections.gov.lk',            'visualizaiton by @nuuuwan',        ]    ),    children=[true_map, dorling],).save('/tmp/infographics.example4.%d.png' % year)
```

[Note, we change the size and position of the True-Map]

We get,

![Image](https://cdn-images-1.medium.com/max/800/1*YH9z7V-X9iR_tyVvFY_e_Q.png)

## Example 3: Dorling Cartogram with Progressive Coloring

For completeness, let's also draw the True-Area Map and the Dorling Cartogram with progressive coloring. To implement progressive coloring, we tweak the color functions (_func_get_color_value etc) to consider the proportion of votes the winning party got.

```
def _func_get_color_value(row):    result = pd_to_result[row.id]    party_info = presidential.get_winning_party_info(result)    party_info['p_votes'] = party_info['votes'] / result['summary']['valid']    return party_info
```

```
def _func_value_to_color(party_info):    return party_color.get_rgba_color(        party_info['party_id'],        party_info['p_votes'],        p_to_a=lambda p: max(p - 0.3, 0) / 0.7,    )
```

```
def _func_format_color_value(party_info):    return '{party_id} {p_votes:.0%}'.format(        party_id=party_info['party_id'],        p_votes=party_info['p_votes'],    )
```

We can plot all four permutations (True-Area + Dorling Cartogram x Not-Progressive Coloring + Progressive Coloring) on a single Infographic as follows:

```
Infographic(    title='%d Sri Lankan Presidential Election' % year,    subtitle='By Winning Party',    footer_text='\n'.join(        [            'data from https://elections.gov.lk',            'visualizaiton by @nuuuwan',        ]    ),    children=[        true_map,        dorling,        true_map_prog,        dorling_prog,    ],).save('/tmp/infographics.example6.%d.png' % year)
```

This gives,

![Image](https://cdn-images-1.medium.com/max/800/1*zQAqQpsCTtpKO4zkzMQfSw.png)

## How are Dorling Cartograms Rendered?

The rendering process begins with drawing the circles in their geoprphically correct locations, like this:

![Image](https://cdn-images-1.medium.com/max/800/1*4GJ8VAGUYcLTr4gYIg6goQ.png)

As you can see, circles in densely population areas (like Colombo) overlap. In the next step, we move the overlapping circles away from each other, by making them repel each other.

![Image](https://cdn-images-1.medium.com/max/800/1*YH9z7V-X9iR_tyVvFY_e_Q.png)

## Variations: Bigger and Smaller Circles

LKDorlingCartogram has a parameter "compactness", which defines have much space the circles take. A "compactness" of 100% will be the largest possible extent possible, where the circles will spread across the entire bounding box of the map.

In practice, about 30% is a good compactness.

![Image](https://cdn-images-1.medium.com/max/800/1*SW7U4jGKn5WifLBL4QdsRQ.png)

## Variations: Other Regions and Years

You can draw the same graphs for sub-regions of Sri Lanka by updating the region_id parameter.

```
region_id = 'EC-04'  # Kandy Electoral District
```

![Image](https://cdn-images-1.medium.com/max/800/1*GNmeSdKV6Tww5CY9DdXCaQ.png)

Similarly, you can update year to build results for other years.

```
year = 2015
```

![Image](https://cdn-images-1.medium.com/max/800/1*y04vDQnVMw-DWzv2A0Odvg.png)

## Variations: Other Shapes

You can tweak LKDorlingCartogram to replace circles with other shapes.

```
plotx.draw_circle((x, y), r, fill=color)
```

## Concluding Requests

Please share your thoughts on how these visualizations and the underlying libraries can be improved. Also, feel free to fork or update the code as you feel fit.