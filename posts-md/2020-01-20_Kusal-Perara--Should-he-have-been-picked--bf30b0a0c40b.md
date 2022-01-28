#### Article 206 · January 20, 2020

# Kusal Perara: Should he have been picked?

### A Machine's Opinion

Kusal Perera was left out of the 15-man Test squad for the ongoing series against Zimbabwe. Many felt that this was a mistake. Many quoted Perera's match-winning 153 against South Africa as possibly the best innings of 2019. Why was such a man left out of the squad?

![Image](https://cdn-images-1.medium.com/max/800/1*taP16K3-rWQARzIT4tv2aA.jpeg)

On the one hand, I know very little about cricket. And even less about how test squads are picked. On the other hand, I was curious about the question: Was it reasonable to leave KP out? And was there a data-driven answer to this question?

## How to pick a batsman

How might we use data to pick a batsman? Why would one batsman be better than another batsman?

Batsman score runs. All other things equal, more runs the better. Hence, we could try and predict the runs a batsman would score. And pick the batsmen with the most predicted runs.

And this is precisely what I did. I built a model that predicts how many runs a batsman is likely to get in their next inning. Based on their past performance during the last 3 years.

The output of the model is a distribution. A range of possible scores.

For clarity, I picked three points on this distribution.

* "Meh" day. What the batsman would score on, not a bad day, but a "very ordinary" day. The 25th percentile of the score distribution.

* "Average" day. The median or 50th percentile of the score distribution.

* "Good" day. The 90th percentile of the score distribution.

Caveats: As I said, I looked at test performance in the last 3 years. Hence, this excludes performance in other formats (which might be correlated with test performance). It also, obviously, excludes new batsmen with no test history. But since the question was "should KP bein the squad?" and since the other squadees had test history, these didn't seem to matter.

## "Average" day

If we sort players by "how much they would score on an average day", Dickwella, Karunaratne, Oshada Fernando, Dhananjaya de Silva, and Mathews head the pack. All five are in the squad.

![Image](https://cdn-images-1.medium.com/max/800/1*SciadU2Htn8TlpDvmaOEaQ.png)

Kusal Perera comes 6th. Ahead of Thirimanne, Kusal Mendis and Chandimal. Who are all in the squad. Hence, if we go by our model's "average day" prediction, Kusal Perera probably should have been picked.

Note: The list only includes Bowlers who are ahead on the predicted scores of at least one Batsman. Hence, Suranga Lakmal and Dilruwan Perera are included. Other bowlers are not.

## "Good" day

If we consider a "good day", and sort accordingly, things get even better for Kusal Perera. On a "good day," our model seems to think that he's only second to Oshada Fernando and Dickwella.

![Image](https://cdn-images-1.medium.com/max/800/1*5cmzO7yxN2dADaxpAnB1eg.png)

## "Meh Day"

On a "meh" day, however, things get bad for Kusal Perera. He's at the bottom of the pack, even behind Dilruwan Perera and Suranga Lakmal.

![Image](https://cdn-images-1.medium.com/max/800/1*HJJxaypQpaoTwV4UdaNUZQ.png)

## Conclusion

As I said, I know very little about cricket. And even less about how test squads are picked.

But if I were to "justify" why Kusal Perera was left out, giving the selectors the benefit of my doubt, I'd reason something like this:

The selectors "played safe". Kusal Perera's "good" days are great. If he has an "average" day, he's only so so. And if he has a "meh" day, he's terrible.