#### Article 300 · January 12, 2021

### Machine Learning for Business

# How do you evaluate your Machine Learning Model?

### Good answers and bad answers

Suppose you use Machine Learning to solve some business problem in your organization. For example, you might run an e-commerce website, where you sell groceries; where customers log in, browse your stock, checkout what they want, pay for it, and then have the goods delivered to them. You (or one of your colleagues) might have built a machine learning model that "recommends" items for your customers, on the home-page of your website.

![Image](https://cdn-images-1.medium.com/max/800/1*WpwCuPLzdbbPlaRK5CXf7g.png)

Now, suppose I asked you,

>>> "How do you evaluate your Machine Learning Model?"

I.e. How do you know if it's good or bad? And if it can be improved? And if other people have better models? I ask this question often, and different people give very different answers: some good, many not so good.

This article is a "classification" of possible answers to the question "How do you evaluate your Machine Learning Model?": From really bad answers to very good ones. Read on to find out if yours is good or bad.

## ML0 — "I don't."

Sadly, the most common answer to "How do you evaluate your Machine Learning Model?" is:

>>> "I don't"

Few people know how well their Machine Learning Models work. Not everyone is this honest, though. Many people (especially on the "business side") say something elaborate, throwing in jargon, and buzzwords, and references to "technology". They might say something meaningless like:

>>> "We use the cutting edge HardMacro Turquoise AI Stack, and have a best-in-class e-commerce recommendation paradigm".

But it's fairly easy to see through the "BS", and that in reality, they have no idea.

This "ML0" is the lowest level in my classification, and if you think you fall into this group, I have two pieces of good news:

* Most organizations fall into this group. They've invested significant resources into Machine Learning or Data Analytics, but have no idea of the exact benefit it brings.

* This article explains how you can move up from "ML0" and improve your organization uses Machine Learning.

## ML1 — "Using Anecdotes"

Slightly better than having no idea is to have some idea. Many people have an anecdotal sense of their Machine Learning Systems; based on qualitative feedback from more knowledgeable colleagues or customers, like:

>>> "Our Chief Data Scientists said that the new model is much better than the old one"

Or a customer might say

>>> "Oh yes. I use the recommendations on your website all the time. It's very useful".

## ML2 — "Using Technical Metrics"

You might argue that it is "business people" who are guilty of ML0 and ML1. If you are a "technical person" (say a Machine Learning Engineer), you use all manner of fancy quantitative metrics to describe your ML.

For example, you might say that your e-commerce recommendation has:

>>> "A False Positive Rate (FPR) of only 60%"

In laymen's terms this usually means "The probability of a recommended item not being purchased by a customer". Similarly, "False Negative Rate (FNR)" means "the probability of not recommending a product that will be purchased by a customer".

On the one hand, having metrics like FPRs and FNRs (ML2) is better than having no idea on how the ML is doing (ML0), or only having a "qualitative" sense (ML1). On the other hand, it has at least three drawbacks:

* "Technical Metrics" like FPRs and FNRs (and more elaborate metrics like ROC curves etc.), have no clear "real-world" meaning. What would an FPR and FNR of 60% and 27.5% mean to the CEO? Would it be better than 70% and 15%?

* A comparison of Technical Metrics might not translate into Business Metrics. A model that is better than another model based on technical metrics is not necessarily better than the other model on business metrics.

* "Technical Metrics" isolate technical problems and people from the "bigger picture". For example, your e-commerce recommendation system could also be improved by better design, better photos, and different colours. These changes are not reflected in metrics like ROC, and hence cannot be compared to technical changes like ML improvements.

Organizations with ML teams that solely rely on Technical Metrics tend to isolate from the broader group working on the problem. "We care about what we measure" or more accurately "We don't care about what we don't measure."

## ML3 — "Using Business Metrics"

In the best ML organizations, even the most technical ML teams, measure themselves on Business Metrics, not Technical Metrics. For example, when I used to work on Ads Optimization at Facebook, we measured Models that recommend advertisements with metrics such as Revenue, Advertiser Profit, and User Feedback. No one ever mentioned FPRs or ROCs. These might be used operationally, (e.g. to "debug" faulty models), but never as a measure of model performance or quality.

Whenever a report or presentation on ML models, gives Technical Metrics priority over Business Metrics (ML2), it usually means one or both of the following:

* The technical team is unaware or unfamiliar with the actual business problem they are trying to solve.

* The technical team is trying to misguide or impress the audience by throwing technical metrics and other jargon.

## ML4 — "Using Business Metrics, across the Pipeline"

The best organizations not only use Business Metrics to evaluate ML Models and ML Teams but also use business metrics "operationally", at a "low level", say, when optimizing, tuning, and comparing different models.

For example, suppose you have several models for your e-commerce recommendation system: one is based on logistic regression, another based on boosting, another based on deep neural networks. You could either compare these models on "Technical Metrics" (like FPRs and ROCs) or you could try and compare these using Business Metrics, like Sales or Revenue. The Business Metrics would give you a more robust and accurate measure of which model is better.

## ML5 — "Using Multiple Business Metrics, across the Pipeline"

Most non-trivial, real-world problems cannot be measured or evaluated using a single metric (ML4).

For example, an e-commerce recommendation system, Revenue or Sales alone might not be sufficient. We might want to also look at measures like "Long term value of Customer", "Time to complete Checkout", and "Customer Feedback". If recommendations are for cheap, but low-quality products, we might see a short-term improvement in revenue, but a decline in long-term value.

Hence, we should evaluate ML Models (and all other parts of the system) on all the business metrics that the organization cares about, not just one. In practice, this might involve some tricky comparisons of "apples and oranges". But this is where humans judgement must take charge. The best Machine Learning systems are aides for smart humans, not replacements for dumb ones.

![Image](https://cdn-images-1.medium.com/max/800/1*W3yTIq2SJn9SfQxfxoeHJQ.png)