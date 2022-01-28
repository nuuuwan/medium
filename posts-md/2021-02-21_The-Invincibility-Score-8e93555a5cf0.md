#### Article 304 · February 21, 2021

# The Invincibility Score

### A more meaningful alternative to Cricket Ratings, and a Brief History of Men's ODI Cricket

## Part I: A more meaningful alternative to Cricket Ratings

Do you know which country is currently ranked highest in the ICC's Men's ODI Team Rankings? The answer is England. Not surprising, since England are the reigning World Cup Champions and have had a decent run of matches lately.

But do you know what England's "rating" is? England has a rating of 123. India is second with 117; Sri Lanka, down in 8th place with 85.

![Image](https://cdn-images-1.medium.com/max/800/1*FDTqbk2idwxo79PNR0KrQQ.png)

### What do these ratings mean?

If you want to learn the exact details and calculations, you can read this excellent Wikipedia article.

But for those of you who are lazy, here's the "intuitive" summary:

* You get more points for winning games; fewer for loosing.

* You get more points for playing against stronger teams (i.e. teams with more points); fewer for playing weaker ones.

* Points are weighted by time. More recent matches count for more points.

* The rating is the average points you win per match.

### But what do these ratings actually mean?

By "actually mean", I mean, does the rating's numerical value have any real-world meaning? The way, say, batting averages, have? For example, Virat Kohli has an ODI batting average of 59.31, meaning that he scores about 59.31 runs on average for each time he's out.

So similarly, what can we say about India's 117 rating?

The ICC website has nothing about interpreting Team Ratings, but it's Player's Rankings FAQ has the following answer to the question, "What does it mean to have, say, 500 points?":

>>> Rating points have a meaning in the same way as traditional averages do. Over 900 points is a supreme achievement. Few players get there, and even fewer stay there for long. 750 plus is normally enough to put a player in the world top ten. 500 plus is a good, solid rating.

They don't say why 900 is a supreme achievement or why 500 plus is good. You must take these things at the ICC's word. The said Mr Kohli has an ODI rating of 870; 30 short of supreme — whatever that means. Sorry Mr Kohli.

### Ratings that actually mean something

What if we had a rating system where the numerical rating actually meant something in the real world? Like a batting average?

So, I thought of designing such a system.

### The simplest possible world

Let's start with the simplest scenario: Suppose the cricket playing world had only two ODI playing countries: Say Sri Lanka and Australia.

If we had a rating system in such a world, what would we want the rating to say? What is the most important and interesting way of comparing the two teams?

For me, I'd like to know the following: If Sri Lanka and Australia were to play an ODI tomorrow, who would win? In other words, I'd like to know the odds of one or the other team winning. For example, Sri Lanka could have a 41% chance of winning, and Australia a 59% chance.

We could directly use these probabilities as ratings: Australia 59%, Sri Lanka 41%. Not only does the better team have a higher rating, but the rating also has a "real-world meaning", namely, the chance of the team winning.

### The Real World

Now, can we extend this simple idea to the real world? Where there are multiple teams? All of which play each other?

We could extend the simplistic, two-team definition to multiple teams. Just as we defined the rating to mean "the probability of the team beating the other team" (in the simplistic world), we could define the rating to mean "the probability of the team beating all the other teams". Any team that could beat all the other teams would, by definition, be invincible.

Hence, our rating would be "the probability of invincibility" or an "Invincibility Score" more flamboyantly.

These statistics can be computed using historical match records.

### Comparing the Invincibility Score to ICC's Men's ODI Team Rankings

Here are the current (i.e. February 14, 2021) Invincibility Scores for ODI Teams:

![Image](https://cdn-images-1.medium.com/max/800/1*DmWT94vHlvLX-JEQxk8bsQ.png)

Invincibility Scores are very similar to the ICC Rankings, the differences being 1) Australia and New Zealand, and 2) Sri Lanka and Bangladesh are switched.

Hence, not only are the Invincibility Scores consistent with the ICC Rankings, they also have a real-world meaning. They tell us that England has about 3% odds of beating all the other teams; while West Indies and Afgahistan have almost no chance in hell.

### Downsides

The Invincibility Score, despite its advantages, as some disadvantages also:

* You might not be a fan of fractions for a rating. You might also not be a fan of teams having zero as a rating. However, its easy to get around this problem by scaling. Instead of % values, we could do a "one-in-1000,000", say.

