#### Article 98 · September 13, 2019

# On Statistical Significance

### When is significant not significant?

>>> "Almost anything can be attacked as a loss of amenity, and almost anything can be defended as not a significant loss of amenity, which seems to signify that one should appreciate the significance of significant." — Sir Humphrey Appleby (Yes Minister)

## Heads or Tails ?

Let's suppose we have a coin. An ordinary coin with a heads side and a tails side. Now, suppose we toss it 10 times, and get the following results:

H H H H t H H H t H

8 heads, and 2 tails. Is the coin a fair coin? How might we answer this question?

## A Tale of Two Tests

One one hand, there are more heads than tails (8 > 2). On the other hand, a fair coin could have resulted in 8 heads (or even 9 or 10 heads, for that matter). So the vital question is: are there too many heads?

### Test A

Now, the probability of getting 7 or fewer heads by tossing a fair coin 10 times is ~94.6% (Alternatively, the probability of getting more than 7 heads with a fair coin is ~5.4%). Hence, our outcome of 8 heads is only found with a (relatively) small set of fair coins. A statistician could have said,

>>> "there is evidence to conclude that the coin is not fair at a 5.4% significance level (or 94.6% confidence level), because all but 5.4% of fair coins are expected to pass the 7 or fewer heads test".

### Test B

But similarly, the probability of getting 8 or fewer heads by tossing a fair coin 10 times is ~98.9% (Alternatively, the probability of getting more than 8 heads with a fair coin, is ~1.1%). Hence, if we got 9 or 10 heads, then we could say that it was very unlikely that the coin was fair. But since we got 8 heads, a statistician might have said,

>>> "there is no evidence to conclude that the coin is not fair at a 1.1% significance level (or 98.9% confidence level), since, like all but 1.1% of fair coins, this coin passes the 8 or fewer heads test".

What do we pick? Test A or Test B?

## True Nature

To know for certain if a coin is fair, we would need to analyse its physical nature. For example, if the coin is a perfect cylinder made of a uniform material, it will likely be fair. Since the specific dimensions of a perfect cylinder can vary, theorotically, there is an infinite variety of fair coins. Unfair coins, similarly, have some physical property that make them unfair. For example, they might be made of two different metals, of different densities.

Hence, if we knew the exact physical nature of the coin, we could have pronounced them fair — without experiment. However, if we don't have the ability to understand this nature, we might need to resort to experiments (like tossing the coin). The observations of these experiments, while functions of the underlying physical nature, don't completely reveal this nature.

Starting from this "True Nature" we could try and answer our "Is the coin fair" question from "first principles".

## First Principles and Roadblocks

We can break our problem, into several questions:

* What are all the possible physical natures the coin could take? Let's denote the various physical natures as N₁,N₂,N₃,...

* Is a coin with a particular physical form fair? Let's define function F such that F(Nᵢ) = 1 if a coin with physical nature Nᵢ is fair, 0 if it isn't.

* For each of these physical natures, what is the probability that we are observing such a coin? Let's denote the probability of observing a coin with physical nature Nᵢ with P(Nᵢ). We need to calculate, P(N₁),P(N₂),P(N₃),...

* For each of these physical natures, what is the probability of observing "H H H H t H H H t H" given that the coin tossed had that physical nature? Let's denote our observation ("H H H H t H H H t H") with O, and the probability of observing O given the coin tossed has physical nature Nᵢ with P(O|Nᵢ). We need to calculate, P(O|N₁), P(O|N₂), P(O|N₃)...

Now, using Bayes' Theorem the probability that a coin has a particular physical form Nᵢ given our observation O:

P(Nᵢ|O) = P(O|Nᵢ) . P(Nᵢ) / P(O).

The probability that a coin is a fair coin given our observation O is:

∑ F(Nᵢ). P(O|Nᵢ) . P(Nᵢ) / P(O).

Similarly, the probability that a coin is not a fair coin given our observation O is:

∑ (1-F(Nᵢ)). P(O|Nᵢ) . P(Nᵢ) / P(O).

