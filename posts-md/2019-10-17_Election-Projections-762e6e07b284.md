#### Article 137 · October 17, 2019

# Election Projections

### Predicting the 2019 Sri Lankan Presidential Election

After polling stations close at 5pm on Saturday, November 16th, the arduous process of vote counting begins. With a record number of candidates, counting might take even longer than usual. It might be as late as Monday (November 18th) when the first results are announced.

The results of smaller polling divisions and postal votes are usually released first. Followed by larger polling divisions. The "size" of the polling division is not the only factor that determines release time. Many polling booths, particularly in remote mountainous parts of the country, are many hours away from counting stations. Hence, travel time also influences how soon results are released.

Either way, some results are announced before others.

The question I want to investigate in this article is:

>>> Can we use early results to project and predict the final result? And if so, how accurate would such a projection be?

## The Experiment

To find out, I ran the following experiment with the previous (2015) presidential election:

* I assumed that election results were reported in order of result size. Starting with smaller results like postal votes. Ending with larger polling divisions like Homagama, Kaduwela, and Nuwara Eliya-Maskeliya.

* For each set of reported results, I built a linear regression model that predicted the final result based on these reported results. The model was trained on the results of the previous six presidential elections.

* To validate if my predictions were reasonable, I also computed "error bounds" of the statistics.

For my experiment, I ignored the travel time factor, and assumed that "time to report" is proportional to the "number of votes to count". It is probably possible to to get the exact "release time" from the Election Commission, or by tracking how media organizations reported the results in 2015, but this seemed too much work. "Number of votes to count" felt good enough.

## 2015 Results

The smallest results for 2015 were the Vanni, Batticaloa and Puttalam district postal votes. Followed by Nuwara Eliya, Polonnaruwa, Trincomalee district postal votes.

![Image](https://cdn-images-1.medium.com/max/800/1*E4RACDKrLneVXZG8TLyRZg.png)

Kayts was next, the smallest polling division, by total polled.

![Image](https://cdn-images-1.medium.com/max/800/1*p0oRMElutyOgR6ivYx6_1A.png)

After each result, I computed the expected final votes for the two major candidates: Mahinda Rajapaksa (UPFA — Blue) and Maitripala Sirisena (NDF — Red).

Plotting the predictions, I got the following graph.

![Image](https://cdn-images-1.medium.com/max/800/1*u6f__dSHBVAHEc2jA41XHw.png)

The thick blue line indicates the projected vote proportion for the UPFA. The two thin blue lines either side, indicate the upper and lower error bounds. Similarly, the red lines correspond to the NDF.

While there is a lot of noise early, indicating the model is weak, and data from previous elections is not representative for small numbers of reported results, it quickly settles down. The obvious observation is that the election is very close. For most of the graph, the blue lines and red lines overlap, indicating that the election is "too close to call".

To see this better, let's zoom in:

![Image](https://cdn-images-1.medium.com/max/800/1*pPskeaWDNKMnLRqyuhh-aQ.png)

While the blue leads red in some places, and red leads blue in other places, the lower error bar for red (almost) never exceeds the upper error bar for blue, and vice versa. In other words, the best case for blue is never worse than the worse case for green, and vice versa. In other words: Too close to call.

There are some intriguing individual results.

At Hanguranketha, the projection shifts in favour of the blues. The blues do better than expected in a polling division that has favoured the reds (and greens) in the past. Note, the result was still statistically insignificant.

![Image](https://cdn-images-1.medium.com/max/800/1*KRMShrP-oBaddHXk5zeDqw.png)

The opposite happens with Colombo North.

![Image](https://cdn-images-1.medium.com/max/800/1*2X-ONJQxpB6eAE-KppiFXA.png)

The final results were:

![Image](https://cdn-images-1.medium.com/max/800/1*Lzp3-azn3E9MxN4UJyGWAw.png)

You can watch a video with a complete roll of "Realtime Results and Projections" here:

## 2010 Results

The 2010 Sri Lankan Presidential Election was a one-sided affair, where the UPFA candidate Mahinda Rajapaksa, comprehensively beat the NDF candidate Sarath Fonseka. So comprehensively that our projection picked the winner after about 30 results.

![Image](https://cdn-images-1.medium.com/max/800/1*cMTVsbRKLiItmpFZi3ow0Q.png)

Note that after about 30 results, the best case for red is worse than the worst-case for blue. Hence, the projection (indicating that blue would win) is statistically significant.

## 2005 Results

The 2005 presidential election was the closest in Sri Lankan history. The UPFA's Mahinda Rajapakse won 50.29% of the vote, just 180,786 votes more than the UNP's Ranil Wickramasinghe's 48.43%.

![Image](https://cdn-images-1.medium.com/max/800/1*9WN_BA0fBT0IMv4aBnkapw.png)

While the projection for the UPFA led that for the UNP for most of the graph (consistent with the final result), the difference was never statistically significant. Hence, again, "too close to call", throughout.

## Concluding thoughts

In On Floating Voters and Bellwether Polling Divisions, I demonstrated the difficulties in predicting election results before elections. In this article, I went even further and demonstrated how difficult predictions are, even after some results are announced.

And this time around (2019), accurate predictions and projections are likely to be even more difficult, particular with several third parties vying for the spotlight, and a record number of candidates overall. We also have a substantial number of first-time voters, who might diverge from the past in their voting preferences.

Either way, come November 16th, 17th, 18th and possibly 19th, statistics might be scratching its poor head. With a confused look on its face.

...

### Bonus: Shameless Plug

The "Realtime Results and Projections" was the first video I uploaded to YouTube since 2011 — when I shared a set of piano minatures that I wrote, inspired by our countryside. If you don't enjoy the article, you might at least enjoy the music

You can find the sheet music here: https://www.facebook.com/NuwansNuances/photos/a.140174619505650/140180422838403/