#### Article 148 · October 26, 2019

# A Machine's Opinion

### 2019 Sri Lankan Presidential Election

>>> Are all Sri Lankan polling divisions the same? Are some different from others?

If you ask a Sri Lankan this question, you're likely to get many answers. Some interesting. Some boring. But what if you don't ask a Sri Lankan? What if you don't even ask a human? What if you ask a machine?

In Computer Science-speak the term "Clustering" refers to:

>>> ...the task of grouping a set of objects in such a way that objects in the same group (called a cluster) are more similar (in some sense) to each other than to those in other groups (clusters) [Wikipedia]

We could give a machine some data about polling divisions, and see how it might cluster them. What it decides to put into what cluster would depend on the its answer to the question:

>>> "Are all Sri Lankan polling divisions the same? Are some different from others?"

## Details on the Methodology

For each of the last four presidential elections (1999 to 2015), I represent each polling division (and postal votes result) by the percentage votes won by the Blues (SLFP, PA, or UPFA), Greens (UNP, or NDF), and others.

For example, Mawathagama would be:

![Image](https://cdn-images-1.medium.com/max/800/1*EiGg2POYNogWqtzoTkJZIQ.png)

Next, I asked a machine (my laptop), to cluster this data using K-means clustering. The "K" refers to the number of clusters.

## The Results

### The Singleton Cluster (K = 1)

Why build a "cluster" of size one? Would it not consist of all the data points? All the election results for the country? It would.

However, running the K-means cluster algorithm with K = 1 is interesting, because it gives you a sense of how various polling divisions are distributed relative to the islandwide result.

![Image](https://cdn-images-1.medium.com/max/800/1*5t0Xq6yWCcYw79RfvxY8pA.png)

Let's see what the machine outputs:

![Image](https://cdn-images-1.medium.com/max/800/1*m47TXsq4vakYVCCY5B-KBQ.png)

The mean of the cluster represents the "average results" for the members of that cluster. With this singleton cluster, the mean is the average result of the entire country.

The machine also outputs the members of the cluster. And the distance of each member is from the mean of the cluster.

![Image](https://cdn-images-1.medium.com/max/800/1*2oHdSI9SL_ugkKYEubqmAQ.png)

Distance is the summed absolute difference between each percentage statistics for the member and the mean. For example, the various results for "Mawathagama" differs from the final islandwide result (the mean for this cluster) by a sum of 8.9%. I have sorted the cluster members in order of distance from the mean.

The polling divisions closest to the mean of the singleton cluster (Mawathagama, Yatinuwara, Moratuwa, Pelmadulla, and Teldeniya etc) are the polling divisions that have the results closest to the national results. They are equivalent to "percentage bellwethers" that I presented in Bellwether Polling Divisions.

### Safe Green and Leans Blue (K = 2)

![Image](https://cdn-images-1.medium.com/max/800/1*j91FAS87ZIF_PLkbLTSIXA.png)

With K = 2, the machine "sees" the most obvious way Sri Lankan polling are different: many lean Blue, while others lean Green.

![Image](https://cdn-images-1.medium.com/max/800/1*AXXM_5StHe3bXC9z3LWWHw.png)

The first cluster (2.1) represents about 15.2% of the voters, and consists of Safe Green polling divisions, which tend to vote 60–75% for the Greens. The results closest to the mean are Nuwara Eliya-Maskeliya, Kalkudah, Jaffna, Puttalam and Colombo North.

![Image](https://cdn-images-1.medium.com/max/800/1*bGBQb9ZB7Qim4o5Mpqf7YQ.png)

The second cluster (2.2) is much larger, and consists of polling divisions that tend to vote 50–60% for Blue. The results closest to the mean are Mirigama, Divulapitiya, Avissawella, Horowupotana, and Kalutara.

![Image](https://cdn-images-1.medium.com/max/800/1*Zsvm-b2S4Z8ZGSMf5qPmyg.png)

While the K =2 pattern is interesting, it is somewhat obvious, and we could like more nuance. So let's try K = 3.

### Swing Polling Divisions (K = 3)

![Image](https://cdn-images-1.medium.com/max/800/1*f0HKDYwfjsHJMUAgEfKLIQ.png)

With K = 3, we see a new type of polling division: Swing polling divisions.

The smaller Safe Green (2.1) cluster stays largely the same (as 3.1), with the exception of its mean changing from Nuwara Eliya-Maskeliya to Colombo North. This is because some of its members moved to other clusters. This is a common phenomenon with clustering. Cluster identities are somewhat arbitrary, and tend to change.

![Image](https://cdn-images-1.medium.com/max/800/1*_JoKSmgz9BrTHRzCbF4P4w.png)

Cluster 2.2 splits into two new clusters. A Swing result cluster (3.2) and a Safe Blue cluster (3.3).

![Image](https://cdn-images-1.medium.com/max/800/1*_hZpAeLzMpQ04HpwtVLLUQ.png)

The Swing polling divisions voted for the Greens in 2005 and 2015, and the Blues in 1999 and 2010. They would have likely "swung" the election to the Greens in 2005, had the LTTE-driven boycott not happened. In most elections, the gap between winner and looser was close. The results closest to the mean are Kundasale, Beruwala, Rattota, Bandarawela and Kurunegala.

![Image](https://cdn-images-1.medium.com/max/800/1*SFp9l2tk6RrZ4hw5z6MG1g.png)

The Safe Blue polling divisions tend to vote 55% to 65% for the Blues. Results closest to the mean are Kegalle, Bandaragama, Balapitiya, Horana, and Hiniduma.

![Image](https://cdn-images-1.medium.com/max/800/1*T4cZfwsLwWab9c3WaxN6ZQ.png)

### Safer Blue Polling Divisions (K = 4)

![Image](https://cdn-images-1.medium.com/max/800/1*1cduTb3OxbrOKBzHYwC72A.png)

Cluster 4.1 and 4.2 are similar to the Safe Green and Swing clusters 3.1 and 3.2 respectively. We see a split of the Safe Blue cluster (3.3) into two new clusters 4.3 and 4.4.

![Image](https://cdn-images-1.medium.com/max/800/1*znGbP5D47ENxU0OHMpCn6A.png)

Cluster 4.3 is still Safe Blue, voting about 50% to 60% for Blue.

![Image](https://cdn-images-1.medium.com/max/800/1*4AtChCIipPX5cNXNPLGgsg.png)

Cluster 4.4 is Safer Blue, with support for Blue over 55%.

![Image](https://cdn-images-1.medium.com/max/800/1*GPO8h0TtxuSsC8G3-wI2Hg.png)

### Blue except 2015 (K = 5)

![Image](https://cdn-images-1.medium.com/max/800/1*6VkqHWLnwjNrzshdtHCRmg.png)

Clusters 5.1, 5.2, and 5.3 are very similar to clusters 4.1 (Safe Green), 4.2 (Swing), and 4.3 (Safe Blue). We see Cluster 4.4 (Safer Blue) split into two new clusters.

![Image](https://cdn-images-1.medium.com/max/800/1*hd97Fb05zu1NZkQWnUlWBA.png)

Cluster 5.5 is very similar to 4.4, with support for Blue over 60%.

![Image](https://cdn-images-1.medium.com/max/800/1*Nl78_DdgfkS6hI6CcXJPnw.png)

Cluster 5.4 is more interesting. While historically it supported Blue with nearly 60% on average, in 2015, Green had a much stronger showing, with a vote of nearly 50%. The results closest to the mean included Biyagama, Panadura, Minuwangoda, Kaduwela, and Kalutara.

![Image](https://cdn-images-1.medium.com/max/800/1*5OLu1g6aczLf0LxXSc2log.png)

### K ≥ 6

We could continue clustering for larger K, but I think we have enough data to answer our original question.

## A human interprets on behalf of the machine

Here's a summary of what our machine did:

![Image](https://cdn-images-1.medium.com/max/800/1*3Rny_YwW8a6U89rhBw1FTQ.png)

K = 5, is our machine's final answer to the question, "Are all polling divisions the same?". It says, "no". And it goes on to describe five quite different types of polling divisions.

The next obvious question is,

>>> "Can we use what the machine said, to predict the 2019 Sri Lankan Presidential Election?"

On the first inspection, it might seem that Green has no chance. This would probably be the case if the next election was first-past-the-post. Blue would likely win a majority polling divisions. However, presidential elections are different beasts. Each vote matters equally.

Let's do some more detailed math.

Consider the "Safe Green" cluster. Using the cluster mean as a guide, we could estimate that the Greens would probably get 55.1% to 78.0%, while the Blues would get 19.9% to 40.4% of the vote. Considering that the safe green cluster is about 11% of votes, this would equate to 6.1% to 8.6% votes islandwide for the Greens, while the Blues would get 2.2% to 4.4% islandwide.

![Image](https://cdn-images-1.medium.com/max/800/1*PoJXyRuShT65b7KszpVD3A.png)

Applying this logic to all the clusters, we get the following aggregate statistics:

![Image](https://cdn-images-1.medium.com/max/800/1*aieN22u8ptW1nS6A1SOByA.png)

Green would probably get between 38.4% and 51.2% of the vote, and the Blues between 46.4% and 59.1%. The lower bounds are similar to the 39% and 44% numbers that I computed in On Floating Voters. Hence, at least by these numbers, the elections is still wide(ish) open.

## Concluding Thoughts (by a Human)

Statistics assumes that "the future will be like the past". This might not be the case. The 2019 presidential election could be nothing like 1999, 2005, 2010 and 2015, upon which my laptop pontificated. We might even have a completely different "colour" winning the election. Hence, as always, administer that cautionary pinch of salt.

On the other hand, the "Machine's Opinion" is (at least for me) quite interesting. For example,

* Come post-November 16th, I'll be keeping an eye on the "percentage bellwether" type polling divisions unearthed by the K =1 clustering. Like Mawathagama, Yatinuwara, Moratuwa, Pelmadulla, and Teldeniya. Their results are likely to match the final islandwide result closely.

* I'll also keep an eye on the 30 or so Swing polling divisions. Like Wattala, Udunuwara, Matale, Harispattuwa and Mawanella.

* Then there are the mysterious Safe (except 2015) Blue polling divisions like Biyagama, Panadura, Minuwangoda, Kaduwela, and Kalutara. Will there be "exceptions" in 2019 also?

Happy Voting!