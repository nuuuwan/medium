#### Article 309 · March 14, 2021

### CoViD-19 in Sri Lanka

# Is there Community Spread?

### The Letter, the Spirit and the Statistic

"Is there Community Spread of CoViD-19 in Sri Lanka?" is a question that gets asked from time to time. And nearly 14 months since Sri Lanka's first CoViD case, there still seems to be a lot of debate and disagreement.

Sadly, much of the discussion lacked one crucial component: a clear explanation of what "Community Spread" or "Community Transmission" means. Those who had some definition tended to be overly literal and seemed to miss the concept's spirit. Finally, attempts at quantifying or measuring Community Spread generally lacked in consistency or statistical rigour.

This article is my (possibly feeble) attempt to right these wrongs. As many of you know, I'm not a medical or epidemiological expert. Comments and corrections are welcome.

## The Letter

There are many definitions of CoViD-19 community spread or transmission, and they are all roughly the same across reputable sources.

For example, the WHO defines it as:

>>> "Community transmission is evidenced by the inability to relate confirmed cases through chains of transmission for a large number of cases, or by increasing positive tests through sentinel samples (routine systematic testing of respiratory samples from established laboratories)."

WebMD as:

>>> "Community transmission is when there is no clear source of origin of the infection in a new community."

Wikipedia as

>>> Community transmission means that the source of infection for the spread of an illness is unknown or a link in terms of contacts between patients and other people is missing. It refers to the difficulty in grasping the epidemiological link in the community beyond confirmed cases

## Problems of "Letteralism"

As with most definitions, an overly literal intepretation can be problematic. Let's investigate a few of these problems

### Problem 1: Trivialities

>>> Suppose a country has exactly one positive case. No one else has tested positive, nor do we know how the positive case got infected. If we apply the definition literally, this would be an example of community spread.

Most would agree that the CoViD situation in this country is "not too bad". But by (literal) definition, it has community spread, which, emotionally at least, feels a bad thing.

### Problem 2: Black or White

A literal interpretation also leaves no other option but to reach a binary conclusion. Either "there is community spread", or "there is no community spread". There is nothing in between or middle-ground.

### Problem 3: Interpretation of causality

What precisely does "inability to relate confirmed cases" or "clear source of origin" mean? How "related" is related? And how close is "close"?

>>> For example, person B tests positive a few days after person A, who happens to work in the same large factory as person B. Can we conclude that A and B are related? Or that A is the "clear source" of B's infection? What if we replace "large factory" with "small factory"? Or "small town"? Or "large town"? Or "country"?

There is no agreed-upon standard.

## The Spirit

To solve these problems of "letteralism", let's take a couple of steps back and consider the "spirit" of community spread.

Why do we care about Community Spread?

It is because we want our health authorities to have the situation under control. And a good signal on "control" is how well our authorities understand how people got infected. This knowledge is a good thing because then the infected folks can be quarantined or otherwise contained, slowing down the disease's spread.

What if we could reinterpret community spread as a statistic that would be a good indicator of control, and thus capture the spirit of the topic?

## The Statistic

Let's start by considering how we might avoid the problems of a literal definition.

How might we avoid a blunt "black and white" interpretation? An obvious path is to have a probabilistic or statistical interpretation of community spread. For example, something like: "Community Spread is the proportion of positive cases with no clear source of origin of the infection." This solves Problem 2.

Conveniently, a statistical interpretation also solves Problem 1. All trivial conclusions (like our one-case country above) would be excluded based on "statistical insignificance".

The actual measurement of this statistic could look something like this:

* Take a random sample of the population and test them.

* Of those who test positive, count the number of people with a clear source of origin.

* Find the proportion of cases with no clear source of origin

>>> For example, if 12,000 people are tested today (roughly the daily number of PCR tests in Sri Lanka, as of writing), and if 400 test positive, and 300 are known to have a clear source of origin, then the community spread rate is 25%.

## The Statistic: Cheat Proofed

But diligent readers would notice that we still have Problem 3, namely, some ambiguity around interpreting "clear source of origin". They might point out that health authorities could artificially decrease or increase the statistic by liberal or conservative interpretation.

How might we avoid this type of cheating? We could try something like this:

* Fix a "clear source of origin" beforehand by designating a set of people as probable origins (the "contact group").

* Then, take a random sample of people who might have come into contact with these designated people and test them. We can use this to estimate the number of positive cases in the contact group.

* Then, take a random sample of the entire population and test them. We can use this to estimate the number of positive cases in the population.

* Since we know the number of positive cases in the contact group, we can compute the number of positive cases outside it.

* The probabilistic community spread rate is the ratio of the number of positive cases outside the contact group to that in the whole population.

>>> For example, suppose there are 1,000 people designated as probable origins. Suppose 60,000 people might have come into contact with these people. We take a random 10% sample of the 60,000 (i.e. 6,000) and test them. Suppose 390 or 6.5% test positive. The complete contact group will have 3,900 positive cases.

>>> We also take a random sample of the entire population (say 6,000) and test them. Suppose 10 or 0.167% test positive. Assuming the population of the country is 22,000,000, the entire population will have 36,667 positive cases.

>>> Thus there are there are 36,667 minus 3,600 or 32,767 positive cases outside the contact group.

>>> Thus the probabilistic community spread rate is 32,767 / 36,667 or 89%.

## So, is there community spread?

If you ask the question, "Is there community spread?" you haven't understood this article. It implies that you still live in a "letteralist" black and white world.

The more meaningful question you should ask is "how much community spread is there?" to which a meaningful answer would be probabilistic, not "yes" or "no".

The good news is that our health authorities do a mix of testing: both random and probable contacts. And hence, it should be possible to calculate the statistic. The bad news is that they haven't published these separately. Hence, for now, my conclusion is "I don't know".

However, it should be relatively easy for the authorities to publish these numbers. And I hope they do.

## Problems Revisited

But we have more problems with Community Spread. Consider another imaginary example:

>>> Suppose in some unfortunate country, CoViD-19 has infected every single inhabitant. Many are dying; everyone is suffering. But suppose bizarrely (don't ask me how), this country has an excellent tracing system. Every single case connects to a source of origin. Hence, community spread (both literal and statistical) is zero.

This example highlights perhaps the biggest problem with the community spread metric. It is a relative metric that compares A) disease spread with B) tracking/tracing efficacy. If the spread is high, but tracking is also good, community spread will be low.

## Conclusions

What I (and probably most people) care about is disease spread. Measuring the effectiveness of tracking/tracing is also essential but strictly secondary.

The way to measure disease spread is simple. Take a random sample of the population and compute the positive rate.

>>> For example, if in a random sample of 10,000 people, 100 people test positive, then 100 / 10,000 or 1% is (for me) the most important metric.

If this significantly increases, then there is a problem. If it decreases, things are improving.

Like my proposed probabilistic community spread statistic, the good news is that all the data required to compute this figure already exists. The bad news is that, as far as I know, it is not published. A publication and analysis of this metric will give us the real picture of CoViD-19 in Sri Lanka.

![Image](https://cdn-images-1.medium.com/max/800/1*O-3mO6klhrWn3DLZ0O9EQw.jpeg)