* It's not trivial to predict what a team's Invincibility Score will be after a single result. This is because the score depends on the results of all other teams, and also time itself. Then again, the ICC's own ratings suffer from this problem.

## Part II: A Brief History of Men's ODI Cricket

If we plot the Invincibility Score, across the history of ODI cricket (which happens to be almost exactly 50 years), we get the following graph.

![Image](https://cdn-images-1.medium.com/max/800/1*TRmcblVnlqNLFQlXDv9zwg.png)

A couple of observations strikeout.

### The West Indies Dominate the 1970s

Perhaps, the most dominant observation is how the West Indies dominated the 1970s and 1980s. For 4+ years between June 1975 and December 1979, the West Indies maintain the top spot. They also maintain an Invincibility Score of around 20% or so consistently, peaking at about 45%.

This level has never been repeated in ODI history, highlighting the dominance of Caribbean Cricket. Not surprisingly, this period included the Windie's two World Cup wins in 1975 and 1979.

### And also the 1980s

Despite losing the 1983 World Cup to India, the West Indies register another streak at the top of over 5 years from June 1983 to October 1988.

![Image](https://cdn-images-1.medium.com/max/800/1*WhOc4k0rPQUgzztUyxuhqQ.png)

[* Other countries have been shaded for easier reading]

England and New Zealand also hold the top spot for brief periods in the 1980s.

### The 1990s: A Mixed Decade

After the somewhat one-sided 1980s, the 1990s is very much a mixed decade. Following their win in the 1989 World Cup, Australia dominates the first couple of years, including a 64-week streak at the top from December 1990 to March 1992.

![Image](https://cdn-images-1.medium.com/max/800/1*p43t_mubvyMecv3ER8dMcw.png)

[** Other countries have been shaded, and the Y-Axis expanded for easier reading.]

Pakistan takes the top spot in March 1992 after winning the World Cup but are replaced after just one week by runners-up England, who maintain the top spot for only over one year until March 1993. England is followed by New Zealand with 39 weeks at the top, until December 1993.

![Image](https://cdn-images-1.medium.com/max/800/1*id_XrYw9x_-crX3zdL6MLA.png)

Australia retakes top spot for 64 weeks from December 1993 to March 1995. Former Invincibles West Indies return to the top for 31 weeks until October 1995. Then, Pakistan takes the top spot for another 9 weeks, and Australia retakes the top spot and maintains it for 44 weeks until October 1996 — a few months after their World Cup final loss to Sri Lanka in March.

Just as Australia rose after their 1989 World Cup win, Sri Lanka took the top spot from Australia in October 1996, which they maintain for just over one year, until October 1997.

![Image](https://cdn-images-1.medium.com/max/800/1*oo23cpA9T86jSidiR03NgA.png)

South Africa dominate the final two years of the 1990s, with over two years at the top from November 1997 to March 2000. This period includes the 1999 Word Cup, where Australia famously choked South Africa in the tied semi-final.

![Image](https://cdn-images-1.medium.com/max/800/1*9Ka-wrucYyFI2gJzd1mWjw.png)

### Australia in the 2000s

If the Windies dominated the 1970s and 1980s, Australia would dominate the 2000s. While not matching the Windies' Invincibility Score, they record the most prolonged continuous period at the top, for almost 8 years from December 2002 to November 2010. This period also included World Cup wins in 2003 and 2009.

South Africa briefly take the top spot a few times in the early 2000s.

### The 2010s: The Second Mixed Decade

The 2010s until September 2011 is a mixed bag. Australia spends the most amount of time, in addition to India and Sri Lanka — the two teams that met in the 2011 World Cup final (in April), the latter winning.

![Image](https://cdn-images-1.medium.com/max/800/1*lDX2ZdiHWMfEmGuaTLvFyg.png)

After the World Cup, Australia records a 2+ year streak at the top, from September 2011 to November 2013. Australia also dominates the next year or so, with India and South Africa taking the top spot for brief periods.

Australia records another 2+ year streak, taking the top spot from September 2014 to October 2017, including Australia's 5th World Cup win in 2015.

September 2017 to June 2019 is a back and both battle between India and England, the former dominating the start of that period.

Since July 2019, following their win in the 2019 World Cup, England have maintained the top spot for 86 weeks and counting.

![Image](https://cdn-images-1.medium.com/max/800/1*pihLpgzydpR4Ol2uTV3mmg.png)