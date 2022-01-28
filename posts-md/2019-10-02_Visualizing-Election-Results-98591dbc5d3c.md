#### Article 124 · October 2, 2019

# Visualizing Election Results

### Different ways to draw maps

Leading up to the 2019 Presidential Election in Sri Lanka, I wanted to learn more about the previous presidential elections. I found this map displaying the results of the 2015 Presidential Election.

![Image](https://cdn-images-1.medium.com/max/800/1*lROd_feXFgSV1MS--KTxsQ.png)

For each of Sri Lanka's 160 polling divisions, the colour indicates who won. Pink for President Sirisena. Blue for President Rajapaksa.

As we know, Sirisena won with 51.28%, to Rajapaksa's 47.58%. Seventeen minor candidates shared the remaining 1.14%.

But if you looked at you'd think Rajapaksa won. A larger proportion of the map is blue. Unsurprising, since Rajapaksa won sparsely populated rural polling divisions, and Sirisena won denser urban areas like Colombo.

And this was no exception.

In the 2008 US Presidential Election, President Obama, like Sirisena, he won more urban counties. His opponent, the late Senator McCain, won more rural areas. While Barack Obama won 52.9% of the vote, to McCain's 45.7%, looking at the map of county results, you'd think McCain won. And easily.

![Image](https://cdn-images-1.medium.com/max/800/1*k7eJ8SHpjihZXEy7XxefGA.png)

The problem with these maps is that it quantifies geographical space. On the other hand, for an election, quantifying population, or more specifically, the voting population is more important.

Hence, is there a better way of representing election results?

## Solution 1: Continuous Cartograms

>>> "A cartogram is a map in which some thematic mapping variable — such as travel time, population, or GNP — is substituted for land area or distance" (Wikipedia).

In the case of elections, we can substitute area for voter population. For example, this is a cartogram of the 2008 US Presidential Election.

![Image](https://cdn-images-1.medium.com/max/800/1*sfOkIdtMVvEjyUZ1XPgHWw.png)

These cartograms distort space by population. Densely populated areas push out their boundaries stronger than sparsely populated ones. The end effect is for the former to expand and the latter to shrink.

One problem with this technique is that it distorts and uglifies the map. Here is a population cartogram of Sri Lanka, which has the same uglification problem.

![Image](https://cdn-images-1.medium.com/max/800/1*EA3ckneAo1PVYZbV1C49_A.png)

## Solution 2: Non-Continuous Cartograms

An alternative is to resize the areas while preserving shape. For example, the 2008 US Presidential election results alternatively look like this:

![Image](https://cdn-images-1.medium.com/max/800/1*UHcy3ZMl2oBN9FCfYfPYLg.gif)

And Sri Lanka, by population, would look like this in a Non-Continuous Cartogram:

![Image](https://cdn-images-1.medium.com/max/800/1*d49MKWNKDGZGxtrdC6YULg.png)

Re-proportioning solves the distortion problem. However, it has a deeper problem. When we look at election results, do we care about the shape of Colombo district or the state of Florida? We probably just want to know the outcome. Who won.

## Solution 3: Abstract Cartograms

A more abstract abstraction is to replace area with boxes or other geometric shapes, which are proportional to population.

![Image](https://cdn-images-1.medium.com/max/800/1*sMA-rG2QJq4eZvNEV1s7lA.jpeg)

We can also use other shapes. For example, here is a hexagon view of the 2015 and 2017 UK Parliamentary Election results.

![Image](https://cdn-images-1.medium.com/max/800/1*azF-dWuMhFxCizYUwpTgEA.png)

In the next diagram, we go one step further with one box for each of Sri Lanka's 160 polling divisions. The 2015 Presidential Election result looks like this.

![Image](https://cdn-images-1.medium.com/max/800/1*WiQRbRXJOLjYx7cdvujFOQ.png)

This view is very specific and focussed. It also connects different districts with similar voting patterns. For example, the east of the Colombo District (Co), unlike the west, tends to vote more like the Kegalle District (Ke).

Note, Presidential Elections in Sri Lanka are won by total votes, but by first-past-the-post, or an electoral college system (as in the US). Hence, specifics of number of votes is also important. If we would factor this, our map would look like:

![Image](https://cdn-images-1.medium.com/max/800/1*FWD6K9O4NSMt3fz3tfyyXw.png)

## So what's the result?

And since we are talking about elections, let's put all this to a poll:

>>> What is your favourite election results map?

Please comment!