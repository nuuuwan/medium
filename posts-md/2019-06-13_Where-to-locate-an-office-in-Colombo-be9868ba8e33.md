#### Article 36 · June 13, 2019

# Where to locate an office in Colombo

### A very rough analysis

A friend and I were debating on the pros and cons of various locations around Colombo for locating offices. Traffic was an important determining factor, and the optimal location was that which as many employees could travel to and from with least difficulty.

To quantitatively augment our mostly qualitative discussion, I did a Google Maps API search, for a selection of office locations, on how long it takes to travel to that location from various parts of Greater Colombo, during the morning rush hour around 8am.

The selected "office locations" were:

* World Trade Center, Colombo 1

* Thummulla, Colombo 7

* Narahenpita Junction, Colombo 5

* Dehiwala Junction, Dehiwala

* The Parliament, Sri Jayawardena Pura Kotte

* Malabe Town, Malabe

This is what I got.

![Image](https://cdn-images-1.medium.com/max/800/1*qsvZ-vUiLOQ76baLETgNjg.png)

The colour legend is:

* Blue < 15min

* Green 15–30min

* Yellow 30–45min

* Orange 45–60min

* Red 60–90min

* Dark Red 90–120min

* Black >120min

![Image](https://cdn-images-1.medium.com/max/800/1*56GP73FHtoZOGanCfsIjdA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*o-0UktsPm3T3uqlhyTfhpw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*N86QQMumpsiekWDwYIZTZQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*fFiQrraIS0hvvxy4CJxVkw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*16mlSjepxYfqLF4EsjyGdA.png)

## Caveats

* "The optimal location was that which as many people could travel to and from with least difficulty" — this visualization only factors travel time. It does not factor the density of population, and hence travel volume of various locations. One location could have a large "quick to travel" zone (Blue/Green), which is sparsely populated, while another location could have a small "quick to travel" zone which is densly populated, and hence with more travel volume.

* The data does not factor in non-traffic features, like proximity to amenties, proximity to customers, "nice neighbouhood", etc.

* Travel time only factors one direction of travel (to work around 8am), and does not factor in travel to and from customer/client offices during the day, and the return commute at the end of the day. Also, many people increasingly travel at unorthodox hours to beat the traffic (probably any time from 4am to 12noon).