#### Article 200 · January 2, 2020

# Hills of San Francisco

### From first principles

[Originally published on Facebook in 2018]

I'm a big fan of "hiking" cities. A couple of years ago, guided by Adah Bakalinsky's excellent book "The Stairways of San Francisco", I completed 29 walks (the book has 30*), which took me to over 400 of San Francisco's stairways. Some of the stairways were hidden in innocuous neighborhoods, while others climbed-up San Francisco's many hills. The summits of these hills afford some of the most beautiful views of the city, and the Bay.

[* I left one out, so that I'd always have a reason to return to SF]

![Image](https://cdn-images-1.medium.com/max/800/1*9-aUlwCALB_3RJInnhwsSQ.jpeg)

Like many cities, San Francisco was once claimed to be built on seven hills (Telegraph Hill, Nob Hill, Russian Hill, Rincon Hill, Twin Peaks, Mount Davidson and Mount Sutro). The other cities include Rome, Jerusalem and Mecca. However, from my stairways walks, I was sure that there were many more. Gladys Hansen's San Francisco Almanac claimed that there were 42. Other lists on Wikipedia and various travel blogs had slightly varying lists each with around 50 hills.

Following-up from my stairways project, I wanted to climb every hill in San Francisco — which I ended up doing in October and November 2016. This note is a belated attempt to document some of my findings and reflections.

## What is a Hill?

Before climbing a hill, you need to find it. But before you can find it, you need to define it. There was no "definitive list" of San Francisco's hills. Like I mentioned, the number varied from seven to 50. Hence, I needed to "define" a hill — from first principles

### Question 1: What is a Hill?

According to wikipedia, "A hill is a landform that extends above the surrounding terrain." Or to put it more simply, a hill is a piece of land, that is at a higher elevation than the land around it. Simple enough so far.

### Question 2: How high must a hill be to be called a hill?

While a Mountain is often defined as a hill that is more than 300m (~1000ft), I couldn't find a "minimum height limit" for a hill. I thought of using 50m as a rough starting point. In retrospect, this proved a serendipitous choice.

### Question 3: How exactly does one measure the height of a hill?

Geographers use the concept of "topographic prominence"; the "prominence" of a hill being the height of the hill from the lowest contour line surrounding it, which contains no higher peak.

![Image](https://cdn-images-1.medium.com/max/800/0*-3dveh0uzI9gTAID)

## My Data

I started with some geographic information system (GIS) data for San Francisco, which tabulated altitude by longitude and latitude. The altitudes looked something like this. Dark Green marks sea level (0m); Yellow marks 50m; Dark Red 250m. For reference, I've also marked some "official" San Francisco hills.

![Image](https://cdn-images-1.medium.com/max/800/0*MYtDGZoO7yM-RufL)

Note: My definition of "San Francisco" is somewhat arbitrary. The San Bruno mountains just south of the area on my map, are actually much taller than the tallest hills of San Francisco. But for simplicity, I excluded these mountains and looked at a rough square north of these. Interestingly, this my chosen area also captures part of Yerba Buena island.

Next, I wrote some code to find the topographic prominence of each location. The colour denotes the prominence of the highest hill within the contour line containing a point. As before Dark Green marks sea level (0m); Yellow marks 50m; Dark Red 250m. The labels including the rank, prominence and height of the hills.

![Image](https://cdn-images-1.medium.com/max/800/0*drUXZANKl1O67Jx1)

![Image](https://cdn-images-1.medium.com/max/800/0*4sTuu7xAXdj-dF08)

![Image](https://cdn-images-1.medium.com/max/800/0*c8wxb_wDsnpH_uAe)

## A Short Analysis

Conveniently, picking the minimum prominence for a hill as 50m, resulted in exactly 50 hills for San Francisco. That is, there were 50 hills in San Francisco with a prominence of at least 50m. As I mentioned, serendipitous.

My new list of hills differed from most official lists in several interesting ways. For example,

* Mount Davidson (271ft) is considered the tallest hill in San Francisco. Mount Sutro (250ft) is usually listed as the second tallest, as it has the second tallest altitude from sea level. However, situated on a plateau, it's prominence was only 115m. According to my data, the second tallest hill was the North Peak of Twin Peaks, with a prominence of 258ft. This difference between prominence and altitude was significant for many other hills.

![Image](https://cdn-images-1.medium.com/max/800/0*Ua0LgquR8ygoEo19)

2. Several "official" hills (including Rincon Hill) didn't appear on my list, because their prominence was below my 50m limit.

![Image](https://cdn-images-1.medium.com/max/800/0*XOW6QUc2u85c0Ys_)

3. Many well known hills (including Telegraph Hill and Nob Hill) were not single hills but clusters of hills.

![Image](https://cdn-images-1.medium.com/max/800/0*CIXo8DL2l6xRhPmS)

4. There were parts of the City (e.g. the Presidio) which had many hills (accordingly to my definition) which didn't have official names.

![Image](https://cdn-images-1.medium.com/max/800/0*2Zjs8ys6is53VOOG)

## My top 10 hills

Most hills are special for some reason, and it's difficult to rank them. But for the sake of coming of with a "Top 10", I attempted to do so. My criteria are roughly: 1) views from the top; 2) surrounding neighbourhood (after all, these are urban hills); and 3) the climb up.

* (My Favourite) Telegraph Hill (74m Prominence — or 29th most prominent). Amazing views of Bay, both bridges and City. Interesting garden and houses on the way up. Right in the middle of the city.

* Bernal Heights (126m, 6th). Probably my favourite views of the city, from all directions.

* Pacific Heights (92m, 16th). Beautiful views of the Bay, especially down the Lyon Stairs.

* Mount Davidson (270m, 1st). Views. Interesting climb through wooded forest.

* Twin Peaks — North (258m, 2nd). Views of the city. Though a bit too touristy.

* McLaren Hill (151m, 4th). Several peaks. Lots of hiking trails. Quiet. Views of the city.

* Russian Hill (52m, 48th). The hill itself is not particularly interesting, but there are many picturesque ways down the hill, including the famous Lombard Street, Green street, and Vallejo Street.

* Strawberry Hill (53m, 45th). Right in the middle of Golden Gate Park. Beautiful views of the park.

* Mount Sutro (115m, 9th). Views. Interesting Climb-up.

* Edge Hill (81m, 24th). Views of the City.

![Image](https://cdn-images-1.medium.com/max/800/1*BY4a6qVIV7LCqauwjGcURA.jpeg)

![Image](https://cdn-images-1.medium.com/max/800/1*oCYH0o6E7-KW2ljPH3V1VQ.jpeg)

![Image](https://cdn-images-1.medium.com/max/800/1*W6J4-I8Gew2NQcgJ_gYelQ.jpeg)

## Next Project

Views from the tops of hills can be nice, but the climb up can be strenuous. My next project is to climb all these hills of San Francisco in the most optimal order — where "most optimal order" means climbing the hills such that "distance climbing uphill" is minimized. That should be an interesting problem to solve.