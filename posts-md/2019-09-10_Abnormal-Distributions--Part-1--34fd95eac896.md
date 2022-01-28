#### Article 94 · September 10, 2019

# Abnormal Distributions (Prologue)

### The Normal Distribution

I wanted to write a series of articles about "abnormal distributions". By "abnormal distributions", I mean phenomena that do not follow normal distributions. But before describing "abnormal", I wanted to explain "normal". Hence, this prologue.

### The Normal Distribution

The Normal Distribution or the Gaussian Distribution dominates statistics. Its probability density function takes the form:

![Image](https://cdn-images-1.medium.com/max/800/1*2P-oV3FGuvCfpBu3pw65fA.png)

This distribution takes the visual form of a bell shape.

![Image](https://cdn-images-1.medium.com/max/800/1*Rz2c2o9FftTI6L2zDtO1dQ.png)

Many natural phenomena (e.g. the height of humans) approximately follow the normal distribution. There is good reason for this.

When a large number of independent random variables are summed together, the distribution of the normalised sum tends to follow a standard normal distribution (a normal distribution with mean,μ= 0and variance,σ²= 1). The (un-normalised) sum also takes a normal distribution.

For example, consider a coin toss. Suppose we represent the outcome with a random variable, x and tails with x = 0, and heads with x = 1. After 1,000,000 tosses the normalised sum of x will approximately follow a standard normal distribution. The (un-normalized) sum will roughly follow a normal distribution with μ= 500,000and σ² = 250,000.

The Central limit theorem(CLT) explains this phenomenon:

>>> "...the sum of a number of independent and identically distributed random variables with finite variances will tend to a normal distribution as the number of variables grows."

Humans are collections of cells which sum to form larger and larger emergent entities. The size of human cells can be (often) approximated as independent and identical distributions. Hence, their aggregates (e.g. Human Height) tend to follow Normal Distributions, as is true for many natural phenomena.

Pure and social scientists alike are quick to use the Normal Distribution as approximations for various real-valued random variables. They lean on the CLT for their justification. Sometimes the approximation is justified. But too often, the assumptions behind the CLT breakdown, leading to "abnormal" distributions.

Pretending that abnormal distributions are normal can be catastrophic.