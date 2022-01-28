#### Article 341 · October 9, 2021

# How to separate Fraud from Genuine Data Analysis

### On P-Values, Cheating, Cost and What to do about these

Most Data Analyses are Fraud. Opinions disguised as Fact.

How do you tell the difference? Read on to find out.

## P-Values

Statistical analyses of experiments are usually accompanied by p-values (short for probability value).

What exactly is a p-value? Experiments have data and claims. The data is supposed to confirm or deny the claim. A p-value is the probability that the proposed claim is false, but the data supports the claim.

For example, if the p-value is 0.05, there is a 5% or 1 in 20 chance that the experiment's claim is false, but the data supports it — say, due to random noise.

There is no universal agreement on what makes a good p-value. Some pick 0.01, other pick 0.05, 0.1 or even 0.2. Intuitively, at least, it isn't easy to decide what value is right.

We might get around this problem by considering the possibility of "Cheating".

## Cheating

What if some unscrupulous experimenter wants to promote a claim (say) because a rich customer pays them to do so?

With a p-value of 0.2 or 1/5, if they repeat the experiment 5 times, they are likely to arrive at one set of experimental data, which supports the claim, even if it is false. Hence, our unscrupulous experimenter discards the data that doesn't support the claim, publishes the one set that supports it (also known as "cherry-picking"), and gets promptly rewarded by a grateful customer.

If the p-value of the experiment was lower, say 0.01 or 1/100, then the unscrupulous experimenter would have to repeat the experiment 100 times (not 5 times) to find "confirming" experimental data. Conversely, if the p-value were 0.5, just 2 experiments would suffice.

In other words, p-values indicate "cheatability" — or how easy it is to cheat. The higher the p-value, the easier it is to cheat.

## Cost

There is another factor that influences cheating, namely cost. If it is easier to repeat an experiment, it is easier to cheat. Hence, we should be particularly aware of experiments that are easy to repeat and have high p-values.

Most cases of "Cherry-Picking" are usually quite cheap to pull off.

## What to do?

How can we use these insights to make sure there is no cheating and that claims are reasonable?

* Step 1: Make sure there is a p-value. Any scientific experiment that attempts to verify a claim should have a p-value. Without such, the promotion of a claim is mere opinion, not science.

* Step 2: If the p-value is high, there should be evidence that either the cost of repeating the experiment is high, or it has been repeated and the data supports the claim in these repetitions.

* Step 2a: If the experiment is expensive, the experimenter should try to find a cheaper experiment or one with a lower p-value. If not, should be honest about the "low power" of the claim.

* Step 2b: If the experiment has been repeated, the results of these repetitions must be published.

* Step 3: In all low p-value cases, the experiment should be transparent about who supports their research and especially who may benefit from their claims. In other words, what their incentive to cheat is.

![Image](https://cdn-images-1.medium.com/max/800/1*fuR565U9_n_1oEqb4Bw7uw.jpeg)