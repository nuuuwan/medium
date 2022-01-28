#### Article 325 · May 23, 2021

# Plotting Maps of Sri Lanka with GeoPandas and MatPlotLib

### A Simple Tutorial

Disclaimer: This article describes a work-in-progress. Please comment on how we might improve the underlying libraries, especially what additional features you would like.

## Geo-Spatial Data

The only real barrier to plotting maps of Sri Lanka with Python libraries GeoPandas and MatPlotLib is the difficulty of accessing geographical data for Sri Lanka. I've attempted to solve this problem by scraping geographical data from various sources, sharing it on GitHub, and providing a simple python library geo-nuuuwan for conveniently accessing this data.

Begin by installing geo-nuuuwan

```
pip install geo-nuuuwan
```

## Example 1: Basic Maps

Module geodata in geo (geo-nuuuwan) implements method get_region_geodata, which returns geographical data (as a GeoPandas.GeoDataFrame) for some region of Sri Lanka, split by some region.

For example, the following snippet returns geographical data for Sri Lanka split by province.

```
from geo import geodatagpd_df = geodata.get_region_geodata('LK', 'province')
```

The GeoPandas.GeoDataFrame can be plotted using MatPlotLib as follows:

```
import matplotlib.pyplot as pltfrom geo import geodata
```

```
gpd_df = geodata.get_region_geodata('LK', 'province')gpd_df.plot()
```

```
plt.show()
```

The result is:

![Image](https://cdn-images-1.medium.com/max/800/1*_-I6L4h0_f7L-b4e9-JKLQ.png)

## Example 1a

Similarly, we can plot Colombo District ("LK-11") by DSDs (Divisional Secretariat Divisions) with:

```
gpd_df = geodata.get_region_geodata('LK-11', 'dsd')
```

![Image](https://cdn-images-1.medium.com/max/800/1*4YMw52TMcWfn0tJO06wZYA.png)

## Example 2: Plotting some useful data

In addition to geographical coordinates, the GeoPandas.GeoDataFrame includes some additional basic data like parent regions, population and area data.

This additional data can be inspected as follows:

```
import matplotlib.pyplot as pltfrom geo import geodata
```

```
gpd_df = geodata.get_region_geodata('LK', 'district')print(gpd_df)
```

Output:

![Image](https://cdn-images-1.medium.com/max/800/1*l6oEkw1ZCM5av6yL9qrVpw.png)

Using the population and area data, we can color the map by each region's (say district's) population density as follows:

```
gpd_df = geodata.get_region_geodata('LK', 'district')
```

```
gpd_df['density'] = gpd_df['population'] / gpd_df['area']gpd_df.plot(column='density', legend=True, cmap='OrRd')
```

```
plt.show()
```

![Image](https://cdn-images-1.medium.com/max/800/1*c6DALweaAY3zkdzSUS7JRw.png)

## Example 2a

Similarly, population density of Sri Lanka's DSD.

```
gpd_df = geodata.get_region_geodata('LK', 'dsd')
```

```
gpd_df['density'] = gpd_df['population'] / gpd_df['area']gpd_df.plot(column='density', legend=True, cmap='OrRd')
```

```
plt.show()
```

![Image](https://cdn-images-1.medium.com/max/800/1*ZIMDazKI7P7E1KRxSPnHOg.png)

## Example 2b: Prettifying the Plot

We can add a title, legend, better color scheme to our plot, and resize it as follows:

```
gpd_df = geodata.get_region_geodata('LK', 'dsd')
```

```
gpd_df['density'] = gpd_df['population'] / gpd_df['area']
```

```
gpd_df.plot(    column='density',
```

```
scheme='UserDefined',    classification_kwds={        'bins': [100, 200, 400, 800],    },    legend=True,    legend_kwds={        'labels': [            '< 100',            '100 - 200',            '200 - 400',            '400 - 800',            '800 <',        ],    },    cmap='OrRd',    figsize=(7, 9),)plt.title('Population Density of Sri Lanka by DSD')
```

```
plt.show()
```

[Note, these are all GeoPandas and MatPlotLib features. Not features from geo-nuuuwan.]

![Image](https://cdn-images-1.medium.com/max/800/1*sU8pcimzbq6PDqTdQb3aIA.png)

## Example 2c

Similarly, "Population Density of Sri Lanka by GND":

```
gpd_df = geodata.get_region_geodata('LK', 'gnd')...plt.title('Population Density of Sri Lanka by GND')
```

![Image](https://cdn-images-1.medium.com/max/800/1*coK7FOTZwS_f6XEwUzHVzg.png)

## Example 2d

And "Population Density of the Central Province by DSD":

```
gpd_df = geodata.get_region_geodata('LK-2', 'dsd')...plt.title('Population Density of the Central Province by DSD')
```

![Image](https://cdn-images-1.medium.com/max/800/1*L6_JvyGAXtJI2q2eAOEfVg.png)

## Coming Soon

The goal of this article was to introduce geo-nuuuwan, and plotting basic maps of Sri Lanka and its regions. In future articles, we'll look at:

* Plotting more elaborate data (e.g. census, election)

* Plotting different types of maps and cartograms

* Anything else? Please comment with your wishlist.