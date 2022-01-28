#### Article 273 · October 8, 2020

### Transport

# Road Metrics

### From Latency to Bandwith

## Simple Road Segments

Consider a hypothetical segment of road. Suppose this segment is short enough that all the vehicles on it move at the same speed.

Suppose we wanted to "measure" the "state" of this road, using various metrics. What metrics might we care about?

### Distance and Speed

The most "well-known" metric about roads is probably distance. Or the length of the road segment. The other "well-known" metric is "speed". Or the distance travelled in a unit time.

For example, if some road segment is 100m, and it takes 10s for a vehicle to move from one end to the other, the "speed" on this segment is "10 meters per second" or 10m/s. Or in more familiar units, 36 km/h.

### Latency

We also care about how much time it takes to get from A to B. For the example road segment, this time or "latency" is 10s.

### Bandwidth and Density

The "bandwidth" of a road is the number of people that can travel through in a unit time. Bandwidth depends on both speed, and how densely people can pack into the vehicle travelling on that road.

For example, a large, 10m-long bus carrying 50 people, carries 5 people/m. A 5m-long sedan, carrying 5 people, carries only 1 person/m.

If the bus were travelling at 10m/s, its bandwidth would be 50 people/s. The sedan would have a bandwidth of 10 people/s.

The number of lanes on the road, also influence bandwidth. For example, if the road had two lanes, each with a bus travelling at 10m/s, its bandwidth would be 100 people/s.

## Complex Routes

In practice, road journeys happen on multiple road segments that form a complex road network. However, the metrics we care about are much the same.

How do the metrics for road segments, "aggregate" to form metrics for road networks?

### Distance and Latency

The Distance or Latency of a route is the sum of the distances or latencies of each of its component road segments.

For example, if a route consists of two segments, the first 100m long, and the second 200m long, and with latencies of 10s and 12.5s respectively, the aggregate distance is 300s, while the aggregate latency is 22.5 seconds.

### Speed

The speed of the route is the sum distance divided by sum latency.

In the previous example, each segment had speeds of 10m/s and 16m/s, respectively. The aggregate speed of the route is 300m / 22.5s or 13.33m/s.

### Maximum Bandwidth

The maximum bandwidth of a route is the bandwidth of the segment with the lowest bandwidth.

In our previous example, suppose the first segment was a single-lane road, while the second segment was a three-lane highway. Also, suppose that traffic on both segments was restricted to 10m-busses. The first would have a maximum bandwidth of 50 people/s, while the second would have a maximum bandwidth of 187.5 people/s.

Now the combined route would still have a maximum bandwidth of only 50 people/s, because it would not be possible to traffic more on the first segment, regardless of the extra capacity of the second.

![Image](https://cdn-images-1.medium.com/max/800/1*tAWPmys0DJxVFKMn38usSw.jpeg)