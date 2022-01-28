#### Article 180 · December 2, 2019

### 2019 Sri Lankan Presidential Election

# The Minority Report

Many have described the recent Sri Lankan Presidential Election as ethnically polarised. Some have even simplified the results to "The majority voted for Gota. Minorities voted for Sajith".

How accurate is this claim of polarisation?

In this article, I attempt a data-driven answer to this question.

## Non-Approach: A perfect answer

Suppose each ballot paper included the voter's ethnicity. Then we would be able to accurately answer all manner of questions around voting and ethnicity. And not just ethnicity. More data about age, gender, religion, and income would also yield interesting insights.

Sadly, (and perhaps happily), this is not the case. Voting is by secret ballot and includes no meta-data about the voter's profile. Hence, we need to resort to approximate estimates.

## Approach 1: A sure, but weak answer

### An imaginary polling division

Suppose an imaginary polling division has 100,000 voters: 80,000 Tamil and 20,000 Sinhala. Suppose the NDF won 80,000 votes, and the SLPP won 20,000 votes. What can we conclude?

On the one hand, we could assume that all the Tamil voters voted for the NDF, while all the Sinhala voters voted SLPP. This would be consistent with the data.

But this is not the only conclusion consistent with the data. For example, all 20,000 Sinhala voters could have voted for the NDF, with the SLPP getting all its votes from Tamil Voters. This might be inconsistent with the intuitions (and prejudices) of many. But it is still consistent with the data.

So what can we conclude? For sure?

We can conclude that the NDF won at least 60,000 Tamil Votes. Why? Because the most number of Non-Tamil votes it could have got was 20,000. We can also trivially conclude that the NDF won at most 80,000 Tamil Votes.

Hence, our conclusions are: The NDF won 60,000 to 80,000 (75% to 100%) Tamil votes, and 0 to 20,000 (0 to 100%) Sinhala votes.

