#### Article 238 · April 25, 2020

### Geography of Sri Lanka

# Where can I see Adam's Peak?

### And other mountains

[If you're not interested in the Maths, please skip to the Appendix]

As the South-West monsoon picks up, the air quality in the South-West of Sri Lankan in general, and Colombo in Particular, improves. Coupled with the CoViD19 Lockdown in the Colombo District, and the resulting implosion of traffic, Colombo air is uncharacteristically clean.

The good air not only makes breathing easier, but also seeing easier. And so, unsuprisingly, the internets are full of sightings of mountains; Adam's Peak in particular. Here's one of my favourites by Namal Kamalgoda.

![Image](https://cdn-images-1.medium.com/max/800/1*gi4wbkf5mQewxaZd8nKqJQ.jpeg)

But from where can you see Adam's Peak? And what else can you see?

Read on to find out.

## How far can we see?

The curvature of the earth puts a limit on how far we can see. We know this from disappearing ships over the horizon, as we stand on the sea shore. But how far away is the horizon exactly?

A bit a simple maths, including Pythogoras's Theorem will tell us.

Suppose,

```
R = Radius of the Earthh = The height of the observer d = The distance to the horizon
```

Then, R, d and (R + h) form a right-angle triangle. (R + h) is the hypotenuse or the side opposite the right angle.

Then,

```
By Pythogoras's Theorem,R² + d² = (R + h)²
```

```
Therefore, d² = (R + h)² - R²= R² + 2Rh + h² - R²=(2R + h).h
```

```
Assuming that R is much larger than h, we can ignore the first h, giving,
```

```
d² = 2Rh
```

```
And finally,
```

```
d = √2Rh
```

For example, if you were 1.8m (just under 6ft tall, or 0.0018km), and given that the earth's radius is 6,371 km, we get,

```
R = 6371h = 0.0018d = √2Rh = 4.789
```

The horizon would be about 4.8km away.

Similarly,

* If you were 1.5m (or just under 5ft tall), the horizon would be about 4.3km away

* If you were standing at the top of a 150m tall building, the horizon would be about 44km away.

* If you were standing at the top of the Lotus Tower (350m), the horizon would be about 67km away.

![Image](https://cdn-images-1.medium.com/max/800/1*e09BRhFAPVaUKi1PLD12Rw.png)

Why did I bring up horizons and lotus towers? To make this simple point: The higher-up you are, the further away you see.

## What can we see?

Adam's Peak is about 80km away from Colombo. That's even further than the horizon from the top of the Lotus Tower. So, does that mean we can't see Adam's Peak from Colombo.

Not quite.

The curvature of the earth will hide the bottom part of a mountain that is far away. But if the mountain is high enough, the top part might be visible. Calculating how much, needs some more calculations and more Pythogoras.

Suppose,

```
D + d = The distance from the observer to the mountain(Note, D is the distance to the mountain, beyond the horizon)H = The height of the mountain b = The height of the bottom part of the mountain hidden by the curvature of the earth
```

Now, R, D and (R + b) form a right-angle triangle. (R + b) is the hypotenuse.

Since we know D, and R, we can compute b as follows:

```
By Pythogoras's Theorem,R² + D² = (R + b)²R² + D² = R² + 2Rb + b²
```

```
D² = 2Rb + b²= b(2R + b)
```

```
Assuming that R is much larger than b we getD² = 2Rbb = D² / 2R
```

For example, if we are looking towards Adam's Peak from a 100m tall building in Colombo, we get,

```
R = 6371d = 44 (See above)D = 80 - d = 36b = 0.1017
```

Hence, the bottom 102m of Adam's Peak would be cut-off. Since the mountain is 2,243m high, we should be able to see the top 2,141m of it.

What if we were not on a tall building, what we were 1.8m tall, and at sea level? Then,

```
b = 0.44381
```

Or, the bottom 444m of Adam's Peak would be cut-off, but leaving plenty off the top. Hence, we should be able to see Adam's Peak without the aid of tall buildings.

![Image](https://cdn-images-1.medium.com/max/800/1*vq31UdBMTjplGbyQcwETMg.png)

While in theory we should be able to see Adam's Peak from the ground, in practice, buildings and other obstructions get in the way. So unless your in a place with little obstruction (e.g. a large ground), some building is likely to block your view. That is why, in practice, you need to get on top of something.

## Modelling what we can see

We know we can see Adam's Peak. But what else can we see? Can we, for example, see Sri Lanka's tallest mountain Pidurutalagala (2,524m)? More generally, can we create a "model" to visualise everything we could see?

### α and ϐ

Suppose you are in the top floor of the World Trade Centre (WTC) in Colombo Fort. You are about 150m above sea-level. Suppose you are looking out of a window facing east, and your horizontal vision spans from North (0°) to South (180°). Let's call this horizontal angle α.

Now, we can look at the horizon (0°), at some point below the horizon, upto directly below us (-90°), or above the horizon, upto directly above us (+90°). Let's call this vertical angle ϐ.

Everything that we see has some α and ϐ. If two things have the same α and ϐ, whatever that is closer will block that which is further away. Hence, we can "model" what we can see by computing its α and ϐ, and seeing if there is some closer thing with the same α and ϐ, that will block it.

Suppose you are looking at Adam's Peak? How do you compute α and ϐ?

If you can see the mountain clearly, you can measure α with a compass, and ϐ by the angle at which you are looking up.

But what if you can't see the mountain? Or you see some mountain, but are not sure if it is Adam's Peak?

We can compute both α and ϐ using a map and altitude information.

### Computing α

The WTC is located at (6.9327° N, 79.8438° E). Adam's Peak is at (6.8096° N, 80.4994° E). α is the tangent of the line between these points.

![Image](https://cdn-images-1.medium.com/max/800/1*qDCloRJGr1bMoqPfa0CnHw.png)

Or,

```
lat0, lng0 = 6.9327, 79.8438 (World Trade Centre, Colombo 1)lat1, lng1 = 6.8096, 80.4994 (Adam's Peak)
```

```
Tan (α - 90) = (lat0 - lat1) / (lng1 - lng0)= (6.9327 - 6.8096) / (80.4994 - 79.8438)= 0.1878
```

```
α = Tan⁻¹ 0.1878 + 90= 100.7
```

So, Adam's Peak should be visible at about 100.7°, or 10.7° from East to South.

### Computing ϐ

![Image](https://cdn-images-1.medium.com/max/800/1*nHh5Tr5-N4VmdoJFareBbw.png)

```
By the symmetry of triangles, x = D (H - b) / (R + b)y = R (H - b) / (R + b)
```

```
Tan ϐ = y / (x + D + d)ϐ = Tan⁻¹ y / (x + D + d)
```

For our WTC scenario,

```
D + d = 80D = 36 (see above)(H - b) = 2.141 (see above)(R + b) = 6371.102
```

```
Therefore,x = 0.0121y = 2.1410
```

```
And, ϐ = Tan⁻¹ y / (x + D + d)= Tan⁻¹ 2.1410 / (0.0121 + 80)= 1.53°
```

Or 1.53° above the horizon.

Hence, now we can compute α and ϐ for every location in Sri Lanka. Using this information, we can visualize mountains. For the visualisations below, I use latitude and longitude information about Sri Lankan mountains from Wikipedia, and altitude information from USGS.

This is what Adam's Peak should look like if viewed from the top of WTC:

![Image](https://cdn-images-1.medium.com/max/800/1*PbXRzXU8pRVXptu0lQzbHA.png)

## Appendix: Examples

### Colombo (World Trade Centre, 150m)

![Image](https://cdn-images-1.medium.com/max/800/1*qryUbJ32JOlcVA7qV_gMUA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*R0catPoyG-OZesbcwXVTzA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*PbXRzXU8pRVXptu0lQzbHA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*y3j5zLcwiuzQMpOiJp-Ifg.png)

### Matara (Hypothetical 150m Building)

![Image](https://cdn-images-1.medium.com/max/800/1*zhOfd-Eebym0hOLdYbLQYg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*W2IViJ0Jz0mhC6SGOiqFDA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*7vyZEjIyvYUcqbUqnSKtWg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*atNuSqQDXopG4VrpBM8J2A.png)

![Image](https://cdn-images-1.medium.com/max/800/1*agJvc4gpMD9xCjVX1E7rJA.png)

### Batticaloa (Hypothetical 150m Building)

![Image](https://cdn-images-1.medium.com/max/800/1*9JLFt-hvREyDJgf1OGeweQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*rjKIh3f24w4RDUqGArDMXA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*oO7jipdrp6DxN9HK-wivkw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*tTNQpmDMoEJ0ncIGT_pfFw.png)

### Kadugannawa Rock View (500m)

![Image](https://cdn-images-1.medium.com/max/800/1*eANkTi1UntpZRZGCp0DcXA.png)

### Sigiriya (Top of the Rock, 349m)

![Image](https://cdn-images-1.medium.com/max/800/1*IvI7Ul6d3TpXnBAQun1IIA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*4Yk-wY1cDZgSiElzXg8mMg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*AQHNM5fxyLuFUQ5jDIUP0g.png)

### Anuradhapura (Hypothetical 150m Building)

![Image](https://cdn-images-1.medium.com/max/800/1*l7oRu3yyPoMp-YwuMjN_Iw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*OXqZpcs9Ou1iTwAGcOdZEA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*mqMVZ8hing3EjW-RI_4N_g.png)

### 20km West of Colombo Harbour (at 0m)

![Image](https://cdn-images-1.medium.com/max/800/1*Rw8iBIct2bDZmCCVnE_tcw.png)

### 30km West of Colombo Harbour (at 0m)

![Image](https://cdn-images-1.medium.com/max/800/1*Et9Kp_WCcaazmqa5dByIlQ.png)

### 35km West of Colombo Harbour (at 0m)

![Image](https://cdn-images-1.medium.com/max/800/1*NncPOO-WYRSHYJsxBtoZ3w.png)

## Appendix: Special Case of Nearby Mountains

What if the mountain is "before" the horizon?

![Image](https://cdn-images-1.medium.com/max/800/1*QHSQixid2EppExdviQatfw.png)

We modify computing ϐ as follows:

```
By Pythogoras's Theorem,R² + (d - D)² = (R + b)²R² + (d - D)² = R² + 2Rb + b²
```

```
(d - D)² = 2Rb + b²= b(2R + b)
```

```
Assuming that R is much larger than b we getD² = 2Rbb = (d - D)² / 2R
```

```
By the symmetry of triangles, (D - x) = (d - D) (H - b) / (R + b)Therefore,x = D - (d - D) (H - b) / (R + b)y = R (H - b) / (R + b)
```

```
Tan ϐ = y / xϐ = Tan⁻¹ y / x
```