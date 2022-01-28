#### Article 155 · November 4, 2019

# On First-Time Voters

### 2019 Sri Lanka Presidential Election

In Sri Lanka, the minimum voting age is 18. Since the last presidential election was in 2015, if you are a Sri Lankan citizen born in 1998, 1999, 2000 or 2001, the 2019 edition would likely be your first Sri Lankan Presidential Election.

How will First-Time Voters impact the 2019 election?

## Distribution of FTVs in 2019

[For this article, I define first-time voters (FTV), as voters who are voting for the first time in the Presidential Election. I.e. people who will be old enough to vote this November 16th, but were not old enough to vote in the 2015 Presidential Election. Even if you've already voted in another election, if this is your first presidential election, you are an FTV.]

Sri Lanka last conducted a census in 2012. Hence, I shift the age statistics to compute the number of FTVs. Also factoring in mortality (using Life-Tables) for various age-groups.

The proportions of FTVs by district are:

![Image](https://cdn-images-1.medium.com/max/800/1*7g8qkIDSw2t6-AT3XbPglw.png)

The absolute number of FTVs are:

![Image](https://cdn-images-1.medium.com/max/800/1*VWsDJfq1d3WUTEG6WUBo3g.png)

Many factors could contribute to these differences. Including:

* Life Expectancy. Areas with lower life expectancies would have a larger proportion of youth, and hence FTVs

* Birth Rate. Areas with higher birth-rates would have a larger percentage of FTVs.

* Migration

[I didn't have enodata to analyze these factors in detail]

## How FTVs Vote and Misleading Correlations

Presidential Elections are by secret ballot. Hence, we don't know how a particular age group might have voted.

On the other hand, we could investigate if polling divisions with high numbers of FTVs voted any differently.

In this graph, I analyze the 2015 Sri Lankan Presidential Election. In the X-axis, I plot the proportion of FTVs in a polling division. In the Y-axis, the difference in votes between the NDF and the UPFA.

![Image](https://cdn-images-1.medium.com/max/800/1*0G7I4Wph9roQTb2CTPFzMg.png)

The fitted line has the equation:

(NDF Vote minus UPFA Vote) = 13.82 x (First-Time Votes) -107.53 %

If you read this blindly, you might conclude that for every 1% of additional FTVs, the NDF won an additional 13.82% votes. This is true, but not a useful observation. Let's see why.

### A Tale of Two Towns

Consider the following "toy" example.

There are two fictional polling divisions, "Rich-Town" and "Poor-Town" side by side. The voters of Rich-Town have excellent healthcare and nutrition and hence enjoy a high life expectancy. "Poor-Town" on the other hand, is not so lucky. Healthcare, nutrition and life-expectancy lag behind Rich-Town.

In 2015, Rich-Town had 1000 voters, of whom 100 were FTVs. Poor-Town also had 1000 voters. But with its lower life-expectancy, had a larger FTV population of 200.

Two parties, The Black Party and White Party, contested the 2015 presidential election. The Black Party has policies favouring wealthier voters and hence expected more votes in Rich Town. The White Party, on the other hand, supported poorer voters and expected more votes in Poor Town.

In Rich-Town, the Black Party won 600 votes to the White Party's 400 votes. We don't know how the 100 FTVs contributed to this, because of secret ballots. In Poor-Town, the White Party won 700 votes, to the White Party's 300.

In Rich-Town, the White minus Black Party Votes difference was -20%. While in Poor-Town it was +40%. We also know that Rich-Town had 10% FTVs while Poor-Town had 20% FTVs.

Now, could we conclude that for every 10% increase in the FTV proportion, the White Party's vote increases by 60%?

We can't. The reason is that in this toy example, the FTV proportion is not the "causal" factor which influences the final vote. It is merely "correlated". Both FTVs and non-FTVs in Rich-Town tend to support the Black Party, while both FTVs and non-FTVs in Poor-Town support the White Party. The "causal" factor is probably income or the parties' policies towards healthcare.

...

Sri Lanka is Rich-Town and Poor-Town. The "causal" factors have probably more to do with ethnicity, economics, and regional politics, than youth issues or FTVs.

This "confounding" we see in the national result does not go away, even when we look at smaller areas. For example, in the Southern Province, the pattern is even more exagerated.

![Image](https://cdn-images-1.medium.com/max/800/1*oiiNHSdr5RKLbrjQ4fd_9w.png)

## So what can we say?

We don't have enough data to say how exactly FTVs will vote. However, if we assume that FTVs voting within a given polling division will be similar to non-FTV voting, we can estimate the effect the new voters will have on the final result.

In 2015, there were very distinct patterns in how various districts voted for various parties. In On Non-Voters, I introduced the concept of Deltas. A Delta is how much of a lead a party gets over the 50% limit needed to win an election. This is how Deltas distribute across the country.

![Image](https://cdn-images-1.medium.com/max/800/1*braxiVNB6gzz5aXOrc19vQ.png)

Similarly, we could compute Deltas for only first-time voters.

![Image](https://cdn-images-1.medium.com/max/800/1*q8RePSg1y2wjfDYyXyOV_A.png)

Overall, if FTVs vote in 2019 the same way non-FTVs do, and everyone votes in 2019 as they did in 2015, the NDF candidate would win about 20K incremental votes from FTVs.

## Concluding Thoughts

My main conclusion is that there is very little data to say anything quantitative about first-time voters.

Other factors like ethnicity confound trends, and we are forced to make hard assumptions like "FTVs will vote exactly like non-FTVs" and "2019 will be exactly like 2015".

Either way, while the impact of FTVs will (probably) not be significant for the election, the election should be significant for FTVs. It will be their first participation in our representative democracy. That itself should be significant.

Happy Voting!