Now, the coin is more likely to be fair if and only if,

∑ F(Nᵢ). P(O|Nᵢ) . P(Nᵢ) / P(O) > ∑ (1-F(Nᵢ)). P(O|Nᵢ) . P(Nᵢ) / P(O)

Or

∑ F(Nᵢ). P(O|Nᵢ) . P(Nᵢ) > ∑ (1-F(Nᵢ)). P(O|Nᵢ) . P(Nᵢ)

Unfortunately, the problem with this first principles approach is that we don't have an answer to two of the questions.

* Question 1: We don't have an exhaustive knowledge of all possible coins. Hence, we can't possibly enumerate N₁,N₂,N₃,... etc. exhaustively.

* Question 3: We don't know the probability P(Nᵢ) of a particular coin occurring

(On the other hand, Question 2 and Question 4 can be answered, through analysis and observation. Hence, F(Nᵢ) and P(O|Nᵢ) can be known, usually)

Hence, we meet a road block. Either we need to try and answer Question 1 and Question 3, or we need to make some assumptions.

## Back to the Real World

Let's revisit our two statistical conclusions:

>>> Test A: "there is evidence to conclude that the coin is not fair at a 5.4% significance level (or 94.6% confidence level), because all but 5.4% of fair coins are expected to pass the 7 or fewer heads test".

>>> Test B: "there is no evidence to conclude that the coin is not fair at a 1.1% significance level (or 98.9% confidence level), since, like all but 1.1% of fair coins, this coin passes the 8 or fewer heads test".

Both claims have something in common: we subject the coin to a test, which a fair coin is highly likely to pass, or highly unlikely to fail.

If a coin fails the test, and we pronounce it "not fair", there is a 5.4% chance that we are wrong in Test A, and a 1.1% chance that we are wrong in Test B. Hence, the only difference between the two "tests" is how wrong we are prepared to be if the coin fails the test.

If we denote "fair" as negative, and "unfair" as positive, we say (in statistical jargon) that Test A has a false positive rate (where the coin is actually negative, but we say it is positive) or a Type I error of 5.4%. Test B has a Type I error of 1.1%.

## Assymetrical Hypotheses

Similarly, if the the coin is actually positive ("unfair"), but we say it is negative ("fair"), we say there is a Type II error, or a false negative.

So what are the Type II errors of the tests? Or in other words, if we conclude that the coin is indeed fair, what is the chance that it might be unfair? But when will we actually say that the "coin is indeed fair"?

Now, if the coin failed the test, we had reasonable confidence that the coin was not fair, because most fair coins pass the test. But can we say the opposite? That, if a coin passed the test, we have reasonable confidence that the coin is fair, because most unfair coins fail the test? We can't say this because we don't know if most unfair coins pass the test. In fact, we know nothing about unfair coins. To know, we would need exhaustive answers to Question 1 and Question 3.

Instead, we deal with the problem of unknown Type II errors by making an assumption, and a very strong one at that: We assume that most coins are fair.

This leads to the following reasoning:

* Most coins are fair.

* Hence, it is unlikely that we will encounter unfair coins.

* Hence, it is even more unlikely that we will encounter unfair coins, and they will pass the test.

* Hence, Type II errors are unlikely.

* Hence, we don't care about Type II errors.

* Let's get back to doing real statistics, without wasting time philosophising...

## So is our coin fair or unfair?

I don't know. I can only say two things:

* Most fair coins pass Test A. Our coin failed Test A.Therefore, our coin is probably unfair. But there's a 5.4% chance that I'm wrong.

* Most fair coins pass Test B. Our coin passed Test B. Our coin is probably fair, because most coins are fair. But there's a chance that I'm wrong, because I know nothing about unfair coins, and if they pass Test B.

Maybe our coin is fair in some worlds, and unfair in other parallel worlds. I don't know. Perhaps, we will never know.

![Image](https://cdn-images-1.medium.com/max/800/1*JUqbxEphlNsDEum9YBYgnw.jpeg)