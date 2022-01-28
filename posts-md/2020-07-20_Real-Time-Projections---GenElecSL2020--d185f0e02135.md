#### Article 253 · July 20, 2020

### 2020 Sri Lankan Parliamentary Election

# Real-Time Projections (#GenElecSL2020)

### "Predicting" the Election in Real-Time

With the hardships of CoViD19, many seem to have lost interest in #GenElecSL2020. It would be interesting to see if turnout exceeds the previous lows of 61.26% (in 2010) and 63.60% (1989). But as with many things with little data, and no precedent, predictions are almost impossible. Hence, I'm not going to attempt predicting turnout, nor the final result.

Instead, this article is like the Election Projections article I wrote around #PresPollSL2019. Where I ask the question:

"Can we use early results to project and predict the final result? And if so, how accurate would such a projection be?"

## The Experiment

To find out, I simulated #GenElecSL2015. As with my previous article,

* I assumed that election results report in order of result size. Starting with smaller results like postal votes. Ending with larger polling divisions like Homagama, Kaduwela, and Nuwara Eliya-Maskeliya.

* For each set of reported results, I built a regression model. That predicted the outcome based on these reported results. The model trained on the previous six general elections (between 1989 and 2010).

* I validated the results by computing error bounds.

However, the similarities end here. Presidential elections are simple. The "final result" is a "winning candidate". Selected based on who got the most votes islandwide. General elections are far more complicated. And our model needs to consider this.

## Complexities of General Elections

A presidential election is, effectively, one, islandwide election. A general election is a collection of many elections.

An "election" is held for each electoral district. Parties gaining at least 5% of the total district vote qualify for seats. A certain number of seats are pre-allocated to each district. These divide among the qualifying parties, proportional to their votes. Of the 225 seats in parliament, 196 are so allocated.

The remaining 29 for the "National List". These divided among parties, proportional to their total islandwide votes.

Hence, the "final result" of a general election is not a single winner, but an allocation of seats. Far more complex.

Every Sri Lankan presidential election has been a "two-horse race". Between candidates from the two main parties. Some might say, some have even been "one-horse races". No "third candidate" has won more than 4.63% of the popular vote.

Hence, predicting a presidential election is easy. Merely predict the votes each major party candidate would get.

General Elections are far more complicated. While the two major parties still get most of the seats, other parties also get significant numbers. Parties also field many candidates, who might not necessarily be permanently loyal to the party. As it is common for politicians to "jump". Multiple parties form complex coalitions, without precedent.

Hence, when it comes to predicting general elections, the "concept" of a "party" is of little value. The election profile of the same "party" in two elections could be very different.

## The Model

Our General Election projection model takes these complexities into account.

With presidential elections, we trained a model as follows. To predict how many votes a party would get in a yet-unreleased polling division. Based on the polling divisions released. Each party had is own model.

In contrast, with general elections, we can't assume "party" as a factor. Hence, our model party agnostic. Each party shares the same model. If "party" does have some significant effect, our model does not capture this.

## The Results for 2015

Let's look at the model's predictions at results in intervals of 40.

![Image](https://cdn-images-1.medium.com/max/800/1*_SWyVyM-9vYEnK65mLrJxA.png)

At 40, the projected result is very similar to the final result for the UNP and the UPFA. But the error bars are very wide.

![Image](https://cdn-images-1.medium.com/max/800/1*Fz_HMz7gm267k4Ef93jlwg.png)

At 80, the error bars narrow somewhat, but are still very wide.

![Image](https://cdn-images-1.medium.com/max/800/1*aza4DHbSIhD0HPc-GDzTcg.png)

At 120, the error bars narrow further, but not enough to call a winner.

![Image](https://cdn-images-1.medium.com/max/800/1*dtlP_xLCGXFw3QRkLb6f4Q.png)

The error narrowing continues into 160. But not winner call as yet.

And finally, the final result.

![Image](https://cdn-images-1.medium.com/max/800/1*qSk-6UI5doZHDvpTEWpoTw.png)

Here's a graph of the seat predictions for the UNP and UPFA, as each result came in. Low and high error bars in thiner line.

![Image](https://cdn-images-1.medium.com/max/800/1*fPUlA-LN2NWV5j0yul15aA.png)

## The Results for 2010

2010 was a far more "one-sided" general election. And many were asking the question if the UPFA would get a two-thirds majority. Many are asking the same question about the SLPP this time around.

Sadly, while it was clear, early that the UPFA would win a majority, the "two-thirds" question remained unanswered right up to the end.

![Image](https://cdn-images-1.medium.com/max/800/1*5mPAEHSM5hDuC1O1PJJIVg.png)

## Concluding Warnings

When training data is scarce and problems complex, prediction is, not only difficult but often inaccurate and weak. This was my constant warning in my presidential election articles.

General elections have about the same amount of data as presidential elections (counting only the Proportional Representation Era). However, as we noted, they are several orders of magnitude more complex.

Hence, I must sound my warning even louder.