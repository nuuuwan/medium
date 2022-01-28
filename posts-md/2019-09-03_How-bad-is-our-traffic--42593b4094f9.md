#### Article 77 · September 3, 2019

# How bad is our traffic?

### The Colombo Traffic Index

## TomTom Traffic Index (TTTI)

The Dutch navigation technology company TomTom recently published its Traffic Index, a measurement of congestion levels in 403 cities across 56 countries. TomTom describes its methodology as follows:

>>> The congestion level percentages represent the measured amount of extra travel time experienced by drivers across the entire year. We start by establishing a baseline of travel times during uncongested, free flow conditions across each road segment in each city. We then analyze travel times across the entire year (24/7) for each city — and compare this information against free flow periods to derive extra travel time.

>>> An overall congestion level of 36% means that the extra travel time is 36% more than an average trip would take during uncongested conditions. Average times are of actual taken trips, across every vehicle in the entire network, 24/7. Travel times in free-flow (uncongested) conditions are not based on speed limits but on actual trips made.

While the index included several South Asian cities, neither Colombo nor any other Sri Lankan city was on the list.

![Image](https://cdn-images-1.medium.com/max/800/1*Qr3xhCYd5SCZYNobeB6PTA.png)

So I decided to do my own version of the "Traffic Index" for Colombo.

## Colombo Traffic Index (CTI) Methodology

TomTom owns a vast amount of traffic data, which I don't have access to. Hence, rather than try and mimic the TTTI exactly, I used a simpler methodology, which makes computation simpler, but still preserves the spirit of the TTTI.

The spirit of TTTI is (for me) the definition of the index, which, in principle is the ratio of Actual Travel Time / Zero Congestion Travel Time. While preserving this definition, I made the following simplifications:

* I used Best Case Travel Time (i.e. travel time at the time of the day when travel time is least) as an approximation for Zero Congestion Travel Time

* Rather than looking at all the roads in the city, I looked at travel between a set of "important locations" on the periphery of the city to the City Centre (which I assumed to be the World Trade Center, Colombo 1). The "important locations" were Wattala, Kelaniya, Battaramulla, Nugegoda and Dehiwala, all about 30 to 60min of travel from the City Centre on average.

* Rather than looking at a whole year's worth of data, I looked at one day: An ordinary working week-day, when schools were open.

My data source was the Google Maps API. Estimates were for "driving" (not public transit or walking) and used "pessimistic" estimates.

## Case Study: Travelling from Dehiwala

For each of the important locations, I looked at travel time to and from the city centre. For example, travel time to and from Dehiwala was

![Image](https://cdn-images-1.medium.com/max/800/1*ku_hedTPqGclGkvb0fA6Zw.png)

The blue line represents travel time from Dehiwala to the City Centre, while the orange line is vice-versa. As expected, both lines have peaks 1) during the morning office rush hour, 2) when schools close in the afternoon, and 3) during the evening office rush hour.

Note: I didn't look into why the travel out of the city takes longer than travel into the city — it might be due to the assymetries in Galle Road, Duplication Road, and Marine Drive.

The Best Case Travel Time in both directions is early in the morning (~4am), and we can use this to compute the Actual Travel Time /Base Case Travel Time ratio (i.e. my Traffic Index) at various times of the day:

![Image](https://cdn-images-1.medium.com/max/800/1*WtrGHV7aH8ez5gCYGArcfw.png)

At the best case travel time (~4am) the index is zero (by definition), and is low until around 6am. By the 8am morning office traffic peak, the Traffic Index into Colombo is 153%. This means that travel time is 153% or 2.53x times more at this time. At 4am you should be able to travel from Dehiwala to Colombo Centre in about 18min. By 8am, the estimate is 44min (or 18min + 153%).

At the close of schools, and the evening office rush hour, travel out of Colombo becomes (comparatively) more congested, with the Traffic Index at 1pm 182% and 5.30pm 221%. At 4am you should be able to travel from Colombo Centre to Dehiwala in about 23min. At 1pm it would take an estimated 64min (23min + 182%); at 5.30pm an estimated 74min (23min + 221%, or 3.21x more time).

## Computing the CTI

We can aggregate the Traffic Index across the day into a single overall Traffic Index. The average travel time from and to Dehiwala were 31min and 43min respectively. The best case travel time from and to were 18min and 23 min. Hence, the average Traffic Indices are 75% and 87% respectively. We can average these two to give 81%.

We can extend this to all the "important locations", and average the TIs to give our final aggregated, global average Traffic Index, or our Colombo Traffic Index (CTI): 80%.

![Image](https://cdn-images-1.medium.com/max/800/1*XpkmYJ-7neQLM_ZAfanGug.png)

## What the CTI tells us

Important Disclaimer: Before comparing the CTI to the TTTI for other cities, note that my methodology is different, simpler, and less accurate. Hence, absolute interpretations and direct comparisons are not recommended.

On the other hand, the CTI does tells us a few things:

* The bad news: Colombo Traffic is pretty bad (though, you don't need an index to know that). In numerical terms, traffic is 80% or 1.8x slower than what it can be, on average. The worse cases are much worse.

* The good news: The "other side of the coin" of a bad traffic index is that there is huge opportunity for improvement. More road capacity (particularly at bottlenecks), and more mass transport (buses, trains, metro) can improve speed up traffic times by nearly double on average, and much more during rush hour.

* The meh news: In the meantime, the information behind the CTI can be useful for planning your travel. For example, optimizing your travel by even a few minutes can result in significant time savings.

## Appendix: Travel times from Important Locations

![Image](https://cdn-images-1.medium.com/max/800/1*dgrWaMGDRs0OC7WgsC09eg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*kQetBBIr3bNs_4xyXC1ALQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*yrOHTnEogDtAoubPK_gbDg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*mYvMx9RSyU9ck5bOvbYHRQ.png)

## Bonus Appendix: Travel time data between Colombo and other cities

Most important takeaway: While travel from Colombo to other cities is comparatively efficient, traffic on some routes (e.g. Colombo to Kandy) is almost as bad as city traffic. Just as we need improved intra-city transport, we also need improved inter-city transport.

![Image](https://cdn-images-1.medium.com/max/800/1*8Nd7BAf7eseuIve1mEikeQ.png)