#### Article 118 · September 27, 2019

# The Center of Sri Lanka

### And different ways of defining it

## Centre of Bounding Box

Question: What is so special about this point on Kandalama Lake?

![Image](https://cdn-images-1.medium.com/max/800/1*eOdbFt9qn0mynk-ddhIV7A.png)

Here's a clue: It's latitude and longitude are 7.877083N, 80.697917E.

Answer: If you draw a bounding box using Sri Lanka's extreme points (Point Pedro to the orth, Dondra Head to the south, Sangaman Kanda Point to the east, and Kachchatheevu Island to the west), this point would be dead center.

![Image](https://cdn-images-1.medium.com/max/800/1*3-zl5WOem4ZKtRIlWiq0Wg.png)

Note, this is different from the Centre of Geography, which involves some more complex calculations.

## Center of Population

Sri Lanka's population is skewed towards the south west of the Island. If you factor this in, and compute the Centre of Population, it would be 7.211559N, 80.427956E, or somewhere near Aranayaka in the Kegalle District.

![Image](https://cdn-images-1.medium.com/max/800/1*iiY3-Pex5YTOZdXclObFKQ.png)

Note, that, obviously, this is to the south and west of Kandalama.

## Where to locate an office in Colombo (Revisited)

In Where to locate an office in Colombo, I looked at travel time to six potential "office locations" in Greater Colombo, from various other parts of Greater Colombo.

![Image](https://cdn-images-1.medium.com/max/800/1*f739S7l5Kvs1_oYeTB35-Q.png)

One problem with my analysis was that it didn't factor in population density, and travel volume:

>>> "The optimal location was that which as many people could travel to and from with least difficulty" — this visualization only factors travel time. It does not factor the density of population, and hence travel volume of various locations. One location could have a large "quick to travel" zone (Blue/Green), which is sparsely populated, while another location could have a small "quick to travel" zone which is densly populated, and hence with more travel volume.

To better answer this question (but still not perfectly), I extended the "centre of population" idea to look at the population distributions around the six "office locations".

![Image](https://cdn-images-1.medium.com/max/800/1*u255uL7yDIt4lysWH05hNw.png)

If one were to target a 1km travel radius, then Thunmulla and Narahenpita Junction, would be the best option, because about over 100,000 people lived within a 1km radius of these "office locations".

Thunmulla would be the best location until around 6km, when The Parliment, with a cumulative population of around 1M people, would be the best location.

After 12km, Malabe Town, with a comulative population of around 2.3M people, would be the best location.

## Center of Travel Time

Obviously, what we really want is a "Center of Travel Time". Traveling 6km to one place, might take longer than travelling 12km to another. But that involves some pulling a lot of data from the Google Maps API, which I will leave for later.