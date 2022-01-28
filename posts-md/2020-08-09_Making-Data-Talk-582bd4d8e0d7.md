#### Article 258 · August 9, 2020

### Data Science 101

# Making Data Talk

### 9 Dos and Don'ts Data Analysis

This article is based on a talk I delivered at Verite Research, a few weeks before the 2019 Sri Lankan Presidential Election.

...

Data Analysis is an interrogation. The data analyst is the interrogator, and the data is the interrogated.

![Image](https://cdn-images-1.medium.com/max/800/1*KJJtjCQTiXnpwmzbALu3CA.png)

The interrogator has a bunch of tools. Some legal. Some illegal. Some ethical. Some not so ethical.

This article is about using those tools. Effectively. And ethically.

## 1. Do ask Questions

![Image](https://cdn-images-1.medium.com/max/800/1*L8-WmEKH2hJ6hMxbRXV1Ng.png)

There is no point in interrogating someone, if you have no questions to ask. If you're silent, the data will be silent.

So you have to have questions. Good questions. Interesting questions.

...

I started one of my articles by asking the question, "How many voters are floating voters?" [A floating voter is a voter who is not bound to a certain party. At an election, they could vote for any party.]

At the beginning, I didn't know how to answer this question. But even if you can't answer your question, you might be able to answer a different question.

So while I didn't know "How many voters were floating voters", I did find a way of estimating "How many voters were base voters". [A base voter is the opposite of a floating voter. Voters who always vote for the same party.]

This Dorling Cartogram represents voters who'll always vote UNP. And how they are distributed across polling divisions. The size of the circle is proportional to the number of base voters.

![Image](https://cdn-images-1.medium.com/max/800/1*6xUO_fjw36v5jXFrc1-pOA.png)

In Sinhala we have a colorful phrase "කැපුවත් කොළ" ("Kepuvat Kola"). Voters who support the UNP so much their blood is green. This is the data analytics representation of කැපුවත් කොළ.

...

Once you have an intermediate answer, you can apply some theory to get the answer you want.

I figured that the number of floating voters is what you get when you subtract all base voters from all the voters.

And so, we get an approximate answer to our question, "How many voters are floating voters?"

![Image](https://cdn-images-1.medium.com/max/800/1*TnuCgOjKcaLLLu40SlMLsQ.png)

...

If you have an interesting question, you can (usually) find an interesting way to find an answer. The important thing is to ask questions.

## 2. Do Reflect on Data

![Image](https://cdn-images-1.medium.com/max/800/1*WfG5tPoitqXxFd6_39iABg.png)

When there is an interrogation in movies, there's always a "mirror scene". Where the police watch the prisoner through a one-way mirror.

And usually the police see some interesting things. Because the prisoner can't see them. And instead sees themselves. And tend to do interesting things.

Can we do the same mirror trick with data? Can we put data into a room and watch it? From behind a one-way mirror?

The answer is, we can.

And the way to make data "reflect", is to see what new conclusions it implies.

...

For example, we can take our floating voter data, and see how it reflects on the 2015 election.

![Image](https://cdn-images-1.medium.com/max/800/1*yaMjBnhSqDngSzniu07EFw.png)

This cartogram represents how the two main political parties performed among floating voters. And as expected, we see that the NDF dominated the floating vote.

...

We get an even more interesting reflection from 2005. Again the NDF dominates the floating vote, but not enough to win the election.

![Image](https://cdn-images-1.medium.com/max/800/1*37erqn3KwVmyfxWC-1DqVQ.png)

Many people talk about the LTTE boycott in the North, and how it affected the final result. But a less talked about point is how the NDF failed to win the floating vote in places like Colombo, Galle, Matara and Gampaha.

All those white circles represent floating voters, who didn't vote NDF, or just stayed home.

## 3. Do understand that Data is stranger

Too often, we think we understand the data. When in fact we don't. Sometimes data is strange. Or even. Stranger.

![Image](https://cdn-images-1.medium.com/max/800/1*pS93JWvcFIS2R1Bk2i7fwQ.png)

...

This is a map of the 50 United States of America and the District of Columbia. And a map of another presidential election.

![Image](https://cdn-images-1.medium.com/max/800/1*i5j3epTWaQhnn0i000x-4A.png)

The Blue states always vote for the Democrat Presidential candidate. The Red vote Republican. The other states are swing states. They vote for one candidate or the other.

The purple states are an interesting type of swing state. Known as Bellwether states. They not only swing, but they tend to swing in the right direction. They almost always vote for the candidate that wins the election.

In any data analysis, it is essential to realize that not all data is the same. For example, not all Polling Divisions are the same. Some might be Bellwether polling divisions.

...

I tried to answer this question and came up with this map. The eight purple polling divisions always voted for the winning presidential candidate.

![Image](https://cdn-images-1.medium.com/max/800/1*_D_-3hqykx-oAu3MnioS_w.png)

...

There are other ways in which data is also different. For example, Turnout can be very different across polling divisions. And this could be significant for elections.

![Image](https://cdn-images-1.medium.com/max/800/1*xql6TeVInFUNa_NRMiGkgw.png)

## 4. Don't let the data get the better of you

After I shared maps of floating voters and bellwether polling divisions, many people concluded that campaigns should focus on either the bellwether areas. Or the areas with the highest density of floating voters.

This shows some fallacies in thinking.

Bellwethers are bellwethers not because they influence the national results in some way. It's because their voter distributions happen to match the national distribution. The relationship is a correlation, not causation. So if a campaign targets a voter in Mawathagama , you might end up getting more votes in Mawathagama. But that won't "cause" you to get more votes Islandwide.

...

The problem with focussing on areas dense with floating voters is that causes you to lose out on other floating voters. The reality is that floating votes are everywhere. And concentrating on just some areas might win you polling divisions. But loose you the election.

...

In this controversial scene from Basic Instincts, Catherine Tramell not only taunts and intimidates her interregators, she ends up sending them in a completely wrong direction.

![Image](https://cdn-images-1.medium.com/max/800/1*v9awDlk5rIdW-RrNChnwWg.png)

Don't let the data get the better of you.

## 5. Don't torture data

I disappointed many by not predicting the result of next month's election. To exasperate these people, even more, I wanted to prove that it was hard to predict the outcome even after the results have been partially released.

To do this, I built a projection model. Which tries to predict the final result of the election using both previous election results. And the released results in the current election.

This graph shows the projected results for the 2015 election. The X-axis represents polling divisions as their results are released. The Y-axis represents the projected votes for each party. The red line is NDF. The blue line is UPFA.

![Image](https://cdn-images-1.medium.com/max/800/1*9cE-x3UPK8XVKMXUND0Eow.png)

Now, if you go by this projection, you'd assume that one party or the other is going to win the election. For most of this graph, it looks like red is going to win (as it did). But for some parts it might look like Blue is going to win.

But this is a wrong conclusion.

...

There are two types of interrogations. In one type, the interrogator wants to learn the truth. In the other type, the interrogator wants to force a confession.

![Image](https://cdn-images-1.medium.com/max/800/1*fnPX7YESx5M498Nm8ggUtw.png)

The problem with data is that with minimal torture, you can get it to say anything you want. So, if you want to learn the truth, the interrogation has to be sensitive and intelligent.

Sadly most data analyses fall into the forced confession category. The analyst has some specific outcome in mind, and they torture the data to call this outcome.

...

Let's look at my projection again. In this second diagram, you see the real state of the data. You see not one red line and one blue line. But three read lines and three blue lines.

![Image](https://cdn-images-1.medium.com/max/800/1*eL2XXrm9XwEFRUvEYWN7EQ.png)

Let's zoom in for more detail.