![Image](https://cdn-images-1.medium.com/max/800/1*RpyhI1rGL_FzXc_PcDfIhA.png)

### Sri Lanka

If we extend this logic to the 2019 Sri Lankan Presidential Election, and the 160 polling divisions, we get the following numbers:

* Moor votes for NDF: 21% to 99%

* Tamil votes for NDF: 43% to 95%

* Sinhala votes for NDF: 27% to 43%

* Moor + Tamil votes for NDF: 41% to 93%

![Image](https://cdn-images-1.medium.com/max/800/1*3HpmjNuIhwRCY9lAyKBT6g.png)

Similarly,

* Moor votes for SLPP: 1% to 74%

* Tamil votes for SLPP: 2% to 51%

* Sinhala votes for SLPP: 51% to 67%

* Moor + Tamil votes for SLPP: 4% to 54%

![Image](https://cdn-images-1.medium.com/max/800/1*icWVOLJNx6WTkwh9_7lMCA.png)

[Note, "Tamil" includes both "Sri Lankan Tamil" and "Indian Tamil". "Moor" includes "Malay" and "Moor". Ethnicities <1% of the total population have been excluded]

## Approach 2: A less-sure, but the more-powerful answer

The above estimate is "sure" because we make no assumptions. On the other hand, it is "weak" because it predicts a wide range. Saying "Moor votes for SLPP: 1% to 74%" while true, is not very useful.

Can we reduce the range of the estimate? Could we make the estimate more powerful?

To gain power, we need to sacrifice "sure-ness". In other words, we need to make some assumptions.

### "Sri Lankan's vote along ethnic lines"

A blunt, but common assumption is that "Sri Lankan's vote along ethnic lines". For example, "X% of Sinhala Voters vote SLPP nation-wide" or "Y% of Tamil Voters vote NDF nation-wide". If we assume that this is true for all polling divisions, we can build a model that estimates X and Y.

```
NDF  = Moor * 86% + Tamil * 83% + Sinhala * 27%   ± 3%
```

Simple Linear Regression models which predict the SLPP vote share, and NDF vote share based on the proportions of ethnicities, take the following forms:

```
SLPP = Moor * 13% + Tamil * 8% + Sinhala * 65%   ± 3%
```

```
NDF  = Moor * 86% + Tamil * 83% + Sinhala * 27%   ± 3%
```

What does the "model think" about how ethnicities vote? The clue is in the model equation.

"SLPP = Moor * 13% + Tamil * 8% + Sinhala * 65%" implies that the "model thought" 13%, 8% and 65% Moor, Tamil and Sinhala voters respectively vote SLPP. Similarly, 86%, 83% and 27% voted NDF.

The ± 3% indicates to what degree the model is sure (or "unsure").

To evaluate the model, we merely plug-in the proportions of ethnicities.

### Sinhala Majority

For example, consider an Beliatta, which is almost 100% Sinhala. The model predicts:

```
SLPP = 0% * 13% + 0% *  8% + 100% * 65% = 65% ± 3%
```

```
NDF  = 0% * 86% + 0% * 83% + 100% * 27%= 27% ± 3%
```

![Image](https://cdn-images-1.medium.com/max/800/1*7MoX0LHp_xLxEQAdarCpFg.png)

This is quite close to the actual result.

### Tamil Majority

Udupiddy is almost 100% Tamil.

```
SLPP = 0% * 13% + 100% * 8% + 0% * 65% = 8% ± 3%
```

```
NDF  = 0% * 86% + 100% * 83% + 0% * 27%= 83% ± 3%
```

![Image](https://cdn-images-1.medium.com/max/800/1*fioaQUXztjQ5bcPj-laPjw.png)

Again, quite close.

### Moor Majority

Sammanthurai has the highest proportion of Moors, with 83% Moor, 15% Tamil, and 1% Sinhala.

```
SLPP = 83% * 13% + 15% * 8% +  1% * 65% = 11% ± 3%
```

```
NDF  = 83% * 86% + 15% * 83% + 1% * 27%= 86% ± 3%
```

![Image](https://cdn-images-1.medium.com/max/800/1*RFuSC8hxWsz-KGVYoANRUQ.png)

### Multi-Ethnic

Pottuvil is Sri Lanka's most "multi-ethnic" polling division. With 38% Moor, 32% Tamil and 29% Sinhala.

```
SLPP = 38% * 13% + 32% *  8% + 29% * 65% = 26% ± 3%
```

```
NDF  = 38% * 86% + 32% * 83% + 29% * 27%= 69% ± 3%
```

![Image](https://cdn-images-1.medium.com/max/800/1*ZHxQ-CVvb32tfozuMC1LpA.png)

Less accurate, but directionally correct.

### Sri Lanka

Using the proportions of ethnicities, and the number of votes in each polling division, we can estimate the number of voters by ethnicity. We get 9% Moor, 14% Tamil and 76% Sinhala. If we plug these into the model we get,

```
SLPP = 9% * 13% + 14% *  8% + 76% * 65% = 51% ± 3
```

```
NDF  = 9% * 86% + 14% * 83% + 76% * 27%= 42% ± 3%
```

![Image](https://cdn-images-1.medium.com/max/800/1*2J-GhH_T8xu-AS5B1MB-eA.png)

## A Journey Through History

If we were to build models for all 8 presidential elections, and plot "what the model thought", we get the following:

![Image](https://cdn-images-1.medium.com/max/800/1*cGIvewP1twlbNu75YKFE9g.png)

Excluding the 1994 anomaly, minority support for the "Blue" parties has waned. Conversely, the "Greens" have had to rely more and more on minorities.

![Image](https://cdn-images-1.medium.com/max/800/1*btoFF3bs5LqldAru5zIHcQ.png)

## Concluding Warnings

While "Sri Lankan's vote along ethnic lines" might be accurate, it can't be generalised. I know many Moors and Tamils who voted for the SLPP, and Sinhalese who voted for the NDF.

This is also clear from the polling divisions where our "Approach 2: Model" had the highest error.

![Image](https://cdn-images-1.medium.com/max/800/1*kp2BB07qXfo68k47AnpKvg.png)

There are two types of error: Minorities who voted for the SLPP (Kayts, Pottuvil, Nuwara Eliya-Maskeliya, Kalkudah), and the majority who voted for the NDF ( Hewaheta, Mahiyanganaya, Polonnaruwa, Medirigiriya, Ratnapura and Hakmana).

Both models and humans might assume that the Sri Lankan voter is a simple soul. Who votes by ethnicity and nothing else.

The reality is far more complicated.