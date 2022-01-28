# Book 5

#### Articles 201 to 250

#### Article 201 · January 2, 2020

# Z-Scores

### An Idiot's Guide to Z-Scores

These days, there is some controversy around the Z-Score system for university entry. Because, the new cabinet plans to replace this "Old-System" with a "New-System". Which is supposed to be "school-based" and "scientific" (whatever that means).

The goal of this article is not to compare and contrast these old and new systems. To compare, one must understand first.

I've been alarmed and shocked by how so many seem to misunderstand the Z-Score system. Few journalists attempt to explain it. And are happy to represent it as some mysterious enigma. With powers of life and death. Others are happy to quote soundbites from "experts".

>>> "Prof. Superfluous says, Z-Scores have a high carbon footprint. We hope to phase-out Z-Scores by 2025".

>>> "According to Dr. Gratuitous, Z-Scores cause pimples. But Salu Sala is well-stocked with preventive medication" [probably meant "Osu Sala"].

>>> "Elton (aged 23) from Kandana complains that Z-Scores are homophobic".

Ad nauseam.

Hence, in this article, I attempt to clear a bit of this mystery. By explaining Z-Scores.

[I hope to make a comparison of the "Old-System" to the "New-System" in a future article. But let's first try and understand the "Old-System" first]

## The Old-Old System

Consider Alice. At the A. Level exam, she gets:

```
Chemistry80
```

```
Maths70
```

```
Physics 70
```

Before we adopted Z-Scores (let's call that the Old-Old-System), raw aggregate marks determined university entry.

For example, Alice's aggregate is 80 + 70 + 70 = 220. She would have gained entry into any university program, where A) Chemistry, Maths and Physics were sufficient subjects, and B) 220 was a sufficient aggregate.

In this Old-Old-System, any mark from any subject is equal. For example, if Alice got 20 fewer marks for Maths (50) and 20 extra marks for Physics (90), she would have still had the same aggregate of 220. And more importantly, the same chances of university admission.

## The Old-System

But is the assumption "any mark from any subject is equal" reasonable? After all, aren't some subjects "easier" than others? If so, students doing well in "difficult" subjects (which have lower marks) are disadvantaged. Compared to "easier" subjects (which have higher marks).

To analyse this assumption, let's consider the marks of all the students who took Chemistry, Maths and Physics. While in practice there are 100,000s of students, for simplicity, let's assume there were only five. Including Alice.

And let's suppose the marks were as follows, with Alice's marks in bold.

```
Chemistry50, 60, 70, 80, 90
```

```
Maths30, 40, 50, 60, 70
```

```
Physics10, 30, 50, 70, 90
```

What can we observe?

* It looks like this year's Maths paper is a lot more "difficult" than the Chemistry paper. And Alice's 70 for Maths, is the top mark. Even though it is 10 marks less than her 80 for Chemistry.

* Similarly, her 70 for Maths looks better than the same 70 for Physics.

* While both Physics and Maths have the same "average" mark (50), the marks for Physics seem to have more "variation". While the marks for Maths are more "closely clustered". Hence, if Alice was to get 20 marks fewer for Maths, and 20 marks more for Physics, she would have had to do "more worse" for Maths than "more better" for Physics. Because the same 20 marks jump from 70 to 50 for Maths would seem to have more significance than the same jump from 70 to 90 for Physics.

Why are these observations significant?

* Alice's 70 for maths should carry "more weight" in her university admissions than her 80 for Chemistry or 70 for Physics. But it doesn't. This is unfair.

* Alice (who got 70 for Maths and 70 for Physics) is probably better than a student who gets 50 for Maths and 90 for Physics. This is also not considered.

## Enter Statistics

All these problems arise from different subjects different in two properties. Statisticians call these "mean" and "standard deviation". "Mean" is the average mark. "Standard Deviation" is the "amount of deviation or variation" in the marks.

For example, Chemistry, Maths and Physics have means of 70, 50 and 50 respectively. Just the average of the five numbers.

[In my example, the Means are also equal to the "Medians". The Median is the "value in the middle".]

The computation of the Standard Deviation is more complicated. But if you're interested, you can read about it here. I'll just give you the answer. Chemistry and Maths both have a Standard Deviation of 15.81. Physics has a Standard Deviation of 31.62. This matches our intuition. Physics has double the "variation" of Chemistry and Maths.

## Problems Solved

The Z-Score system solves the problem of different subjects having different means and standard deviations, by "normalising" the raw marks as follows.

```
Z-Score = (Raw Mark — Mean) / St. Dev
```

After the normalisation, the raw marks are transformed into z-scores as follows:

```
Chemistry-1.26, -0.63, 0, 0.63, 1.26
```

```
Maths-1.26, -0.63, 0, 0.63, 1.26
```

```
Physics-1.26, -0.63, 0, 0.63, 1.26
```

Marks below the mean have negative Z-scores. And marks above the mean have positive z-scores. Hence, the effect of different means is "normalised out".

Similarly, dividing by standard deviation "normalises out" differences in variation.

## So, how did Alice do?

Alice's Z-scores are:

```
Chemistry0.63
```

```
Maths1.26
```

```
Physics0.63
```

And her average z-score is 0.84 ([0.63 + 1.26 + 0.63] / 3).

Does it solve the problems we observed earlier? Yes!

* Alices Maths performance now carries more weight. Compared to Physics and Chemistry.

* Also, if Alice got 50 for Maths and 90 for Physics her Z-scores, her respective Z-scores would be 0 and 1.26, giving her an average z-score of 0.63 ([0.63 + 0 + 1.26] / 3). Lower than her current average z-score.

## Concluding Disclaimers

Z-Scores are not perfect. They don't solve all the problems. Just two: that of subjects having different means and different standard deviations.

As promised, I hope to analyse the broader problems in a future article.

![Image](https://cdn-images-1.medium.com/max/800/1*0sWN0ihJzr21ofLLrBjBkA.jpeg)

#### Article 202 · January 3, 2020

# The Slapping Monk

### Religious Tension in Sri Lanka

[Warning: Many of you might find this article problematic (at best). But I'm writing it anyway. Tough things need to be said.]

Let me begin with the viral videos. Ven. Ampitiye Sumanarathana, a Buddhist monk, slaps a man claiming to be a Christian missionary. A police officer is also criticised for "not taking action". In another video, the same said monk verbally abuses a man in the clothing of a catholic priest.

![Image](https://cdn-images-1.medium.com/max/800/1*-TGUUPVhEoHEzmYMBDLX9w.jpeg)

The monk and these episodes were the basis of an interesting argument that I had with a friend.

>>> Friend: Was the monk wrong?

>>> Me: What do you mean by wrong?

>>> Friend: Wrong means doing things like slapping people.

>>> Me: So you mean, If A did X, where the definition of being wrong is doing things like X, is A wrong?

>>> Friend: Yes

>>> Me: Isn't that a tautology?

My friend was somewhat exasperated at my reluctance to directly agree with "Wrong means doing things like slapping people".

While I didn't reveal it (to my friend's exasperation), I did agree with "Wrong means doing things like slapping people". At the same time, I was not completely happy with this agreement. For several reasons. Here's why.

* Doesn't "Wrong means doing things like slapping people" depend on context? After all, "Killing people is wrong" depends on the context. For example, many would agree that self-defence is not wrong. Nor killing an enemy in battle.

* Do we mean "Was the monk wrong?" or "Was the monk doing a wrong thing?" Was the monk a criminal? Or was the monk committing a crime? Was the doer evil? Or was the deed evil?

Why do I even care?

Why can't I (like most people in my "liberal" Twittersphere) just judge the monk as the embodiment of everything evil and be done with it?

## Here's why.

Hurting another, in any context, is distasteful. This is quite simple. But is it unreasonable? This is not quite simple.

Religious "marketing" has always been a touchy subject. Not just in Sri Lanka, but globally. Many wars have been fought. And much blood spilt. In Sri Lanka in particular, conversions by the Portuguese was particularly brutal and savage. More recently, there have been reports of poor Buddhist being "targeted" for religious conversion with economic carrots.

I don't know the extent and nature of the "real situation". A lot of the "data" is anecdotal and hearsay. Hence, I don't know if there is a "problem" and its extent. But what I do know is that some people feel there is a problem. And some people try to "solve" the problem. For example, by attacking churches, verbal abuse and slapping people.

Hence, am I saying that Ven A. S. is reasonable? Not quite. But I am saying that he might have reasons. Whether or not I agree with these reasons is a different matter.

## On Judging

While many might see the monk as wrong, this is why some might see him as "not wrong". Many who find the action distasteful, might, regardless, find it justifiable at some level.

This underlies a deep philosophical point about human nature. And judging humans. It's easy to judge deeds. Relatively. It is much harder to judge people. So much so, that some philosophies prohibit judging explicitly ("Judge not, that ye be not judged" — Mathew 7:1). Others implicitly ("Let his thoughts of boundless lovingkindness pervade the whole world" — Karaniya Metta Sutta).

Am I trying to be a saint? Or "judge" those who aren't? No. I have far more practical and "worldly" motives.

The violent monk is definitely a problem. He must be dealt with. Ideally, by the police. Though given the preferential status Buddhist clergy enjoy in Sri Lanka, I doubt this will happen. At various times in history, the state has regulated and reformed the Buddhist clergy. We badly need such a reformation right now.

But there is a bigger problem. We have a terrible habit of over-simplifying religious tensions. For example, one could argue "Religious freedom is a right. Religious marketers can do whatever they want. Period". But this argument assumes that everyone agrees with this "freedom" or "right". Without agreement, law is suppression. And many feel they are being suppressed in various ways. Whether they actually are, is not the point. Nor is whether others are suppressed even more. The point is that they believe they are.

## So what to do?

For me, the solution is simple. And complex. We must stop pretending that complex questions have simple answers. They might get you more twitter followers wallowing in an outrage culture. But a simple solution is almost always likely to be wrong. And, in the long term, you only end-up fanning hate, division, and intolerance.

Instead, we must see complex questions for what they are. They need clear thought and complicated solutions.

Religious tension in Sri Lanka cannot be minimised to a few YouTube videos. But sadly, they are. We can't afford that.

![Image](https://cdn-images-1.medium.com/max/800/1*TSQcvrO3XAdoRy6Y0SAYXg.jpeg)

#### Article 203 · January 5, 2020

# The Death of the Hypercube

### A tale of Abortion and High Taxes

## Alice, Bob, Charlie and Debbie

Do you support Abortion? You might say "yes" (or that you are "pro-choice"). Or you might say "no" (or "pro-life"). Or you might say, "sometimes". Perhaps in particular situations. Say, when the mother's life is at risk.

Either way, this "where you stand" can be represented on a line. Or the spectrum. For example, if Alice is "pro-choice" and Bob is "pro-life":

![Image](https://cdn-images-1.medium.com/max/800/1*QvQjmabKgq8ypvPE12cQGQ.png)

What about "High Taxes on the Rich"? Again, we could represent "your stand" on a line. We could also represent both your views on Abortion and High Taxes on a two-dimensional (2-D) plane.

For example, suppose Alice supports both High Taxes and Abortion. Bob supports High Taxes, but not Abortion. Charlie supports neither High Taxes nor Abortion. And Debbie supports Abortion, but not High Taxes. We get the following "2-D plane":

![Image](https://cdn-images-1.medium.com/max/800/1*WQ9tfPJLiNFuruBK9XVzgg.png)

## 1000-D

Civics is complicated. It has many issues. Not just two, like Abortion and High Taxes. In reality, there are thousands of issues. From education, to immigration, to poverty. And citizens have (or should have) various opinions on these various issues.

If we were to represent these issues on a diagram, we could need a new "dimension" for each issue. Now, it is easy to represent one issue on a "1-D" line. Or two issues on a "2-D" plane. We could even visualise three issues on a "3-D" cube. But beyond this, things get tricky. How might we draw a "4-D" or "5-D" diagram? And a political discourse with 1000 of issues would need a "1000-D" diagram.

While we can't visualise 1000-D on a diagram, we can represent it mathematically. Such a representation is known as a hypercube.

A hypercube could have any number (n) of dimensions. If n = 1, it is a line. If n = 2, it is a plane. If n = 3, it is a cube. As two (X, Y) numbers or "coordinates" represent a point on a 2-D plane, n numbers can represent a point on an "n-D" hypercube.

## Elephants and Donkeys

Let's go back to our 2-D Hypercube. Suppose Alice, Bob, Charlie and Debbie, live in a country with two dominant political parties. The Democratic Party and the Republican Party. Now, what policies should these parties have on Abortion and High Taxes?

One option might be to consider a "middle-of-the-road" approach. Where the parties adoption the "average" view of the people. Another approach is that parties look at the most popular "locations" on the Hypercube, and adopt those as policies.

For example, in the US, the Democratic Party has adopted a "Pro-Choice and High Taxes" view (like Alice). The Republican Party has adopted the polar-opposite "Pro-Life and Low Taxes" view (like Charlie).

![Image](https://cdn-images-1.medium.com/max/800/1*E2LgwfjZUMRdJ7vhVxJZmA.png)

What party do Bob and Debbie choose? Very often, voters sacrifice one view for another. For example, Debbie might feel that Low Taxes are more important for her, and vote for the Republicans. Bob, might conversely feel that High Taxes are more important and join the Democrats.

![Image](https://cdn-images-1.medium.com/max/800/1*JGDDIn_hrRrAuR1bOzCZ1w.png)

Voters might have diverse views on diverse issues. But the existence of two dominant party identities leads to concentration in a few areas in the Hypercube.

But this leads to an even deeper problem. Consider Bob. He has given up his "Pro-Life" views to join the Democratic Party. How does he justify this to himself?

What many voters end-up doing is to create a "belief system" that "what the party believes is right". This leads to belief systems that are based less on reason and thought, and more on authority and identity.

And since "the other" cannot be dismissed with reason and thought, it must be demonised with hatred and villification. "The other" is far worse than "rationally wrong". "The other" is evil. Sub-human .

![Image](https://cdn-images-1.medium.com/max/800/1*6xfgsVCSZKfdm3eAdi3K_A.png)

And so we start with a hypercube that is infinitely diverse and complex. But sadly ends-up with a simple bi-pole of partisanship, hatred and evil.

#### Article 204 · January 7, 2020

# Digital Data Diet

### Recommendations for the "Digital Data" Ministries of Agriculture, Health and Nutrition

## Prologue: Grandma's 70th

It was grandma's 70th birthday. Her six grandchildren, three children and their spouses were treating her to lunch. At a colourful restaurant.

The adults seemed happy enough. The children were bizarrely silent. Watching a set of squeaking cartoon characters bump about a screen. Each peering into a phone or tablet. Their own phone or tablet.

The restaurant had a comprehensive menu. And a large subset was ordered "family style". But this was for the adults.

The kids had their own "kids menu". Their lunch was as mundane. They hardly looked at their food. From time to time, a disinterested parent would shovel a load of potato chips or chicken nuggets (the two items on the "Kids Menu") into their limp mouths. The cartoon characters continued to squeak. And the kids continued to peer like zombies.

![Image](https://cdn-images-1.medium.com/max/800/1*ap8SIDNrr98Za2OthmR0bw.jpeg)

## This Article: An Analogy

This article is not about kids addicted to screens. Or junk food. But it is about the connection between screens and junk food.

The acceleration of technology has resulted in many challenges. Which we are struggling to understand and counter. On the other hand, we humans have been eating food well before we were humans. While we also have many problems with food, we understand food a lot better than technology.

What can our understanding of food, teach us about technology? And the consumption of data?

In this article, I ponder these questions from a government's or state's point of view. More specifically, the Sri Lankan state.

Can its policies around food, nutrition and health, influence its policies around technology and data?

## Modern Farming

Food begins with farming. If agriculture is efficient, food is likely to be better in both quality and quantity. More quality and quantity would promote value addition. And a more vibrant economy around food. For example, there would be more restaurants and a "food culture".

Suppose you visit a Sri Lankan government department. Say to fix some anomaly in your pension. You will consume and interact with a lot of data. But most of this data is "non-digital". Data input is by hand. Filling paper forms. These forms add to larger batches of forms. Usually stored in several paper "files". Output consists of reading these files. And "data processing" happens in the minds of humans.

To be fair, this system works reasonably well. And it does have advantages. It is (probably) impossible for a hacker in Eastern Ukraine to nobble your pension numbers. Just as many ancient farming techniques are healthier and even organic. But like ancient farming techniques, these systems are slow. And expensive. And inefficient.

Consider all "data interactions" (input, processing and output) the ordinary Sri Lankan has. From pensions to banking, to welfare, to health, to transport. A significant part of these involves "ancient farming techniques".

![Image](https://cdn-images-1.medium.com/max/800/1*uY916dAkhHkBL3X_tEWelw.png)

## Food Distribution

Suppose all our farmers produced all the food Sri Lanka needed. Using the most efficient and modern farming techniques. Enough to make Sri Lanka self-sufficient in food. And a surplus to support value-added exports. Not only do we have all the rice we need, but we also dominate the market in organic rice noodles and rice crispies.

But what if our roads and rail networks were crappy? What if all the rice never left the farms? All modern farming would go to waste.

The same applies to data. Even if all government services are digital and digitalised, they are wasted if citizens cannot access them. Less than 35% of Sri Lankan citizens have internet access. Those who aren't, cannot optimally utilise digital services.

The problem is not purely about infrastructure. Like our rice distribution and transport is controlled by monopolistic businessmen with political connections, telecommunications infrastructure suffers from quasi-oligopolistic control. We need more competition and freer markets. And regulation that would enable this.

We also need more "food-technologist" and "farmers" for digital data. People who design new types of data, design them and grow them. In other words, application designers, product managers and software engineers.

![Image](https://cdn-images-1.medium.com/max/800/1*POqoPtTVjyZn-YgyxtyUMw.jpeg)

## 2000 K. Calories Per Day

Despite being connected, many Sri Lankans cannot afford data. And hence can't make the best use of tech and its applications. Food is available. But it is too expensive for too many. Hence, many Sri Lankans don't meet their "data" needs. Like many Sri Lankans (particularly Children) don't meet their calorific needs.

Network bandwidth and data should not be the luxury it is. These days, it is a commodity. Like rice or dhal. Not a luxury item. Like fine wines or caviar.

As the government has goals around nutrition and calorific intake, why not goals around internet data access? For example, what if (for "starters") every citizen has access to 1GB of data per day?

![Image](https://cdn-images-1.medium.com/max/800/1*oIX1pMiuZ11wLdpmKK3nmQ.jpeg)

## A Balanced Diet

But there is no point in giving citizens 1GB per day if that is entirely spent on Facebook, YouTube or Gossip LK. Like 2000 K. Calories entirely composed of refined sugar and crisps (or chips and nuggets, for that matter). Hence, the digital diet needs to be balanced.

While we do understand that fresh fruits and vegetables are healthy, we don't have a good sense of what precisely makes a healthy "digital diet". However, our understanding is steadily improving. We know that a lot of social media content is like sugar. We get an instant-dopamine boost and a sudden crash. Leading to an immediate need for more. We have a much better understanding of how some content is addictive. Like cocaine or heroin. We also know that certain types of data, like long-form content (e.g. academic courses, and medium articles😉), is "good for you".

Hence, just as governments educate citizens on good food, they could educate on useful data.

Just as we need more Nutritionists, Doctors and Therapists, food-wise, we need people equivalent "data-employees". We need people who can advise citizens on how to use data and get the most out of it. We need psychologists and therapists who can help people deal with the fallout. Like the sad kids at Grandma's 70th.

![Image](https://cdn-images-1.medium.com/max/800/1*JM1LNhCT2P1P32mmdZyVFw.jpeg)

## Food Imports and Exports

Most software used in Sri Lanka, both in the public and private sector, is designed and manufactured abroad. A lot of the raw data consumed also originates overseas. That's like importing all of our food from foreigners.

Just as many countries exploit our "third world" status and export us "third-grade" food, a lot of the software we buy is also "third class". But we are happy to smack our lips and pay millions. Because "they are foreign" and hence "must be good".

Hence, just as we should be mindful of our export and imports of food (and other goods and services), we should be aware of our "software and data trade deficit". Any government in its right mind would want a plan that could turn the deficit into a surplus.

![Image](https://cdn-images-1.medium.com/max/800/1*dTHbVzZMZHJVBCh7xX5BOw.jpeg)

## Summary Recommendations

Suppose Sri Lanka had a "Digital Data" version of the Ministries of Agriculture, Health and Nutrition. They should consider the following questions:

* What proportion of government processes use "Modern Farming"? How might the proportion increase?

* How efficient is "Digital Data Distribution"? Is the market free? Are there monopolies? Is regulation needed?

* Do all citizens have access? Is there malnutrition? Can every citizen have 1GB per day?

* Are citizens getting a "Balanced Diet"? What about obesity and drug addictions? How do you deal with drug barons?

* How do we educate more Designers, Product Managers and Engineers? And "Digital Nutritionists" and "Therapists"?

* Finally, how do we fix our huge Digital Software and Data Trade Deficit?

#### Article 205 · January 12, 2020

[Comment]You don't consider දාර්ශනය a reasonable way to find පිළිතුරු to තමාගේ ප්‍රශ්න?

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

#### Article 207 · January 20, 2020

# Lost in Translation

### One Nation divided by Three Languages

Suppose a random Sri Lankan met another random Sri Lankan. Would they be able to talk to each other? And understand each other?

The 2012 Census has some interesting data about what languages Sri Lankans speak. In this article, I analyse this data. And also speculate on some of the consequences of these statistics.

![Image](https://cdn-images-1.medium.com/max/800/1*rmwyPko7Xlaa4t_zV0loGA.png)

## What do Sri Lankans Speak?

Here's a diagram summary of the census data.

![Image](https://cdn-images-1.medium.com/max/800/1*PWBdyksh7koCtc0zilocjA.png)

The circles represent people who speak some set of languages. For example, the red circle represents the 56% of the population who speak only Sinhala. The lines between the circles represent the set of common languages that the people across circles can use to communicate.

For example, the people in the Sinhala + Tamil circle (orange), communicate with the Tamil + English (green) in Tamil (yellow line).

[For clarity, I have excluded "tiny circles". For example, a small proportion of Sri Lankans speak only English, and a few also speak other languages. I have excluded groups that have under 100,000 speakers.]

## "Weak" Understanding

There is a ~82% chance that the two random Sri Lankans will speak a common language.

Is 82% good enough? Should we do better? Should it be 100%? The "shortest path" the 100% would be for the 13% who don't speak Sinhala to learn Sinhala.

But would that mean that Sri Lankans would understand each other? Would that be the end to all tension around language and related ethnic, social, economic, political and religious tensions?

Intuitively, it scarcely seems the case. And were this intuition true, the 82% would be at best a "weak" metric. And at worst meaningless.

## Dividing Lines

Our 82% metric measures "languages shared". But what about "languages not-shared"?

What are the consequences of one person speaking a language that the other does not speak?

### English

Consider two Sri Lankans. One only speaks Sinhala (red 56%). The other speaks both Sinhala and English (purple 15%).

On the one hand, this is an example of the 82%. The two can "talk to each other". On the other hand, there is an asymmetry. The English Speaker has access to all the advantages afforded to English Speakers.

For example, English Speakers can speak to other English Speakers. Consume all manner of content produced in English. And perhaps most significant to Sri Lanka, they are members of the "English-Speaking" club. Which, for most of the last two centuries, has dominated economic, political and social power.

![Image](https://cdn-images-1.medium.com/max/800/1*4yB9ihSaS0jNNQJyyuK9oA.png)

### Sinhala

Since independence, Sinhala as steadily caught-up with English as the "language of privilege".

While English still (probably) affords more economic power, Sinhala is top-dog in broader settings. It is almost impossible to work with a government ministry or department without Sinhala. Most official documents, notices and signage are published exclusively in Sinhala. At some security checkpoints, merely speaking in Sinhala reduces one's chances of being suspected of being a terrorist.

Tied to "English-privilege", in some circles, Sinhala continues to have adverse effects. For example, in some social circles, "Sinhala-Speaking" is considered the opposite of "English-Speaking". Rural and unsophisticated. A few even equate Sinhala-Speaking to fascism or worse.

![Image](https://cdn-images-1.medium.com/max/800/1*e3GrXJO3wpdMo6gqV-Ig5Q.png)

### Tamil

Just as English and Sinhala divide, mostly favouring speakers over non-speakers, Tamil also divides, though usually disfavouring speakers. In many cases, the disfavour is compounded by irrational paranoia, often fuelled by politicians and religionists. To many Sinhalese, Tamil is the language of "LTTE Tiger Terrorists", "Wahabists", and more recently "ISIS Terrorists".

![Image](https://cdn-images-1.medium.com/max/800/1*WNMwKxmF8OY4lpCuEmqZLg.png)

## Compound Divisions

Multiple dividing lines could compound.

For example, a Sinhala + English (purple 15%) speaker, might discriminate a Tamil Only (yellow 12%) as being (say) both "Non-English-Speaking" and an "LTTE sympathiser".

![Image](https://cdn-images-1.medium.com/max/800/1*FplOMpDFejyhkcgTBDxxcQ.png)

## "Strong" Understanding

Suppose a random Sri Lankan met another random Sri Lankan. What is the probability that each speaks all the languages the other speaks?

About 36%. Hence, ~64% of the time, there's some possibility of "language division".

Happily, there's a solution. The human brain is more than capable of learning three languages. And often even more.

What should you do if you're a Sinhala only speaker? Again, learning Tamil gives you the best opportunity of "expanding" your ability to understand other Sri Lankans. Similarly, if you are a Tamil only speaker, then Sinhala.

Of course, many Sinhala only and Tamil only speakers will try to learn English as their "next language", particularly since it has disproportionate advantages in Sri Lanka, and is an international language. But even these groups, could learn Tamil and Sinhala, respectively, parallel to English.

![Image](https://cdn-images-1.medium.com/max/800/1*gt9Lnx9amBsQaBmkb3bmDw.png)

## Concluding Caveats

Much needs to be done besides people learning languages. For example, official documents, notices and signage need to appear in all three languages. Not just one or two. Deeper discriminations based of language, beyond mere documents, need analysis and solutions.

You might also claim that I've reduced a complex problem, to a single factor: language. This is a fair critique. In the end, my "language model" is only a model. And all models are wrong. But some are useful. Hopefully, this is.

Finally, you might claim that I made unequal things sound equal. For example, that I make the English, Sinhala and Tamil "divides" are equally problematic. Again, fair critique. Take my "sounds" as more qualitative, than quantitative.

On the one hand, acquiring a "strong" understanding of each other's languages won't necessarily lead to strong understanding as people. Many Sri Lankans speak many languages. But in their thesauri, "Tamil" is a synonym for "Terrorist", and "Sinhala" is a synonym for "Nazi". As long as these deeper prejudices exist, learning languages alone won't foster real understanding.

On the other hand, learning others' languages will be a start. And will have a multitude of other benefits. Even beyond understanding.

#### Article 208 · January 28, 2020

# A Tech Startup Ecosystem in Sri Lanka (I)

### Part I: What makes a good tech startup ecosystem?

This article (Part I) paraphrases a conversation I had in late 2018. With an Israeli Entrepreneur-turned Angel Investor. Mostly on the question: "What makes a good tech startup ecosystem?"

## The Startup Paradox

The ideal tech startup ecosystem is a "support system". It has everything a startup needs. Funding is available at a reasonable cost. And it has connections to markets and economies.

Thus, the ideal tech startup ecosystem becomes a magnet for talent. Not only new entrepreneurs looking for their first wins. But also experienced veterans. Seasoned entrepreneurs who have succeeded elsewhere, often many times. "Knowledge organizations" like universities and research groups, join these people.

But I could have described many parts of the world. Not all of which are startup hubs. The great startup hubs of the world have something else. And here lies the paradox.

Ideal startup ecosystems are "nice places". Complete with funding, market reach, connections, talent, experience and knowledge. But invariably, the best startup entrepreneurs tend to come from "not-so-nice places". Often places with economic hardship, war and persecution.

Thus, often a startup-hub is not just one place. But two places: the nice place and the not-so-nice-place. The former is the "official startup hub". While the latter is where many of the entrepreneurs come from.

![Image](https://cdn-images-1.medium.com/max/800/1*Qztwn7tSytn9wkaVUVrTRQ.png)

## Nice-places and not-so-nice-places

### Silicon Valley (SV) Type

Silicon value has all the "nice" properties of a startup hub, from almost infinite funding, to broad market reach. However, a disproportionate number of successful SV startups have been founded by immigrants from "not-so-nice-places". Russia has been, for several years, the "not-so-nice-place" of choice. Followed by China and India. In fact, there is an SV joke that no startup is complete without a Russin-Jewish co-founder.

This dynamic is also true for other parts of the US like New York City, Boston, and Los Angeles. And many European cities like London, Berlin and Paris.

### Beijing/Shanghai Type

Beijing and Shanghai are fast becoming "nice-places" to rival SV. However, its source of "not-so-nice place"-entrepreneurs has been not Russia, or other parts of the world. But China itself.

In the last couple of decades, China has accelerated from extreme poverty to significant prosperity. But many parts of the country are still relatively poor. Thus, past memories, and present inequalities, motivate people in "not-so-nice" parts of the country to seek prosperity.

Bangalore, India also follows this type. Like Beijing and Shanghai, part of the "niceness" is also driven by "returners" particularly from the US.

### Tel-Aviv Type

Israel's "not-so-niceness" derives, not from poverty, but from geopolitics and history. Israel's neighbours want to blow it off the face of the earth. To this end, they have waged many wars. Both military and "diplomatic". While on the surface Israel might have the "niceness" of a developed country, there is a constant "not-so-nice" threat of destruction. This has driven unparalleled development. Particularly in defence and security technology.

### Singapore Type

Singapore's "not-so-niceness" comes from its government. Which is, on paper, democratic. But in many ways autocratic. There is a significant amount of pressure applied to all manner of institutions, from universities to companies, to innovate. Particularly technology.

## More Reflections

None of these "types" is completely single-type. Each is some combination of all four types. The "types" are more an understanding aid.

Israel and Singapore demonstrate that the "nice place" and the "not-so-nice place" can be one and the same. In a sense, it is more a mindset, than a place.

"Nice places" often cannot be "not-so-nice places". Except in exceptional cases like Israel and Singapore. For this reason, there are very few "2nd or 3rd Generation" entrepreneurs in "nice places" like SV. While the first generation has enough memory and experience of "not-so-nice", their children rarely inherit this motivation.

The same place can be "nice" for some people and "not-so-nice" for other people. On the one hand, most of Sri Lanka has been, historically, quite a "nice" place. Basics like food and safe lodging are abundant. On the other hand, parts of the country are much harder to live in. Similarly, some ethnicities and communities have faced more hardships than others. This "not-so-niceness" might have contributed to more entrepreneurship in the said places and groups.

## Can Sri Lanka Build a Tech Startup Ecosystem?

The Israeli Entrepreneur-turned Early Stage Investor seemed to think not. Why? Sri Lanka, while a "nice enough" place, had almost no supply of "not-so-nice" talent. At least that's what he thought.

But is that actually true? Might things change in the future?

I will address this in Part II.

#### Article 209 · January 28, 2020

# CoronaVirus Numbers

### As of January 27, 2020

* Incubation period (time from exposure to developing symptoms): 2 to 14 days. Contagious during this time.

* Confirmed Cases (As of 1/27): ~4,673

* Confirmed Deaths (1/27): 106

* Death Rate: ~2.3%

* Basic reproduction number ("how many people a newly infected person is likely to pass the virus to"): 1.4 to 3.8

* Confirmed Cases outside China: 77

* Confirmed Deaths outside China: 0

* Symptoms: Fever in 90%, dry cough in 80%, shortness of breath in 20%, respiratory distress in 15%.

* Estimated Cases (assuming a 10-day delay between infection and detection): 26,200 infections (as of 1/27 — Northeastern University)

[Source: 2019–20 Wuhan coronavirus outbreak from Wikipedia]

![Image](https://cdn-images-1.medium.com/max/800/1*LovjAVNAUvu3fXKZQwzHow.jpeg)

#### Article 210 · January 30, 2020

### Digitalising Identity (Part 1)

# How much of my private data is public?

### And what is my "data exposure"

We all share a lot of our data with the outside world. Not just on social media. But also with Banks, Hospitals, Phone Operators and the Government. In Sri Lanka, the "process of sharing" is still often manual. When we open a bank account, we often fill in paper forms.

But digitalisation will likely replace these manual processes in the next few years. Making many processes more efficient and accurate. And benefit consumers in all sorts of ways. But there are also risks. Particularly around privacy and data exposure.

This article is the first in a series about "Digitalising Identity". Written from a Sri Lankan perspective.

In this article, I address one of the most fundamental questions about Digital Identity: What is my "data exposure"? Or other words, how do you answer the question "How much of my private data is public?"

## Example Data: Sri Lankan National Identity Card

![Image](https://cdn-images-1.medium.com/max/800/1*D5mhSAj3KU8g3AQE6jezEQ.png)

Consider the data on your the front face of your Sri Lankan National Identity Card. It contains the following fields of data.:

* 12 digit NIC Number

* Full Name

* Sex

* Date of Birth

[We will ignore signature and face photo, until a later article]

How much information is here? Let's consider each field one by one.

### Sex (and Information Content)

In computer science, we have a notion of "information content". Which we can use to measure the "amount of information" in some piece of data. "Information content" is the smallest number of bits needed to store some data. Equivalently, it is the least number of "binary questions" that might infer the data. A binary question is a question with only two possible answers.

For example, "Sex" takes two values "MALE" or "FEMALE". Requiring a single bit of storage. Say "0" for "FEMALE" and "1" for "MALE". Using the "question intuition": To reconstruct the data, you only need to ask one question. Something like "Are you FEMALE or MALE? " or "Are you FEMALE?"

Note, in practice, we might use more bits to store the data. For example, we could store "Sex" as six Unicode characters (which would take 96 bits). But "information content" refers to the "smallest". Which is just one bit.

### Date of Birth

What is the information content of "Date of Birth"?

If we use a MySQL DATETIME data type to store "Date of Birth" we could need up to 24 bits of data. However, this is not the "smallest" amount of data. Assuming that we are only interested in people who were born within a window of about 200 years, "Date of Birth" can only take about 73,050 distinct values.

What is the information content of 73,050 distinct values? We can answer this question by asking "What is the least number of binary questions that might infer this data?"

The list of binary questions would be something like this:

* Is your DOB in the first half of the 200 years or the second half?

* If you answer "second", we split that half into two halves and ask the same question.

* And so on.

* In the end, we will end up with just two possible birthdays.

The mathematicians among you will notice that the number of questions is about log2(73,050) or (rounding up) 17 questions. Hence, "Date of Birth" needs about 17 bits.

### NIC Number

>>> 1970 510 1234 5

The Sri Lankan NIC number consists of four parts:

* First four digits: Year of Birth (e.g. 1970)

* Next four digits: Day number in Year of Birth (e.g. 10 if you were born on January 10th) + 500 if you are female. Hence, a female born on January 10th would have "510". A make would have "010".

* Next four digits: A serial number

* Last digit: a checksum

What is the information content of the NIC Number?

You would have noticed that the information contained in the first seven digits is the same as the "Date of Birth" and "Sex" combined. Hence, it is 17 + 1 = 18.

The four-digit serial number can take any value, and hence has 10,000 unique values. Thus, if has log2(10,000) or 14 bits of data.

The final checksum derives from the other 11 digits. And hence, it doesn't contain any new information of its own.

Hence, the NIC Number has 18 + 14 = 32 bits of data.

### Full Name

What is the total number of unique "Full Names"?

It is difficult to say exactly. But probably a number in the order of the size of our population. Or ~22,000,000. Hence, "Full Name" contains about log2(22,000,000) or 25 bits of information.

[In practice, information systems rarely store "Full Name". And instead store a combination of "First Name", "Middle Names" or "Middle Initials" or "Initials", and "Last Name". For simplicity, we'll ignore this fact for now.]

### Complete NIC

Hence, what is the total amount of information in the NIC?

Since, "Date of Birth" and "Sex" are contained in "NIC Number", the total information is 32 (NIC Number) + 25 (Full Name) = 57 bits.

![Image](https://cdn-images-1.medium.com/max/800/1*HjD-LON_8XX5dPCujUzy-w.png)

## Case I: Bank

Suppose you want to open a Bank Account. And suppose the Bank needs your "Full Name" and "Date of Birth".

[In practice, Sri Lankan Banks need all the NIC information. Plus tonnes of other details. But let us assume this scenario for now.]

Let's also assume that your only private data are the 57 bits of information on your NIC. For the sake of these cases.

How much information have you "given away" to your Bank? 25 (Full Name) + 17 (Date of Birth) = 42 bits. Hence, 42/57 or 74% of your private data is "publicly exposed".

![Image](https://cdn-images-1.medium.com/max/800/1*QKUu7O5XNe3BuejUoNl9gA.png)

## Case II: Minimalist Bank

Suppose Sri Lanka has comprehensive and enforced data protection and privacy laws. Suppose these laws make sure that institutions (like Banks) only ask customers for a minimal set of information. The minimum they need to do their job.

For example, suppose that "Date of Birth" is only used to verify that the customer is 18 years or older. Hence, the Bank is not allowed to ask for "Date of Birth". Only "Are you over the age of 18?"

Since "Are you over the age of 18?" is a binary question, this contains 1 bit of information.

[Note, this "intuitive binary question" approach, is an approximation. "Are you over the age of 18?" actually needs less than one bit. But we'll ignore this technicality. You can learn more at Entropy.]

Hence, you only need to give the bank 25 (Full Name) + 1 (Are you over the age of 18?) = 26 bits of data. Instead of 42 bits. Now, your data exposure is 26/57 or 46%.

![Image](https://cdn-images-1.medium.com/max/800/1*t0MwOPaE0aQwwImOCQNNQQ.png)

## Case III: Hospital

Suppose you need to visit a doctor, and the Hospital need your "Date of Birth" and "Sex". This would contain 17 (Date of Birth) + 1 (Sex) = 18 bits of data. 18/57 = 32%.

![Image](https://cdn-images-1.medium.com/max/800/1*oFBSerOi8u2dKTTxuYoHNw.png)

Now, suppose you also opened a (non-minimalist) bank account (like Case I). What is your total data exposure? Across both Bank and Hospital?

Before we answer that question, why would you care?

Suppose you are of the Mormon religion. And suppose your Bank knows this. And suppose the Hospital has a racist policy of charging Mormons double. However, since the Hospital doesn't have your "Full Name", it doesn't know your religion. As far as the Bank and the Hospital are concerned, you are "two people". Each can't connect your two accounts.

But what if a teller at the Bank (who knows your name) is married to an accountant at the Hospital. They might pass information between each other. And your privacy is blown.

How might we represent this in our "data exposure" metric?

## Average Data Exposure

Let's assume that the Bank and the Hospital are the only data collecting organisations in Sri Lanka.

And let's assume that they are equally important. We could compute your "average data exposure" as a weighted average of your exposures. Or 74% × 50% + 32% × 50% = 53%. In the case where they can't share data.

Now, in the case where the teller and the accountant are sharing your data with each other, each has 25 (Full Name) + 17 (Date of Birth) + 1 (Sex) = 43 bits. Or 43/57 = 75%. Since, both parties have all this data, your "average data exposure" is 75% × 50% + 75% × 50% = 75%.

Many techniques can minimise "data exposure" when confronted with multiple (possibly colluding) data collection organisations. Including "differential privacy".

## Summary and Future Articles

In this article, we discussed the computer-scientific concept of "Information Content". And, based on this, derived a "data exposure" metric. We extended this to an "average data exposure" metric, to consider multiple data collecting organisations.

We also discussed "minimalism" or how data collecting organisations should only collect the minimal data needed to "do their job". "Minimalism" and many other concepts we discussed (and will discuss in future), depend on data protection and privacy laws.

We also, explained how "data exposure" can explode when data collecting organisations collude to (possibly illegally) share data.

In future articles, I hope to address the following questions:

* How do we design minimal data sharing schemes?

* How does data exposure relate to identity and authentication?

* How do we prevent "data exposure" explosions, when confronted by colluding data collecting entities?

* How do we implement all of this in a digital system?

Please comment if you have ideas on more interesting questions.

#### Article 211 · February 9, 2020

# Digitalising Identity (II)

### Part II: Digital Identity, Ownership and Protection

[This article is the second in a series about Digitalising Identity. See also Part I.]

## Identity

What is our "identity"? It is who we are. It is the "collection of things" that "make us". Or the information that "defines us". Everything from our DNA to our physical appearance, to our memories. To our ethnic, religious, cultural, political and social affiliations. They are all part of our identity.

This information can be encoded as digital data. For example, our DNA could be sequenced. And this sequence could be digitally represented. We could take a photo of our face, and represent it as a "bit map". We could record our voice and store it as an mp3 file. Hence, in all these various ways, an increasing proportion of our identity is "digitised". Into a "digital form".

The digitisation of identity has led to a vast digital industry. Offering various goods and services based on identity. Facebook lets you interact with the digital identities of people and businesses. Socially, but also economically and socially. LinkedIn hosts a subset of your identity that reflects your employment record. And helps you find jobs, network professionally, and gloat over colleagues with less impressive profiles. Google hosts various parts of your identity for free. In the form of search history, emails, and calendar events. Convenient digital alternatives to public libraries, snail mail, and physical diaries. Which Google effectively "sells" for vast amounts of ad revenue.

## Ownership

Intuitively, we might believe that we "own" our identities. Digital and Analog. Online and Offline. But ownership is a relative concept. Relative to enforcement. Without enforcement, ownership is meaningless.

In turn, enforcement is also relative. Relative to power. In any society, the powers-that-be determine what enforcement and ownership mean.

For example, a government might deem that all the phone records of its citizens are its property. And shady civil servants might be eavesdropping on our most intimate conversations. Similarly, a multi-national corporation might deem it owns "all your photos" because its "terms of conditions say so". And because you have no chance of winning in court. Even if the TOC did not say so.

Which definition of ownership you believe to be "right", depends on your political beliefs. If you are a communist, you might believe that no ownership should be private. If you are a capitalist, you might believe that all should be. On identity, there are even deeper nuances. Some capitalists believe that the original owner should always own private identity data. Others believe that it might be bought and sold.

## Large and Small Rebellions

No political ideology is absolutely good or bad. Their relative goodness or badness depends on their effects. For example, if ownership and its enforcement result in extreme inequalities, people suffer. And suffering people rebel. And large rebellions lead to large-scale pain and destruction.

Not all ownership-driven rebellions are outwardly political. If you have had a severe illness, and your insurance provider knows this, your premium might be expensive. Exorbitantly so. One might argue that this is rational, even "fair". But it all sick people were priced out, medical insurance would be meaningless. Hence, regulations that ban higher premiums for "pre-existing conditions" are good all round. For both the patient and the provider. Other regulation protects against "unethical" sharing of data. For example, an medical insurer should not buy credit card history from a bank. In these examples, the principle is the same. Extreme asymmetries and inequalities in access to data lead to problems. And potential rebellions.

Large rebellions can be prevented. Via small rebellions. Whenever the existence or potential for extreme asymmetries and inequalities are detected, there should be some "letting-off of steam". The asymmetries and inequalities must be reduced. This might cause some short term pain, but it is better in the long term. For example, regulating insurers might dent their profits in the short term, but is better for both patients and providers in the long term.

When dealing with asymmetries and inequalities in digital identity, small-scale rebellions come in the form of introducing legislation. Usually, in the form of data protection laws.

![Image](https://cdn-images-1.medium.com/max/800/1*ya_viQAjsoKpTb7lKZMk3w.png)

## Horror Stories

Recently, I heard a horror story.

A reputable Sri Lankan bank emailed a spreadsheet to a data analytics firm. The spreadsheet contained thousands of rows of client credit card information. Including the card numbers, the client names, and transaction history. The emailing happened via an unsecured email connection. Employees of the data analytics firm had full access to all the data.

But the real horror of this story is that, all this was not illegal. We don't have data protection laws that prevent such actions. And as long as this is the case, more and more of this will happen.

But this is not a Sri Lankan phenomenon. Silicon Valley is probably the best example of a complete breakdown. Of Digital Identity and Ownership.

Like in Sri Lanka, there is almost no protection of personal data, when it comes to large tech companies. Like Google and Facebook. Security breaches and hacks do happen from time to time. But the real damage comes in the form of huge asymmetries and inequalities of data ownership. Given the data ownership advantage large tech companies have, they have an asymmetric power in profiteering from data. As a result, no other businesses can compete with these behemoths. This data inequality leads to income inequality and wealth inequality. And also inequalities in political and social power and dignity. San Francisco might be home to some of the world's wealthiest people. But it has also become the homelessness capital of the world.

![Image](https://cdn-images-1.medium.com/max/800/1*ZMx9I7qNKIwAV-7pQRaCdg.jpeg)

## What to do?

If Sri Lanka can learn anything from Silicon Valley, it is that Digital Identity in particular, and data in general, needs protection. What are some good fundamentals to follow?

The problem with fundamentals is that no fundamental is perfect. And if you believe in the perfection of fundamentals, you become a fundamentalist. Usually leading to a lot of pain for you and others.

Hence, I'm not a fan of many fundamentalist views of data, its ownership and its protection. Including communist and capitalist views. The problem with these fundamentals is that they are too broad and vague. And for every example of their success, there are as many failures.

There are better fundamentals. For example,

* Minimalism. It's better to concentrate as much data ownership with individuals. Make sure that larger entities like states and corporations have a minimal set of information they need to do their job.

* Equity. Whenever a small number of players have an asymmetrically large proportion of data, the industry suffers. The small amount of players will prosper in the short term, but everyone loses in the long run. Hence, small rebellions that remove inequities will prevent large rebellions that destroy industries.

The next step is a set of small rebellions. That might cause a small amount of pain. But is better in the long term. Ones based on minimalism and equality. That will make sure our digital identities are protected.

#### Article 212 · February 9, 2020

# The Socratic Method

### Dumb people have all the answers. Smart people have all the questions.

## My favourite meetings

Like most people, I am not overly fond of meetings. But one type of meeting, I do like. One-on-ones. Meetings I have with one other person.

One-on-ones (1:1s for short) have many benefits. They can be had in informal settings. Like a cafe. Or a park bench. Or even while walking. "On the hoof". They tend to be far more productive. Because the "agenda" must be relevant to both parties. Unlike most large meetings, where one, two or a few people talk. While others twiddle their thumbs, phones. Or sleep.

But one of my favourite benefits of 1:1s is that they are the perfect setting for applying one of the most potent conversational tools: The Socratic Method.

Let me demonstrate.

Suppose I'm having a 1:1 with an engineer that I'm mentoring. She says something like:

>>> "I'd like to be a more productive coder. I'd like to be able to write more code in less time. How might I do that?"

I could reply,

>>> "Use a better IDE [Integrated Development Environment — a tool for writing programming code]. XYZ is excellent."

or

>>> "You should master Git [A tool for maintaining multiple versions of code]. Here are a couple of tips..."

or

>>> "Here's a reading list. Some great books on programming."

or

>>> "Let's do some pair programming [where one programmer codes and the other watches, observing possible mistakes or patterns]. Then, I'll be able to suggest something."

or

>>> "That office chair looks very uncomfortable. Get an ergonomic evaluation and a better posture".

All of these are reasonable answers. But there is a problem. They are answers. But what, you might ask, is the problem with answers? Let me explain.

## The Problem with Answers

To start with, answering a question might be based on or lead to the assumption that the question has only one answer.

For example, my coding mentee might become obsessed about the perfect IDE. And forget about Git, programming books, pair-programming and posture.

But even if I caveat my answer with "this is one of many things you could do", there is a more severe problem. When I answer a question with an answer, there is no "creation of knowledge".

Knowledge passes from one person to another. Between us, there is no new knowledge. Even though one of us might now have more knowledge. The system as a whole, has not gained.

## The Socratic Solution

Alternatively, I could have "answered" the question as follows:

>>> "Why do you want to write more code in a day?"

or

>>> "What makes you think you are not writing enough code?"

or

>>> "How would you describe a "productive coder"?"

When a question answers a question, there is an opportunity for "creating" knowledge. Or "expanding" knowledge.

For example, I get a better sense of why my mentee wants to code more. Or anxieties she might have about not being a good enough coder. Or (possibly flawed) views and opinions she has on what makes a "productive coder". The "correct answer" to her question might have nothing to do with writing more code. It might have something do to with writing smarter code. Or even nothing to do with code at all. The motivation behind the question might be about getting more respect from colleagues. Or a higher salary.

And to my question, my mentee can reply with yet another question. The "Socratic Method" refers to this type of cooperative conversation. Based on questions and constructive argument.

The Greek Philosopher Socrates loved asking questions. Especially from self-important dogmatists who believed they had all the answers. And he would follow one question with another question. Many of his interlocutors were annoyed by his behaviour. And dubbed him a "gadfly". Many believed that they wanted to undermine his power.

In reality, Socrates had only one aim. He wanted to expand knowledge. But not just his, but the collective knowledge of all humanity.

![Image](https://cdn-images-1.medium.com/max/800/1*q-eNBoG6iSyUTbB6HCaI6A.jpeg)

## Anti-Patterns

### "Venerable Experts"

Sadly, much of Sri Lankan discourse has a very anti-Socratic nature. We love authority and the opinions of authorities.

Recently, I attended a Bhana (Buddhist lecture). Where the lecturing monk was not only irrelevant but also inaccurate. I am sure many in attendance recognised these errors, but no one questioned anything. This is so ingrained in our culture that "saying no" to a Buddhist monk is considered taboo.

This basis extends to education in general. In primary and secondary school, the teacher is always right. In university, the lecturer or professor is. And in real life, we tend to believe anything experts tell us. Because they are "experts" or "professors" or "reverends" or "doctors".

### "Paper Qualifications"

A common question in professional recruiting is:

>>> "Is this person suitable for the job?"

The easy way out is to look at their paper qualifications. "He has a Masters Degree. He must be good. We don't have to interview him!"

A more challenging course is to ask a question. Or to be exact, many questions. In the form of an interview. Sadly, many employers are unable to conduct an interview. That might see through dubious paper qualifications. Because they don't know how to judge a good employee. So they default to the easy answer. "Do they have a degree? Yes! End of story"

## Concluding Questions

Should you use the Socratic method?

Is the aphorism "Dumb people have all the answers. Smart people have all the questions" true?

I'll leave that as an exercise for you, dear reader. You could try answering it.

Or better still ask a question.

#### Article 213 · February 10, 2020

# Sea Levels Rising

### What if Sea Levels rise by 1m?

>>> 

Recently I posted a video simulating what Sri Lanka would look like if sea levels rose by 100m. While many found the video interesting, even entertaining, I did caveat the tweet with:

>>> To be clear, this is an unlikely scenario. Estimates indicate a few meters in the next century. But even 1m would submerge many densely populated parts of the country, incl. much of #Colombo and #Jaffna.

A rise of 100m is almost impossible. Possibly for several centuries. Probably until after the next ice age. On the other hand, 1m is entirely possible. Certainly in a century. Possibly in decades.

What if Sea Levels rise by 1m? What would be the impact on Sri Lanka? How many people would be affected?

## Methodology

In this article, I attempt an approximate answer to these questions. "Approximate" because my population information (2012 census) was at the Grama Niladaari Division (GND) level. I assume that the altitude (above sea level) for the entire population in the GND is the mean altitude of the GND.

Since this analysis mostly considers small altitudes (e.g. less than 1m), this approximation is reasonable. For example, if the mean altitude of the GND is below 1m, most of the population is likely to live below 1m.

### Sri Lanka (621,432 people at risk, 3% of population)

About 621,432 Sri Lankans or 3% of the population live below 1m. While the GNDs at risk cover a relatively small area, these are usually densely populated.

![Image](https://cdn-images-1.medium.com/max/800/1*ocUtlgMTcKF-ov-gLPYAXg.png)

### Colombo (100,607, 4%)

The largest number of people at risk by district live in the Colombo District. Mostly concentrated around Colombo North, Colombo Central, and the Moratuwa area.

![Image](https://cdn-images-1.medium.com/max/800/1*R3fTTkDn7cSdmveanOLmHw.png)

### Batticaloa (84417, 16%), Ampara (77540, 12%), and Trincomalee (62290, 16%)

After Colombo, the most populous at-risk districts are Batticaloa, Ampara and Trincomalee. With about 16% of their populations at risk, Batticaloa and Trincomalee have the highest proportions of the population at risk.

![Image](https://cdn-images-1.medium.com/max/800/1*5WaR5weZBTQzRsGHUFKpsQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*2-gU339gdiyG8LqqPEjKJw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*sM4QtUKGgFg7nNXxJlhx5w.png)

### Puttalam (59818, 8%)

![Image](https://cdn-images-1.medium.com/max/800/1*R2LejSIM9vpmlFsIKoq17Q.png)

### Jaffna (54589, 9%)

![Image](https://cdn-images-1.medium.com/max/800/1*pFYhNI7xNLgRc2x4kX9q2g.png)

### Kalutara (51220, 4%) and Gampaha (33458, 1%)

![Image](https://cdn-images-1.medium.com/max/800/1*f9etJME1cxtJbIHEC4O7JQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*-LsrEuUNeRp7vBIhcXrbrw.png)

### Matara (30554, 4%), Hambantota (24861, 4%), and Galle (23827, 2%)

![Image](https://cdn-images-1.medium.com/max/800/1*T3MXISQdXzaRrBBy07rAOQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*TXx95YBh7tA_FitEw1aRgw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*-6S-_yW-iUqb2yTI0E-WNA.png)

### Mullaitivu (3584, 4%)

![Image](https://cdn-images-1.medium.com/max/800/1*7YpwkxloykYpybuyQy_8-A.png)

## Caveats

As noted in the Methodology, these computations are approximate. Also, we consider only altitude as a fact. Other factors, like severe floods and rising rivers and lakes, could even submerge significant parts of the island.

#### Article 214 · February 27, 2020

# A Tech Startup Ecosystem in Sri Lanka

### Part II: Can we build a Tech Startup Ecosystem in Sri Lanka?

In Part I (What makes a good tech startup ecosystem?), I defined the "Startup Paradox" as follows:

>>> Ideal startup ecosystems are "nice places". Complete with funding, market reach, connections, talent, experience and knowledge. But invariably, the best startup entrepreneurs tend to come from "not-so-nice places". Often places with economic hardship, war and persecution.

>>> Thus, often a startup-hub is not just one place. But two places: the nice place and the not-so-nice-place. The former is the "official startup hub". While the latter is where many of the entrepreneurs come from.

![Image](https://cdn-images-1.medium.com/max/800/1*qgZZ--S3Hhzq8G3kTwwvPg.png)

The answer to "Can we build a Tech Startup Ecosystem in Sri Lanka?" depends on two questions:

* Can Sri Lanka be a "Nice (enough) Place" to support a Startup Hub?

* Does Sri Lanka have sources of "Not-so-nice Places" that can supply entrepreneurs?

## Question 1: Can Sri Lanka be a "Nice (enough) Place" to support a Startup Hub?

>>> The ideal tech startup ecosystem is a "support system". It has everything a startup needs. Funding is available at a reasonable cost. And it has connections to markets and economies.

>>> Thus, the ideal tech startup ecosystem becomes a magnet for talent. Not only new entrepreneurs looking for their first wins. But also experienced veterans. Seasoned entrepreneurs who have succeeded elsewhere, often many times. "Knowledge organisations" like universities and research groups, join these people. (Part I)

Does Sri Lanka have adequate funding? Do we have access to markets and economies? Do we have decent "knowledge organisations"?

The most common answer I've heard is:

>>> Yes, but not enough. We could do better.

For example, there is a nascent angel investor community in Sri Lanka. Which is good. But too often, startups need to give up a too larger share of their business for a too smaller amount of funding. Hence, not good enough. Similarly, Sri Lanka has access to large markets, especially in South and East Asia. Which is good. But at the same time has various problems with brand, reputation, access and exposure. Hence, again, not good enough. The same probably applies to "Knowledge Organisations" and other factors.

Hence, unsurprisingly, many people have been trying to improve these factors. From "not good enough" to "better". Presumably, these people believe that the answer to "Can Sri Lanka be a "Nice (enough) Place" to support a Startup Hub?" is yes. And they might be right.

But then what is the problem?

The problem is that most people "with the good of Sri Lankan Startups at heart", have over-focussed on "Can Sri Lanka be a "Nice (enough) Place". And completely ignored the second question: "Does Sri Lanka have sources of "Not-so-nice Places" that can supply entrepreneurs?"

## Question 2: Does Sri Lanka have sources of "Not-so-nice Places" that can supply entrepreneurs?

The Israeli Entrepreneur-turned Early Stage Investor (who inspired these articles — see Part I), visited Sri Lanka to invest in, not one startup, but a bucket of startups. The point of a bucket was to "diversify" the portfolio. Since most startups only have a small chance of success, the only wise investment is a diversified one.

The problem with the Sri Lankan Startup Ecosystem was that there weren't enough startups to fill a bucket. An investor could find one or two potentially promising startups. But not enough to build a diverse portfolio. Hence, any investor had one of two options:

* Leave Sri Lanka, and invest somewhere else. Like the Israeli did.

* Pass on the risk to the entrepreneurs, by offering little funding for a lot of shares. Like most Sri Lankan angels do.

Now you might ask, why can't Sri Lankan startups be Part of some bigger bucket. Like Indian startups. This is a fair point. And many investors do invest in Sri Lanka as Part of a larger South Asian or Asian bucket. However, many don't. Because investing in another country involves some non-trivial fixed costs. And the supply in Sri Lanka is a small fraction of giant India.

The cause of this supply problem is that Sri Lanka has no "Not-so-nice-Places". Hence, the solution lies in "building" such places.

## What to do?

In Part I, I gave several examples of "Nice" Startup Hubs, and their corresponding "Not So Nice" sources of entrepreneurs. Let's see what Sri Lanka might learn from these.

### Singapore and Incentives

>>> Singapore's "not-so-niceness" comes from its government. Which is, on paper, democratic. But in many ways autocratic. There is a significant amount of pressure applied to all manner of institutions, from universities to companies, to innovate. Particularly technology. (Part I)

What if the Sri Lankan government creates incentives for universities and companies to drive more innovation? For example, through special funding and other financial incentives?

And what if innovation is engrained into work culture? For example, what if university professors are not evaluated on publications in esoteric journals, but on the FDI their research helps bring in?

Of course, there are pros and cons to these measures. But this is what Singapore does. And it has undoubtedly yielded them some pros.

### Silicon Valley (SV) and Immigration

>>> Silicon value has all the "nice" properties of a startup hub, from almost infinite funding to broad market reach. However, a disproportionate number of successful SV startups have been founded by immigrants from "not-so-nice-places". (Part I)

The main factor that has driven SV's success is that it has been a magnet for global talent. A simple solution to Sri Lanka's entrepreneur (and general labour) shortage would be to make immigration easier. Particularly from South and East Asia.

Now, while SV has been generally positive for the world and its entrepreneurs, it has been hugely detrimental for Native Californians. Many were "priced out" and had to leave their homes for other parts of the country. Similarly, if Indians and Indonesians throng to Colombo and other parts of the country, many "Native" Sri Lankans will suffer. For all sorts of reasons.

Hence, this whole discussion has a general caveat: Do we want a Tech Startup Ecosystem in Sri Lanka? Because it will involve breaking some eggs.

### Beijing/Shanghai and "Internal Immigration"

A large proportion of Colombo's "Startups" founded by rich kids with rich dads. Because being a "founder" is cool. Because you can wear hip clothes. And attend "events". These Pseudo-Startups are a complete waste of time. And I've learnt to avoid these like the plague.

In contrast, a lot of meaningful tech startups have emerged from other parts of the country. Other towns like Galle, Jaffna and Kurunegala. And even suburbs of Colombo — disconnected from the Pseudo-Startup hype.

By "Internal Immigration", I don't mean entrepreneurs coming to Colombo. But investors and marketers exploring other parts of the country. Similarly, the government could consider investing in such places. As well as incentivising their schools and universities.

### Tel-Aviv and "Intimidation"

The "Island Culture" is very much a part of Sri Lanka. Food and shelter are generally (if not necessarily excellent) almost always sufficient. Relaxation and leisure usually take precedence over the stresses of hard work. Weekends and holidays are valued over "work days". Hence, in some ways "Sri Lankan Culture" and "Entrepreneurship" are a contradiction in terms.

In contrast, many Startup Hubs are driven by threats and intimidation. For example, in Part I, I described Tel-Aviv as follows:

>>> Israel's "not-so-niceness" derives, not from poverty, but from geopolitics and history. Israel's neighbours want to blow it off the face of the earth. To this end, they have waged many wars. Both military and "diplomatic". While on the surface Israel might have the "niceness" of a developed country, there is a constant "not-so-nice" threat of destruction. This has driven unparalleled development. Particularly in defence and security technology.

Does Sri Lanka have "threats" that might be a source of motivation?

Several come to mind. But Climate Change is my favourite.

"Hot and Humid" countries like Sri Lanka are particularly vulnerable from rising temperatures. 35 degrees with 100% humidity can be fatal for humans. And such numbers of increasingly more common in many parts of the Island. Rising sea and river levels, and the resulting floods are also a threat to some of the most densely populated areas. Finally, poor air quality is causing a spike in asthma and respiratory disease. Particularly in children.

What if Sri Lanka can become the leader in Climate Change Tech?

## Concluding Thoughts

Should we build a Tech Startup Ecosystem in Sri Lanka?

There are arguments both ways. Just as Native Californians have suffered from Silicon Valley, the construction process will involve breaking some eggs.

The answer might very well be "No".

But if we decide "Yes", then we should set about solving the problem intelligently.

So far, those who have decided yes are only focussing on "Can Sri Lanka be a "Nice (enough) Place" to support a Startup Hub?". And are ignoring "Does Sri Lanka have sources of "Not-so-nice Places" that can supply entrepreneurs?".

Without a good answer to the latter, the pursing the former is a waste of time.

#### Article 215 · February 27, 2020

# The Everything Store

### Part I: What to Store

[The ideas expressed in this article are not original. This is more of a "thinking aloud" exercise. The Computer Scientific theory behind this article can be found here]

Suppose you had a database. Which could store anything. Any piece of data. Any information. How might we design such a store?

Let's start with the "things" it would store.

## Entities

By entity, I mean "things" that have some unchanging identity. Eternally. We could call them "eternities" even.

What other things would we need to store?

## Relationships

Suppose we were to store a news article in the Everything Store. The article could have an author. An organisation might publish it. The article itself might refer to various people and organisations. And finally, there is the article itself. Including its text.

A "relationship" is a collection of entities, united by some meaning. For example, we could say,

>>> "Author X wrote article Y, and organisation Z published it. Article X also referred to politicians P, Q and R, and ministries M and N.".

Note, we can write meaning in different ways. For example,

>>> "Article Y was written by Author X and published by organisation Y".

## Attributes

Finally, entities have characteristics or "attributes" that are not entities themselves. The "text" of the article, for example.

![Image](https://cdn-images-1.medium.com/max/800/1*AGbdoD6z753AbLRnb0dCKQ.png)

#### Article 216 · February 28, 2020

### 2020 Sri Lankan General Election

# Jumpers

### A Brief History of Parliamentary Crossovers

The next Sri Lankan general election will likely be in April or May. Which party will you vote for?

You might reply, "What is a party, but for its politicians? And if all the politicians in a party have recently jumped ship from another party, has that party any integrity? And is that party worth your vote?"

Fair point.

In this article, I try to answer the question, "Which side does a politician actually belong to?" by analyzing "on which side" our MPs have spent their parliamentary tenure.

## The Methodology

My analysis of "Which side does a politician actually belong to?" is based on a Recency Weighted % of Time Spent in Party metric. I look at the time each member as spent loyal to a political party, and weight it by recency. So that more recent time counts for more than time in the distant past.

For simplicity, I define "loyal to a political party" as loyal to the "blue side" (SLFP, PA, UPFA alliances) or the "green side" (UNP, UNF, UNFGG alliances). I've counted the "blue" alliance members who joined the "majority-green" National Government as still "loyal to blue" given that the government was a "National" Government. I've grouped "third" parties that supported blue as blue, and green as green.

"Recency Weighting" works by applying a "half life" of 3 years to the membership. Membership 3 years ago has half the weight of membership today. 6 years ago, has a fourth and so on.

My analysis begins in 2000, until the 2019 presidential election.

## The Results

>>> 

#### Article 217 · March 1, 2020

# The Only Big Match

### A highly sophisticated statistical analysis

"‘Tis the season for Big Matches!"

"Season?", you inquire. "Are there many Big Matches?"

![Image](https://cdn-images-1.medium.com/max/800/1*qSrK_kKIvpv9QHQEhTfWVQ.png)

Of course, you're right to be suspcious. While the misinformed amateurs on Wikipedia claim that Sri Lanka has no less than 34 "Big Matches", this claim has been vociferously denied by the experts.

As one twitter pandit explained, and many commentators agreed:

>>> 

Of course, to the calm, unbiased and rational statistician (like, ahem, yours truly), all this "qualitative" banter is hogwash. Mere half wollies and long hops to be hit for six sans mercy. Only "quantitative quantities" (or "numbers" — if you're an unsophisticated tail-ender) matter. And so one wondered, if there was a statistically significant method one could use to answer the "Is the Battle of the Blues the only Big Match?" question.

Or as Ranjit Fernando might have expertly and originally paraphrased:

>>> "One wondered, Nuwan, if there was a statistically significant method one could use to answer the "Is the Battle of the Blues the only Big Match?" question"

## One's Sophisticated Methodology

All statistical analyses begin with a "Null Hypothesis" and an "Alternative Hypothesis". The "Alternative Hypothesis" is the thing that must be tested. The "Null Hypothesis" is the default position we accept if there is no evidence to accept the "Alternative Hypothesis".

Hence, let's begin with our Null and Alternative Hypotheses:

* Null Hypothesis: "The Battle of the Blues is the only Big Match."

* Alternative Hypothesis: "The Battle of the Blues is not the only Big Match."

Now, let's dig into the data.

### Caps

Our School Matches are cousins of Test Matches. So let's consider the question "Which schools did test-match players attend?" The more test-caps, the better the school.

"Why only Test Cricket?", you ask.

As I said, it's about good genes and breeding. School Matches and Test Matches are family. ODI's and (dare I mention it) T20s are pretend love children. At best. Undeserving of profound contemplations and analyses such as this.

One hundred fifty or so male cricketers have represented Sri Lanka in Test Cricket. These are the schools they graced:

![Image](https://cdn-images-1.medium.com/max/800/1*4l0mLhmt-VrqTTQkK5-0qA.png)

We see the "Battle of the Maroons" in front. Followed by the "Battle of the Saints" and the "Battle of the Blues". Hence, there seems to be some evidence that the "Battle of the Maroons" is a Big Match. Of sorts. And, so might the "Battle of the Saints" — though to a much lesser extent.

### Matches

But you retort, "Berty played only one match. And was out first ball in both innings. Why should that count?"

And you are right. We should give more credit to chaps I mean, Caps who have played more matches.

![Image](https://cdn-images-1.medium.com/max/800/1*SLUR888S_5DYyUplWxUlNw.png)

After this adjustment, the "Battle of the Maroons" is still ahead. But let's not jump to conclusions. For I see you inching towards another appeal.

### Runs

"Offside!", you exclaim, "Amarabandu scored many more runs than Bonipace. Why should every match appearance count equally?"

And again, you've caught me one short. Let's look at the total aggregate test runs by the school.

![Image](https://cdn-images-1.medium.com/max/800/1*p92ZIgUe9DLz3CNG3CPxVw.png)

Again, the Maroons seem to be in front.

### Wickets

But, again, I see you waving your hands.

"I want to refer that!", you exclaim. "The Maroons might be good at batting, but aren't they crap at bowling?"

And of course, you are right again.

![Image](https://cdn-images-1.medium.com/max/800/1*cIxJEBmTDA_Vd3iNXdXEkA.png)

The Maroons are, indeed, utter balls at flinging crap. I mean, utter crap at flinging balls. And with that last-minute referral, they are marooned to the back of the league table.

And so, we are back to square one. Or square leg, as we say in the trade. Our evidences for any other big match, along with the marooned Maroons, are well and truly stumped.

## Concluding Conclusive Conclusions

And so, what are our profound conclusions?

Based on rigorously analysing a wide range of rigorously complex factors, all genuine quantitative quantities (or "numbers" to the plebs), from Caps to Matches to Runs, to Wickets, we must conclude the following:

There is no statistically significant evidence to accept the Alternative Hypothesis. In other words, there is no evidence to say "The Battle of the Blues is not the only Big Match".

And hence, we must accept the Null Hypothesis. Or in other words (according to the statistics),

"The Battle of the Blues is the only Big Match."

Back to the pavilion, one thinks? Eh Ranjit?

#### Article 218 · March 2, 2020

# On Code Reviews

### Some Random Thoughts

## The Most Important Goal of Code Review

The most important goal of code review is not to check if the code is high quality. The most important goal is to check if the code does what it should do. I.e. align with its business purpose. A "perfect" piece of code which doesn't do what it is supposed to is garbage.

Unfortunately, some very senior engineers often don't know their organisation's business purpose. Are not told, or don't want to find out. These usually don't have any choice but to focus on the second most important goal of code review. Often at a high cost.

## On Code Quality

The second most important goal of code review is code quality. Making sure that the code meets some "minimum bar". Code Quality is not absolute. It (again) depends on what the organisation wants to do. For example, if you are building a throw-away prototype, Code Quality is usually a waste of time.

I detail this topic in On Code Quality and discuss three common myths.

## Code is a Communication Channel

The third most important goal of code review is to serve as a communication channel. The code is a sort of "common room" where all coders interact. They learn what other people are doing, and also learn about other people. You can learn a lot about a human's personality, ability and ideas from the code they write.

The more accessible code is to larger parts of the company, the better the communication.

## Code Reviewers are not Automated Testers

Humans should do only human things. I.e. creative things. Everything else, machines should do.

Hence, if changing some code must always run some tests, the reviewer shouldn't need to check-up on this. If the coder changes the code, the tests must run automatically. A machine should do the checking-up. And if the tests fail, the code shouldn't even reach the reviewer.

## Code Reviewers form a Social Network

The more people who can review some code, the more cohesive the engineering organisation. These people form a network who can collaborate on many other things. Like brainstorming and designing new systems. And even non-engineering topics like management and culture.

And just as code reviewers form a social network, the social network forms the code reviewers. A coder is far more likely to ask a friend or acquaintance to review code. And is just as more likely to ask the engineering at the next desk, rather than someone in another building.

[Back in 2009, my manager wrote a script that automatically assigned desks to engineers by looking at who reviewed whose code.]

## Short Reviews are (usually) better reviews

The most efficient reviews are those that review a single logical change. Where a single, short sentence can describe the complete change. Larger changes should be broken down into such changes. Usually hierarchically. The ability to do this efficiently is the hallmark of a sound engineer. Bad engineers almost always make big changes.

## Code Review is mentally intensive

You can't review code (well) in a hurry. Nor if you're tired. Nor if you're distracted with something else.

## Code Review needs reward

The top reason why code review is terrible in many organisations is not because "they don't have a process". It is because code review is not rewarded. If the incentive is created, the process will sort itself out.

What would be a good example of an incentive? There should be both carrots and sticks. Every level of engineer should have some minimum code review expectations. Miss these and you get points dinged. Similarly, reviewing lots of lines of code should be rewarded the same way writing lines of code is reward. And, of course, weighted, but the impact of each line of code.

![Image](https://cdn-images-1.medium.com/max/800/1*pCT1z39epd_K9Pd3bcsYPg.jpeg)

#### Article 219 · March 4, 2020

# The Colombo Bus Map

### On Inaccurate Maps

## "Accurate" Maps

A map is a collection of places. Where a place appears depends on the map. Dehiwala is at the south-west of Colombo. So, on a map of Colombo Dehiwala would appear on the bottom-left corner. If the map is accurate geographically. That is, if the x-y coordinates of places match their longitudes and latitudes. As I said, it depends.

For example, here is a map of Colombo's bus routes. The bus stops are in their geographically correct place:

![Image](https://cdn-images-1.medium.com/max/800/1*wD3zR65N5aegOIsGHgoJBg.png)

But what if you want to draw a different sort of map? What if, say, you don't care about geographical accuracy.

## "Inaccurate" Maps

The previous map might be geographically accurate. But it is also difficult to read. And ugly. The reader doesn't care about geographical accuracy. All they want is to get from A to B. And what routes enable this.

On such a map, places don't match their longitudes and latitudes. Instead, we try to make the bus routes look as simple as possible. If, say, a route heads roughly north to south, a straight line, top to bottom, should represent the route.

On such a map, each location is a member of one or more bus routes. Places with no bus routes we can completely ignore. Each bus route has a shape. And where a location lands depends on where on that shape it appears.

How do we determine the "shape" of a bus route? Here's the paradox. The shape starts with the "real" locations of the places. This gives a rough shape. Once we have the rough shapes of all the routes, we simplify the shapes. As much as we can.

If we redraw* our Colombo Bus Map respecting the "shapes" of the bus routes, we get the following map:

![Image](https://cdn-images-1.medium.com/max/800/1*zaog50Me4y6dOCbqoRDIzg.png)

[* There are several different algorithms for doing this. There is no algorithm which is perfect in every situation. Beauty is highly subjective.]

## Appendix A: Other "Inaccurate" Colombo Bus Maps

I found a few more geographically "inaccurate" Buss Maps of Colombo.

![Image](https://cdn-images-1.medium.com/max/800/1*ZoPKj9lA1_MCaMZb97Zoog.png)

![Image](https://cdn-images-1.medium.com/max/800/1*ecUjSceRPwOowqrp-i5S0w.png)

![Image](https://cdn-images-1.medium.com/max/800/1*IhXO93njjcXYaD1ruy2RXQ.png)

## Appendix B: Updated History

I've updated these maps based off feedback on Twitter and Facebook. Here's a rough update history:

>>> 

>>> 

>>> 

>>> 

>>> 

#### Article 220 · March 5, 2020

# On Advertising

### Democracy and Power

## Sponsored Content

Facebook and Twitter (the companies) are debating how they should treat political content. Especially ahead of the 2020 US Election. "Sponsored" content is particularly sensitive. But also "Organic" material. Especially content bordering on "Fake News".

There is a thin line between "Sponsored" and "Organic". When a post is "Sponsored" or "boosted" on the Facebook Newsfeed, it is "ranked" higher, relative to other non boosted content. "Ranking" is the process that decides what content appears on the feed. It sorts all available content into a queue. And displays the items at the top. "Sponsored" content get to jump the queue. The more advertising dollars spent, the more jumps. In other words, sponsoring biases ranking in favour of sponsored content.

But suppose there was no sponsored content. Facebook and Twitter still need ranking, as there is more content than space to show it. The ranking criteria are complex and evolving. It is a combination of how users engage with the content and its quality. These concepts are subjective. And, depending on your viewpoint, biased. Even without sponsoring.

![Image](https://cdn-images-1.medium.com/max/800/1*ezRNysoTTfIQXhwvE2hkvw.jpeg)

## Unofficial Advertising

I was reading the "business" page of a newspaper. As expected, it had many advertisements. Some well designed, others not so well. These advertisements appeared between "articles".

But something didn't feel right. All the articles were "positive". They all described companies or projects but had only good things to say about them. Another international award. Another goal-beating quarter.

Of course, I should have expected this. The "articles" were also advertisements. I don't know what the deals between the paper and the businesses were. Something like "If you say nice things about us, we will buy more ads?" I don't know. But either way, the paper was creating "bias" in favour of the businesses.

## The "Unbiased" Newspaper

But suppose the newspaper had "integrity", and didn't indulge in quid pro quo ("something for something"), like an online feed with no sponsored content.

As an online feed has ranking, a newspaper has a complex news selection process. From people who access bits and pieces of news. To those who determined what small subset appears on the front page. And the rest of the paper. These people also have their own biases. Political, Social, and Economic.

Hence, as ranking biases a newsfeed, a newspaper's internal process biases its articles. They might say, "We are what we publish". "We publish what we are" is closer to the truth.

## What does "unbiased" mean?

It's not illegal or even unethical for newspapers have biases. The New York Times and the Wall Street Journal have leaned left and right-wing, respectively. But most people consider them intelligent and useful sources of news. But why do we say one leans left, and the other right?

Partly, a set of absolute ideas around left and right "wing-ness". There are some ideas that the NYT will always suppose. Others that the WSJ will. But "wing-ness" is also tied in the present content. If all newspapers were "left-wing" then we won't call out the NYT as left-wing.

The present contexts depend on the views of the world. At the present moment. Compared to the 19th century, all newspapers were more "left-wing" in the 20th century. In the 21st century, thus far, there is more polarisation, while the "average wing-ness" hasn't changed. The left-wings are more left-wing. The rights more right.

But my point is this. "Bias" is always relative to some baseline. The present context determines this baseline.

And what determines the present context?

## Bias and Power

In the last decade, we have seen the bizarre phenomenon of YouTube millionaires. People whose videos go viral, transforming them into instant celebrities. Along with the millions of advertising dollars that follow. But YouTube (and other social media) millionaires are rare. For every success, a million failures exist. With almost identical videos and histories. Winners and losers of the YouTube lottery.

Despite their humble beginnings, these millionaires have an enormous influence on the internet. They "influence" what people do, think and even feel. Most importantly, they influence the contextual baseline that determines bias.

While some win power in a lottery, others inherit power. Others (claim to) win power by merit, hard-work or skill. Like YouTube millionaires, other millionaires and billionaires also define the baseline of bias. In Silicon Valley, most of the billionaires are "left-wing". And the baseline is also so.

## Bias and Democracy

Ideally, democracy is a "One person, one vote" system. And in spirit, this "vote" is not only a vote but a unit of power. Every human has an equal amount of power. This power applies to thinking, speaking and doing. For example, in an ideal democracy, everyone should have the same enlightenment and education. They should have the same freedom of expression. And they should have the same freedom to act.

The "bias" we've discussed in this article, erodes the innate equity of democracy. While many countries boast the token "one person, one vote", the biases of power skews history in favour of a few.

I'm not arguing that inequity is a bad thing. Or democracy is a good thing. I'm pointing out that the two are contradictory. Freedom is not possible in a billionaire owned world.

## On Advertising

Advertising in general and political advertising, in particular, have a bad reputation. But they are not the disease, but a symptom. The virus (if I may call it that) is the bias of power. And the symptom is not only advertising but everything we read, think and feel. They are all biased by power.

Again, I'm not arguing that something is good or bad. I'm pointing out what is what is.

[The author worked on the Facebook Ads Engineering team for over eight years, as a Software Engineer and Engineering Manager]

#### Article 221 · March 5, 2020

# On Decisions and Impact

### Reflections on Performance Reviews

January, February and March are "Performance Review Season" in many companies. For bad companies, performance reviews are a mundane formality. All employees get a raise based on some arbitrary percentage. Usually not much.

For good companies, however, it is a time of deep reflection. "Did we meet expectations? Perhaps, we exceeded expectations? Maybe we didn't meet some expectations?"

## Impact

At good companies, these questions are discussed and debated, at and for every level of the company, from the company as a whole to its teams, and every employee. What the company accomplished (or "impact") is the sum of its organizations, which are the sum of its teams. And ultimately, people.

Conversely, an employees impact must be a subset of the companies impact. If the employee did something and this something is not such a subset, then that work is useless. Sadly, many employees in many companies, do a lot of useless work.

Many companies, including many good ones, anchor performance reviews on impact. "What was the impact X was supposed to make? Did X meet that?" Where X is the company as a whole, a team or a person.

## The Problem with Impact

Employees don't spend their time making impact. They spend their time making decisions. A "good decision" is one which has the best chance of yielding most impact, given the information available to make the decision. In other words, good decision making is a form of forecasting. The best decisions produce the best forecastable future.

The problem with forecasting and probability, in general, is luck. A good decision could lead to bad impact. In other words, an employee could make all the right decisions, but still, end up with the wrong impact. Just because they got unlucky. The opposite is worse. When bad decisions lead to good outcomes.

Even if the decisions lead to impact, it won't lead to impact now. This is the other problem. Usually, there is a significant lag between when decisions sow, and impact reaps.

[My former employer Facebook had performance reviews every six months. Hence, there was an incentive to pick projects which yielded impact on six months or less. This led to a shying away from longer-term projects, despite many such having more impact potential. Our fix was to endow long-term projects with shorter-term milestones. Where the milestone was a proxy for future impact. Sadly, these milestones were never valued as much as the "final impact".]

## The Solution

The solution to this problem is to stop valuing impact. And instead, evaluating decisions. Decision-based performance measurement (DBPM) must replace impact based performance measurement (IBPM). The latter, asks "What past decisions caused this present impact?" The former asks "What present decisions will cause future impact?"

![Image](https://cdn-images-1.medium.com/max/800/1*ozyVeINZf3PwAKuyFoD1Zg.png)

IBPM relies on correlation. The employee working on a project correlates with the project's impact. There is no (statistically significant) explanation on how the employee caused the impact. DBPM, on the other hand, relies on causation. When we try to determine if a decision was good, we build a causal theory on how it might cause a good outcome.

You might argue that this process of "determining causality" is complicated. It might be almost impossible to say which decision is the best option. This is precisely my point about luck. If two employees made one "impossible to determine" decision, and the other made another, and one succeeded and the other failed, why reward one and not the other?

## On Calibrations

[Performance Review Season is a hectic time for managers. At Facebook, we spent a lot of time with other managers in "calibration meetings". In a "calibration" different managers discuss the performance of their reports. The goal is to make sure that everyone has the same "baseline" on what "meeting expectation" means. A calibration is a detailed review of the past from macro-level dashboards with top-line metrics, to micro-level lines of individual code.]

Managers build "histories" on how the employee's decisions of the past "caused" the impact of the present. This process can have significant "cherry-picking". When there is a good impact, the manager can highlight employees' good decisions and hide bad. Asymmetrically, when there is lousy impact, the manager can ascribe the present to bad luck. Not bad decisions.

To be clear, good managers seldom "cherry-pick". They are as good at drawing connections between bad decisions and bad impact, as they are with good. But good managers are rare. There is also a breed of bad manager that "throws in a few bad apples". Such a manager will, from time to time, give a few examples of bad decisions, to avoid "Tommy only sings praise"-type accusations.

## How not to "Predict the Past"

But my point is not about good or bad managers. It's about the process. Even for good managers, this process of "predicting the past" is arduous. When you predict the future, you might be wrong. When you predict the past, you might certainly be wrong. But with IBPM, this is unavoidable.

DBPM solves "predicting the past" by avoiding it. There could still be calibrations. But instead of discussing the correlation between good things done and good impact, managers would purely discuss the goodness of decisions. Focus would shift from a few points of time where impact reaped, too many points of time where decisions sowed.

A DBPM calibration would consist of presenting an employee's decisions, and how good they were, without the benefit of hindsight. Such a presentation would need a lot of "real-time" present management from the manager. They would need to know what decisions the employee made. Daily.

## Contradictions

Despite what I've said, IBPM is more popular than DBPM. Why? There have been many studies on the subject. The most common reason goes something like this:

"With IBPM, it was possible to differentiate "good" employees and "bad". There was quite a lot of "signal" to do this. With DBPM, unfortunately, everyone looked much the same. How their decisions would cause future impact was difficult to predict, so everyone got, roughly, the same evaluation. Hence, employees didn't have incentives to work harder than others. And the company stagnated."

Reflecting on these studies let me to an interesting thought. What the following were true?

The "differentiation" IBPM causes leads to more activity. Not good activity, but activity none-the-less. The company, one way or the other, does not stagnate. The ones that are lucky enough to have "good activity" become "good companies". We don't hear of the ones that don't.

So what if IBPM works because we can only see the companies for which IBPM has succeeded? What if "An ecosystem of IBPM companies" worked better than "An ecosystem of DBPM companies"? Because the latter has become stagnant?

Then, we could conclude the following:

* DBPM companies have smarter employees. IBPM companies have "lucky" employees.

* DBPM companies are more likely to succeed than IBPM companies. DBPM companies owe their success to skill. IBPMs to luck.

* But IBPM company ecosystems are more likely to succeed than DBPM company ecosystems!!!

## Breaking the Contradiction

Can a company have both the cake and eat it? Can we have the benefits of both DBPM and IBPM?

It should be possible, if you accept that the benefit of IBPM is purely motivational. Being better than our peers is a fundamental social need. Can something else replace this motivation?

There are many right answers to this question. But the main barrier to DBPM is not the lack of one but the popularity of IBPM. So many people and companies believe that this system brings them success. And exclude the role luck might have played in it. Sooner or later, luck will run out. But then, they will the next IBPM company will replace then.

Hence, the bigger question is, "How do you convince people that DBPM is better? And IBPM will eventually lead to doom?"

But I've already tried to do that in this article. So if you are not convinced, maybe you could reread the article?

#### Article 222 · March 10, 2020

# The Biggest Problem in the Tech Industry

### And how to fix it

## A-Grade Software Engineers (SWEs)

What is the biggest problem in tech today?

The lack of creative products? Privacy? A few large corporations controlling the show?

All of these are good answers. You might favour one over another depending on your circumstances.

My "circumstances" have involved a lot of recruiting. I've spent much of the last two years hiring Software Engineers (SWEs). It has been tough. I don't mean any-ol' coder. They are a dime a dozen. I mean recruiting "A-Grade" SWEs:

>>> "[A-Grade] candidates have, besides professional skills and social, behavioural and cultural skills, the right mindset and motivation to work well in an organisation" — On Software Engineers

Hence, relative to my circumstances, the biggest problem is recruiting "A-Grade" SWEs. The supply is low. The demand (particularly from "A-Grade" software companies) is high.

Am I talking about Sri Lanka? Or Silicon Valley? Well, both. The problem is global. For the sake of focus and clarify, I'm going to focus on Sri Lanka. But the ideas and implications extend worldwide.

How do we fix the shortage?

Again, there are many good answers. We need more kids learning to code. More investment in tech education. And more tech graduates from universities.

But what about this answer?

"What if we remove the barriers for women becoming tech professionals?"

## Barriers? What barriers?

Is there any data supporting this "barriers" theory?

Good numbers are hard to come by. Especially for Sri Lanka. There have been few surveys, with few participating companies. Definitions are vague, and few differentiate between A-Grade SWEs and lower quality candidates.

But extrapolating several sources, I came up with this narrative. See this more as direction and descriptive, and less as rigorous and quantitative.

* Half of O.Level students are female; a much smaller proportion consider studies in tech.

* Female undergraduates in tech fields are far more likely not to enter the tech job market. Only 20% of Junior SWEs are female.

* Female Junior SWEs are less likely to become Mid-Level SWEs. Only 10% of Mid-Level SWEs are female.

* Female Mid-Level SWEs are far less likely to become Senior SWEs. Only 5% of Senior-Level SWEs are female.

![Image](https://cdn-images-1.medium.com/max/800/1*v_7j1WcRhTO3VSjr_Qi80A.png)

Hence, at every step of the pipeline, female potential drops out. Again, remember my caveat on the quality of the data. But this is not hard to verify. Walk into any Software Company, and what do you see? Almost only males. Hence, barriers must exist.

So, how do we remove the barriers? Let's start by analysing the different steps in the pipeline.

## Step 1: Secondary School to University

Female students are less likely to pick the "Physical Science" or "Maths" A. level stream than males. Why?

Ignorance? Many parents and teachers feel that girls are less suited for tech and mathematics. Compared to boys. Hence, they encourage girls to pursue other fields instead of Physical Science. This prejudice shrinks female demand for the Physical Sciences. As a result, girls' schools have fewer teachers, classes and facilities. The lack of facilities leads fewer girls picking the physical sciences. Reinforcing the initial prejudice: "girls are less suited for tech and mathematics". The cycle continues.

Why do parents and teachers hold these views?

Data is scarce and theories are vague. One theory is that "Engineering" is a "man's" field. Like a Steam Engine "Engineer" shovelling coal into a furnace. While women (supposedly) prefer "softer" and creative fields, now, I don't see why women shouldn't shovel coal. But more to the point, professions don't get much "softer" than caressing keyboards and creating "soft"-ware. And few professions are more creative. Writing code is a sort of alchemy. Where one creates wondrous things out of nothing.

What the profession lacks is not softness or creativity. What it lacks is brand. The SWE Industry should lead the battle against this ignorance. Female leaders could evangelise tech in their former schools. Customised plans should target parents, teaches, and students. These plans should target the tail-end of O. Levels, since it is here that students make vital decisions.

In parallel, we should lobby for more maths teachers and classes in girls' schools.

## Step 2: University to Junior SWEs

Why do female tech graduates shy away from the industry?

The problem is not "dropping out" of university. Tech "Drop out" rates in Sri Lanka are low for both sexes. But while almost all-male graduates enter the SWE job market, half of females don't.

The problem is the SWE profession itself. It is very much a "Boys Club". The vibe of the tech company office resembles a classroom in a boys' school. The few women tend to congregate in a corner, trying best to avoid the noise and "locker room" banter. Even the term "Hacker" is far more "male" than, say, Doctor or Lawyer.

"Work Longer, Not Smarter" is the philosophy of many Junior SWE roles. Often middle-level managers measure new SWEs by how late they stay in the office. Code committed at two in the morning scores a lot of points. Tech companies don't realise the cost of this lack of Work-Life balance. For males, it reduces productivity and future potential. For females, it often wholly discourages candidates from taking the job to start with. Why pick a job where you have no life when there are plenty of better jobs?

Some claim that female graduates prefer academia to SWE roles. But academia is merely another particular case of another "better job".

Tech Companies should move away from "Work Longer, Not Smarter" for the sake of both males and females. In the medium to long term, it serves no one. In the short term, it might be a cheap way of completing BPO projects, that involve the mechanical translation of "requirements" into code. But those days are over. To succeed, tech companies must exploit human creativity, not brute-force (mostly male) labour. And that is all about working smarter. You can't be creative if you don't have a life or lack sleep.

Tech has a diversity problem globally, which reflects in the one-sided products it builds. Diversity is not just a problem across sexes, but within sexes as well. Male SWEs tend to skew to "specialists" with little knowledge and interests outside their field. Many lack essential communication and social skills. Working with such "Dilberts" is, to put it bluntly, boring. This culture of bores discourages others (including "generalist" males). It also degrades the quality of software development. Hence, diversity is not a fad. The lack of it has real costs.

The obvious way for tech to fix a big portion of its diversity problem is to hire more female SWEs. This is not about lowering the bar. But being smarter about recruiting. For example, if a team or company has at least one woman, other women are far more likely to join that group. Hence, all teams should have a "critical goal" of reaching that "one woman critical mass". Similarly, when women conduct interviews, other women tend to perform better. And are far more likely to join. New SWEs get deep impressions of the company from interviews. The list of "fixes" is endless.

Parallel to these structural changes, tech must improve its image and brand. Particularly within universities. Female undergraduates need female role models. Universities should have more female lecturers and guest lectures from female industry leaders.

## Step 3: Junior SWEs to Mid-Level SWEs

After a few years of experience, the entry-level SWE acquires various "non-academic" skills. They gain more independence; the ability to do things without being told. They acquire an ability to answer questions which are not asked: "What new systems and products should be built?". They increase the size of the "big picture" that they see. Hence, mid-level SWEs move beyond mere technical skill and competence. They understand products, business and people better.

While a large proportion of male junior SWEs reach the mid-level, more than half of women drop off. The leading cause is, again, Work-Life Balance. Especially around marraige and maternity.

It is sickening how so many "industry leaders" have Victorian views: "We don't want to hire women, because they get married and have babies". And I hear it often, even in (supposedly) 21st-century tech companies.

These prejudices are, at best, unscientific. Consider a woman's career. Suppose it spans from age 25 to 55. Suppose the woman has two children. And that six months of maternity leave follows each birth. That is one year in 30 or 3.3%. Is that such a significant loss? How does this compare to vacation and sick leave?

The "problem" with maternity is that it is conspicuous. And being away for six months of baby leave is more visible than goofing-off on a Monday morning due to heavy drinking with the "boys" the previous night. Alcohol is considered a "positive" in many tech companies, and a massive part of "culture" and "team bonding". The same "leaders" who complain about women having babies are happy to overlook male drunken idleness.

The benefits of better Work-Life balance, I've already explained. Tech companies should also help balance the burden of raising children. Paternity leave is an obvious step in this direction.

But industry leaders should begin with themselves. And change their Victorian minds.

## Step 4: Mid-Level SWEs to Senior SWEs

Senior SWEs influence the long term direction of tech companies, and also the industry as a whole. Roles diverge into areas involving people management, product and business development. In Sri Lanka, there is a severe shortage of such people. Both male and female. The root cause is the lack of diversity at lower SWE levels. Note, this includes "intra-male" diversity. Too many male SWEs are "Dilberts".

While there are few male Senior-SWEs, there are even fewer females. A few dozen across Sri Lanka, maybe. The shortage influences the whole pipeline. Female SWE candidates leave the profession for the lack of role models and favourable influence. Conversely, the lack of middle-level female SWEs causes a shortage of senior female SWEs. Another vicious cycle ensues.

Senior career progress hinges on a professional network. And sadly, Sri Lanka's professional network is an "Old Boys' Network". With every connotation of that phrase. From school loyalties to drinking buddies. Not only in tech, but across the board.

Both "ends" of the problem needs solving. More junior and middle-level female SWEs graduating to the senior level will help. And the few senior females SWEs and leaders should continue to strengthen their networks, and help grow the pipeline.

## Concluding Clarifications and Confessions

Some consider diversity in general, and women's empowerment in particular, a "fashion". And some outwardly display interest for professional acceptance or other gains.

My goal in writing this article is not to join the fashion show. My motivations are entirely and sincerely selfish. My work suffers from the lack of SWEs (both male and female, at all levels). An obvious cure to this pain is to remove the barriers that women face.

Like recruiting high-quality SWEs, the going has been tough. Few people believe there is a problem. Those who agree that there is a problem don't know what to do. Those who know what to do, don't want to do anything.

Hopefully, this will change. Maybe someone reading this article will help?

...

[Thanks Kanchana Ambagahawita for proof-reading this article, and providing many valuable comments and insights]

#### Article 223 · March 10, 2020

# The Uncertainty Principle

### Of Knowledge

## Chandrika the President

>>> Doctor: "Who is our president?"Patient: "Chandrika Kumaratunge"Doctor: "What year is it?"Patient: "1995"

This conversation would have been unexceptional in 1995. But it wasn't had in 1995. It happened a few weeks ago. And the president is Gotabaya Rajapaksa.

The patient had recently had a brain injury, which wiped out 25 years of her memory. She believed it was 2005. She was sincere and convinced.

Have you suffered from an episode like this? You think not? Let me jog your memory with an example. Do you remember this conversation?

## Tommy the Good

>>> Me: Is Tommy a good accountant? You: Yes! He has a spotless record. Competent, honest and discrete. Me: But he could spoil his record in the future, right? If he, for example, gets involved in some scandal? You: But his record now is spotless. Me: How long have you known him?You: We go way back. We were at school together. Best friends. Until he went to the US. About 25 years ago. Me: Why did he move back to Sri Lanka? You: I don't know. He wanted to be closer to family?Me: So you didn't hear about the Aurus? You: What's Aurus?Me: The reason Tommy lost his accountants' licence?

What do these two episodes have in common? The principle is the same "knowledge loss". A severe car accident caused the first. Ignorance caused the second. In both cases, both people lost 25 years of knowledge

But who exactly is the President? Gotabaya Rajapaksa or Chandrika Kumaratunga? Well, it depends. If you clarify, "The President, now", then it would be GR. But without this clarification, the question has no precise answer.

You might say that I'm quibbling about semantics. And of course, you are right. But with most questions, I'd be right to quibble. Because when we ask questions, we don't know what we are asking. And when I ask you a question, you might answer a different question.

For example, when I asked "Is Tommy a good accountant?" you answered the question "Was Tommy a good accountant 25 years ago?". As the patient answered the question, "Who was the President 25 years ago?"

So, is Tommy a "good accountant". Well, that depends. 25 years ago, he seemed to have been a good one. Then he blotted is copybook in New York, and became a "bad accountant". And now he's back in Sri Lanka, back to being a "good accountant" (at least by local reputation) it seems.

The answer is precise at single points of time. Like 25 years ago, or now. But considering Tommy's entire career, the answer various and ambiguous.

## Conclusions: Adolf the Socialist

Let me conclude with Hitler.

>>> The "Libertarian": Socialism is the worst. Me: What are some good examples of socialism? The "L": Hitler. He was a socialist. Do you want the US to be like Nazi Germany?

There are two underlying questions: "Is socialism a bad thing?" and a more profound question "What is socialism?"

The "L" believed that socialism was bad. But his view was also based on a specific and narrow definition of socialism. He was either ignorant or was "blocking out" less unfavourable examples of socialism.

What has Hitler got to do with car accidents and dodgy accountants?

If you want to say something "certain", you have no choice but to restrict yourself to a narrow context. If your definition of socialism is Hitler's national socialism, then socialism is terrible. If you judged him on his record 25 years ago, then Tommy is a good accountant. If it is 1995, then Chandrika Kumaratunge is the president.

If you want to see a broader context, then what you say is likely to be various, ambiguous and uncertain. You will use "that depends", clarifying definitions, nuance and invoke randomness.

Or in other words:

>>> The broader one's knowledge, the less certain one is. One cannot have both broad knowledge and certainty.

Or as MacGyver said:

>>> "Only a fool is sure of anything; a wise man keeps on guessing."

![Image](https://cdn-images-1.medium.com/max/800/1*DneRsuwZVPuHCCKliaKIbQ.jpeg)

#### Article 224 · March 11, 2020

# How to work in your sleep

### Some personal reflections

Disclaimer: I'm not a physician, psychologist or sleep expert. I'm writing about something that has worked for me. It might work for you. Then again, it might not. Either way, I'd appreciate your comments and feedback. The book Why We Sleep: The New Science of Sleep and Dreams, by neuroscientist and sleep researcher, Matthew Walker, has inspired and influenced this article.

## The Machine

Our brains are powerful machines. We use it all the time. For all manner of tasks. From folding clothes to writing operas.

Sleep comes in two forms:

* NREM Sleep or "Non-Rapid Eye Movement" Sleep. Where one is "dead to the world" and where one goes to sleep and wakes up eight hours later, as if was the next moment.

* "Rapid Eye Movement" or REM sleep. Where one dreams. While both mind and body are "shut down" during NREM sleep, the mind is awake during REM sleep. That is why one dreams.

![Image](https://cdn-images-1.medium.com/max/800/1*NIrwOyybHIQld8I-Zr989A.jpeg)

Dreams are subconscious meanderings. Where your thoughts bounce off partial and disconnected ideas. It is also where "creativity" happens. When disconnected ideas "have sex" to spawn new ideas. If you think about it, familiar people, places and concepts make-up dreams. But these people, places and concepts combine in strange and fascinating ways. Which is what makes dreams interesting.

Can we get dreams and other subconscious activities to "work for us"? We can!

## Uploading Problems to the Machine

Think of the most exciting and creative problems you need to solve. If you are a Software Engineer, it might be, "What is the most efficient way to design that architecture?". If you are a UEX designer, "What would the most simple and intuitive UI look like?". If you are a political strategist, "How might we win over demographic X?". Your problem depends on your work. You know best.

Not less than two hours before you go to sleep, find some way of reflecting on the tasks. At the end of the "workday", I write down a list of the most fascinating unsolved problems. Another could be going through them in memory. Another could be speaking them out loud: "How do I design a better messaging UI?"

Use whatever that is most natural. But you mustn't overthink. Conscious thinking is a conscious task. And conscious tasks tend to usurp mental energy for subconscious tasks. If you overthink, you might spend the rest of the day thinking about them, and this might even disrupt your sleep.

## Running the Machine

How should you run the machine? Try to maximise the amount of REM sleep.

To do this, first, try to optimise sleep in general. Make sure that your sleeping arrangements are comfortable. Cool, silent and dark. A fixed set of sleeping hours also helps.

Avoid alcohol and caffeine. While sometimes encouraging NREM sleep, they tend to disturb REM sleep. Some foods, like milk, tend to promote REM sleep. A cup of hot milk before bed is ideal.

## Downloading Solutions from the Machine

You can't copy the solutions to a pen-drive, as you could from a conventional computer. Or photocopy them, as you would do from a book. You need to give the machine "some space and time". To download the solutions from your subconscious to your conscious memory.

I try to minimise "conscious thinking" during the first two hours after I wake. I meditate for about 45 minutes. Meditation consists of "observing without thinking" or "being without doing". And helps, with the downloading process. I try to do some "mundane" tasks that don't need conscious brainpower. Like arranging dishes drying in the kitchen overnight. Or tidying-up the house. Or going for a walk. Jeff Bezos calls this "pottering around".

## Does it work?

Be patient. Unlike the conscious mind that can "obey orders", the subconscious mind takes its own time. The machine might solve the problems you upload today, in a week or month.

The subconscious mind also tends to do things its own way. You might upload one problem, but the solution is for a different problem. It might be a solution to a "better" problem.

It works for me. That's the only "evidence" I have.

Try it out and see if it works for you.

#### Article 225 · March 12, 2020

# The IC-Manager Spectrum

### Should an Engineering Manager write code?

## In theory

Software Engineering organizations have two types of employees: Engineering Managers and Individual Contributors (ICs).

ICs contribute to the company through their (own individual) effort. They design and implement systems; usually, by writing code.

Managers contribute through "helping others contribute". At Facebook [where I was both an IC and an Engineering Manager for eight-plus years], managers were supposed to support their managees (or reports), in four ways:

* Provide Context. Help ICs understand how what they do connects to the "Big Picture".

* Set Focus. Help ICs focus on what is essential and ignore the rest.

* Drive Impact. Help ICs translate what they do to top-line impact.

* Cultivate Growth. Help ICs grow and progress

[See Mantras for Managers by colleague and ex-Facebook Engineering Manager John Lusty, for more details on these "four ways"]

A manager's "impact" must be "incremental". If the company credits a manager for all their ICs impact (as well as the ICs), there will be "double-counting". Instead, the company rewards managers for the "incremental impact" their ICs make, compared to had the manager not existed.

Hence, managers needed one set of skills; ICs another. At least in theory.

## In practice

There is no such thing as a 100% manager or a 100% IC. In practice, most people are somewhere in between.

If a software engineer, mentors another, they are "managing" to some extent. Similarly, if a manager spends time designing a system or even writing code, they are "ICing".

As an IC gains experience, they tend to do more "managery" tasks, like mentoring. Facebook evaluated IC Engineers across three dimensions: 1) Technical; 2) Product; and 3) People. The "People" dimension had a substantial "management" component. The "weights" of the dimensions changed with the ICs experience. While a junior Engineer's "People Dimension" might weigh 10%, it could be 50% or more for a senior engineer.

These "dimensions" reflected the diversity of expectations. The same applied for Managers.

## How to make this work

Hence, in practice, there is a spectrum; from a "pure" IC to a "pure" manager. Whether or not the spectrum is effective, depends on how the company is organized and managed.

### 1. Structure

Definitions of roles and levels must be consistent with an IC-Manager spectrum.

In many organizations, managers are "above" ICs. ICs, once they reach a certain level, are "promoted" to management. In such an organization, an IC could take on some manager tasks, especially if they "aspire to management". On the other hand, a manager doing IC work might be considered "beneath them". This also resulted in senior ICs who could not progress further. These "dead-end ICs" tended to stagnate or leave the organization.

A better structure is one where ICs and managers are equal in level. For example, Facebook had the following structure. The company promoted ICs to more senior ICs, and managers to more senior managers, it never "promoted" ICs to management. When an IC became a manager (and vice versa), the move was known as a "transition".

![Image](https://cdn-images-1.medium.com/max/800/1*tgXYbkIG6Hxk9yKA2FY0Cw.png)

### 2. Expectations

Setting the right expectation is critical. Managers at Facebook had an explicit "agreement" with their managers, about the IC-Manager Balance. Their performance was measured relative to that expectation.

While at Facebook, I moved back and forth through the spectrum: I was a 100% IC, a 100% Manager, a ~50% IC (with 50% "managing") and a ~50% Manager (with 50% individual contributing); and a multitude of shades in-between.

### 3. Roles

It is easier to be something if that something has a name.

Is a 50% manager/50% IC a "manager" or an "IC"?

While the company would expect such an employee to make the same aggregate impact as a manager or IC at the same level, their impact purely as a manager, or IC would fall short of a 100% manager, or a 100% IC. Hence, they will be undervalued if they are judged relative to a "pure" role.

At Facebook, these roles were known as "IC-Manager-Hybrid". Expectations were accordingly set, and performance was relatively measured.

## Concluding Thoughts

The term "Manager" has some historical baggage. "ICs" were associated with the "working class", and consigned to that lowly position for eternity. Managers were an elite, were often parachuted in from a different pool of candidates, often with different backgrounds and no "technical" qualifications. This historical class structure still prevails in many companies.

Tech Companies (or at least the better Tech Companies), on the other hand, have diverged from this model. Instead of a class system, status depends on impact. Hence, an IC making more impact than a manager holds a higher position.

It probably boils down to what you value more. History appreciated a status quo; the modern tech company values impact.

Finally, should an engineering manager write code?

The depends on two factors:

* Can the engineering manager write code? Any EM worth their salt should be able to write excellent code.

* Does the company support it? The better tech companies do. This article might help those who don't but want to.

#### Article 226 · March 13, 2020

# Science, Social "Science", and Statistics

### On Theories, Hypothesis Testing and the Future of Social Science

## Science

Science is a collection of interconnected theories and facts.

A fact is an observation known to be true. For example, "the sun rose from the east today".

A theory generalizes a set of facts. For example, after observing the sun rising from the east, every day for several years, a caveman might generalize, "the sun rises from the east".

## Falsification

A theory assumes that what we know for observed facts, must be valid for unobserved situations. For example, "the sun rises from the east" implies "the sun will rise from the east, tomorrow".

If an unobserved situation contradicts a theory in the future, we say that the "theory is falsified", or is shown to be false. For example, if the sun explodes sometime today.

Hence, a theory can never be proved correct. It can only be proved false.

## "Back-up" Connections

Why do we accept a theory? Like "the sun rises from the east"? Is it only based on the many observations of the sun rising from the east?

Not quite. This theory connects to other theories. Like "the earth rotates around its axis". "Because the earth rotates around its axis" is a reasonable answer to the question, "Why does the sunrise from the east?"

Hence, theories "back-up" other theories. Which further back-up theories. But this still doesn't make the theory "true". Because the "back-up" theories are also theories. Which might be falsified by future observations.

On the other hand, the "back-up" makes a theory a "better theory". Or at least it feels that way, intuitively.

But then, what exactly is a "better theory"?

## The "perfect" theory

The "perfect" theory is one which can be derived entirely from facts, without generalization.

For example, suppose you "observe" that "a number that is a multiple of four and six, seems to be a multiple of 12" often. And you conclude "any number that is a multiple of four and six, is a multiple of 12". This "theory" is "ideal" because you can "prove it mathematically" from "first principles" or "axioms".

"Perfect" theories like this are restricted to "formal sciences" like mathematics and statistics. As the subject increases in complexity, from mathematics to physics to chemistry to biology, and so on, it becomes harder and hard to build a theory from first principles.

Even in physics, there have been many instances where we thought we had the "perfect" theory, only for one observation to falsify it. The most famous example is probably Newton's laws of motion, which were believed to be "perfect" until Quantum Theory falsified them several centuries later.

Strictly speaking, there are no "perfect theories" even in mathematics, because the "first principles" or "axioms" are not pure facts. For example, in Euclidean (or "classical") geometry, we assume that two parallel lines never meet. Riemannian geometry does not assume this. Even "1 + 1 = 2" is based on a set of axioms in set theory, upon which number theory and arithmetic are built.

Axioms can be dangerous, especially when we force ourselves (and others) to accept a flimsy theory, as an axiom.

## A "not bad" theory

While Quantum Theory proved Newton "wrong", his Laws of Motion are still useful. Because they are a "good enough" approximation in most situations. For example, if you're an engineer computing a car's braking distance, Newton is more than sufficient.

Hence, a theory need not be "perfect". It only needs to be good enough. Or possibly, "not bad".

How to we test if a theory is "not bad" or not?

We could compare a theory to a "bad theory", and if the "bad theory" is as good, we could conclude that it is not a "not bad" theory.

How do we do this? Statistics provides an excellent technique.

## Hypothesis Testing

Statistical Hypothesis testing consists of two hypotheses: The "Null Hypothesis" and the "Alternative Hypothesis". The latter is the theory you want to test. The former is the "bad theory" for comparison.

I was talking to an Economist about a particular development strategy X. "Why does it work?", I asked. The Econ explained that ten countries adopted it, and seven countries observed significant development. Let's use this episode as a "case study".

The "theory" here is:

>>> "X results in development".

And that will be our "Alternative Hypothesis". Let me propose the following "bad" theory, as the "Null Hypothesis":

>>> Development has nothing to do with X. Instead, God says, "I'm going to toss a fair coin. Once per country. HEADS, and I grant development. TAILS and I grant no development"

Alternatively, if you are an atheist, or believe that God doesn't toss,

>>> "Development has nothing to do with X. Each country has a 50% chance of achieving development."

This type of "random" bad theory, is widespread in statistics

How do we test if the "bad theory" is as good as our theory? Simple, we see if the bad theory might explain the observations. Or "what is the chance that the coin-tossing God might explain the 7/10 outcomes?"

A simple calculation will tell you that with the "bad theory", the probability of 7 or more countries developing is about 17%. Hence, we see that the "bad theory" explains the observations.

![Image](https://cdn-images-1.medium.com/max/800/1*aivxMDPNXtOWFsaUxR9PVQ.png)

But is 17% enough?

In practice, we use much smaller numbers like 1%, 5% or 10%. The smaller the number, the more we favour the "Null Hypothesis" or "bad theory". And the smaller the number, the more "not bad" the "Alternative Hypothesis" is. We refer to this limit as the "Significance" of the Test. Alternatively, we might report the (100% — Significance), known as the "Confidence" of the test. 5% Significance is equivalent to 95% Confidence.

The Econ's theory won't pass a 5% or 10% Test.

## "Statistics is too strict."

But you might say, "It would pass a 20% test. Wouldn't it? Was our 5% or 10% bar too strict?"

Suppose we lived in 1900. And suppose we were trying to test Newton's Laws of Motion. We run 100 experiments, and all return the correct result. At what significance would this series of experiments pass a statistical test?

If we use our "random bad test" as the "Null Hypothesis", the significance is the probability of getting 100,000 heads while tossing a coin. This probability is "zero point zero thirty-one times followed by a seven" or almost zero.

Hence, a properly good theory will not only pass a 5% test; it will pass a much stricter test.

## "Bad" is relative

"Newtonian Physics might demand an almost zero significance. But isn't 17% sufficient for Economics?", you counter.

And you might be right. Different fields seem to have different opinions and on "significance". We might even "classify" academic fields on his basis:

* Formal Sciences: 0%

* Physics: Almost 0%

* Chemistry: <1%

* Biology: <5%

* Medicine: <10%

* Social "Sciences": >10%

![Image](https://cdn-images-1.medium.com/max/800/1*aG3Jb89V0cQ0KrOrAKo-3Q.jpeg)

## An Alternative to Social "Science"

You'd notice that I don't list the "humanities" above. This is because the humanities don't propound "scientific" theories. When they do propose theories, they are descriptive and qualitative. They seldom involve the "scientific method" and "falsification". Theories in humanities have some aspect of generalization, but these are more summaries, as opposed to general theories.

Now, this lack of "science" doesn't make the humanities less useful. They are far more helpful because they are intellectually honest. They don't make false claims.

The Social Sciences also had their roots in sociology, which was a part of the humanities, and followed the tradition of "non-scientific" study.

Sadly, starting in the 19th century, and possibly driven by envy for the newly emergent Chemistry and Physics, sociologists rebranded as social "science". The rebranding reached new heights when in the early 20th century Economists annotated itself the "New Physics". Classical Economists minimized complex processes into simple equations. Not only did they win unparalleled influence among leaders and politicians, but self-celebrated their success to levels never seen before. They even granted themselves a Pseudo-Nobel Prize (proper title: "The Sveriges Riksbank Prize").

Happily, beginning in the late 20 century, Economics and other social "sciences" are finding their way again. Economists recognize their proper place among academic disciplines, and place themselves above medicine and psychology, instead of next to physics. This reflects in 21st century Sveriges Riksbank Prize winners, like Daniel Kahneman (2002) and Robert Schiller (2013). Conversely, many of the winners of the 20th century have been debunked and forgotten.

## A Concluding "Bad" Theory

Sadly, there are still many Social "Scientists" around. I have my own "bad" theory on why.

* Those who understand statistics won't study Economics, Politics or Sociology as a "science". They would either research their pure scientific basis (like Kahneman) or as humanity (like Schiller), or do something else.

* Hence, those who do study Economics, Politics or Sociology as "science" don't understand statistics.

* Hence, as long as there are people who don't understand statistics, there is always the danger of Social "Sciences", and their fallout.

#### Article 227 · March 18, 2020

# The CoViD AI

### "Who to Quarantine" and Other Decisions

This article is a thought experiment about an imaginary Artificial Intelligence, which I call the "CoViD AI" (or CAI for short). This AI is omniscient, omnipotent and omnipresent about all things CoViD-19. I discuss what CAI would look like, and how we might build something like CAI.

[Disclaimer: The concepts described in this article are not original, and quite standard. Many have already written about it. Some are even making parts of it work.]

## The Qualities of CAI

### Omnipresent

CoViD, like many contagious diseases, is all about proximity. Person A infects Person B, only if one is physically close to the other. Hence, the first thing we need to know is was Person A close to Person B.

An Omnipresent CAI is "present everywhere" and would know where everyone is. And hence would be able to tell us where Person A or Person B is at a particular time:

```
function getLocation(person, time):    return location
```

If we know the locations of Person A and Person B at any time, we know also know the physical distance between Person A and Person B, and any particular time. And more importantly, whether they were close enough to each other to infect.

```
function getDistance(personA, personB, time):    return getDistanceBetweenLocations(        getLocationA(person, time),        getLocationB(person, time),    )
```

### Omniscient

Fighting CoViD is all about testing. We have to know if PersonA is sick with CoViD.

An Omniscient CAI is "all-knowing", and hence knows if any Person is sick.

```
function isSick(person):    return result
```

Not only would an Omniscient CAI know whether a person is sick, but it would also know what to do with this knowledge. For example, if a person is sick, they might need quarantine with different levels of medical support. A healthy 20-year-old will need very different treatment than a 70-year-old with diabetes and a weak heart.

```
function getAction(person):    result = isSick(person)    return getActionForTestResultAndPerson(result, person)
```

### Omnipotent

All the knowledge in the world is useless if one doesn't make use of it. In other words, make and take intelligent decisions and action based on that knowledge.

An Omnipotent CAI would have the "power to do anything". It would execute the action (determined omniscient) in a timely and efficient manner.

## AI without CAI

But CAI does not exist. Even the Chinese or the Americans, with all their AI prowess, have not succeeded in building one. A machine with such powers will likely never exist. So, what do we do?

We approximate. We might not have omniscient, omnipotent and omnipresent powers, but we can try to get close. Here are some ideas:

### Almost Omnipresent

Most Sri Lankans carry phones, and many of these are "location intelligent" smartphones. Hence, in theory, an Omnipresent CAI who knows where everyone is location already exists.

The Telcos that run our phone networks already have access to this information. They cannot "give away" this data to health authorities for privacy reasons. But the phone-owners could opt-in to share location, and the system could anonymise the data for security.

We could have laws to require high-risk individuals (e.g. recent returners, family and friends of infected cases) to opt-in, and advertising targeting lower-risk people.

### Almost Omniscient

One bottleneck in the CoViD battle is testing, which is expensive and time-consuming. While only a medical test can conclusively answer the "isSick" question, AI could crunch other data (location, symptoms, family details, etc.), and estimate of "probability of being sick."

```
function getProbabilitySick(person):    return p
```

Health workers could use this estimate to optimize testing. For example,

```
function doAction(person):     p = getProbabilitySick(person)    if p > 0.8:        doMedicalTest()    else if p > 0.6:        isolateAndWatch()    else if p > 0.2:        recommendSelfIsolate()    else:        doNothing()
```

[Disclaimer: I'm not a health expert, and I don't know if the probabilities and actions are meaningful. But you get the picture.]

### Approximate Omnipotent

In Sri Lanka, a combination of health workers and military personnel have done an excellent job on the "action" piece. If machine CAI "provides the tools" on the "Omnipresent" and "Omniscient", the our humans have all the "potency" to "finish the job".

## Concluding Thoughts

Time is of the essence. And will all things AI, Data is critical. Most of the data the AI needs already exists. But people who own. maintain and understand the data must come together and work on building the AI systems around them.

If this happens soon and smart, AI will play a central role in minimising the damage from CoViD-19; in the world in general, and Sri Lankan in particular.

Godspeed!

![Image](https://cdn-images-1.medium.com/max/800/1*JlsxfiVoKNyFJsGqtrML-g.jpeg)

#### Article 228 · March 18, 2020

# The Truth

### Why "the truth is rarely pure and never simple"

## The Whole Truth and Nothing but the Truth

Suppose I toss a coin. The question "what was the result?" has exactly two answers: "heads" or "tails". You can give the correct answer if you saw the coin fall; or if a truthful person informs you that they saw the fall; and what the result was. In this matter, the truth is simple. A simple binary.

Now suppose that I tossed a coin a 1000 times. Collectively, the result has two to the power 1000 possibilities; a decimal number with over 300 digits. Suppose I ask you the same question as before: "what was the result?"

The "Whole Truth" will be a list of 1000 "sub-results"; each being a head or a tail. If all 1000 sub-results are correct, your answer would be "Nothing but the Truth". If you miss any of the results (say, if you only report the last 500 results), your answer would be "Nothing but the Truth", but not the "Whole Truth". If you report all the results, but only the last 500 are correct, it would be neither.

## Arguments

Suppose Alice (like you), reports all the results, but only the last 500 are correct. Bob, also reports all the results, but in his case, only the first 500 are correct. Both Alice and Bob are "half-right" and "half-wrong". At the same time, the disagree on all 1000 results. They agree on nothing.

If the have a conversation about the results, it is likely to turn into an "argument" that can't resolve.

## Complexity

We can explain the result of a coin toss, or even 1000 coin tosses, or even a billion coin tosses, with precision and accuracy. But such an explanation is not possible for most real world phenomena.

Consider the statement: "Capitalism is better that Socialism" (or the reverse, if you wish it). Verifying this statement would involve analysing and understanding billions of data points. A "Capitalist" is someone who believes that most of the data points are consistent with the statement. A "fanatically, fundamentalist capitalist" might believe that *all* the data points are consistent. Similarly, a socialist would believe the opposite.

All but fanatics, both Capitalists and Socialists would accept that some data points support the opposite view. Often, the "Truth" is somewhere in the middle.

## Unknowns and Unknowable Unknowns

As complexity increases, the data points needed to verify statements also increases. Many of these data points would remain unanalyzed and unknown. Hence, some data points would support "Capitalism is better that Socialism", some would refute it, and many would remain unknown.

A particular variation of the "Unknown" is randomness; data points with changing values. A piece of evidence that supports one view at one time, and another at another. Unlike the "Unknown" in general, that might become "Knowable" future time, randomness consists of "Unknowable Unknowns".

Randomness is not the only "Unknowable Unknown". For example, Kurt Godel proved that certain mathematical statemens are true, yet, we cannot prove them true.

## Best Practices

* It is best not to have "strong views". Best to say "I don't know", "Yes and No", and "On the other hand".

* It is best not to pronounce simple answers to complex questions. To "Is Capitalism is better that Socialism?", only a fool would answer "Capitalism" or "Socialism".

* It is best to ask questions. Especially clarifying questions. "Is Capitalism is better that Socialism? How would you define better? What is Capitalism? What is Socialism?"

* It is best to try and hold the opposite view. While the opposite of a true statement must be a false statement, the opposite of a partially true statement, can also be partially true. All statements about complex phenomena are partially true; and hence so are their opposites. Hence, "Capitalism is better that Socialism" and "Socialism is better that Capitalism" can both be true.

* It is best not to adopt labels. Anyone who calls themselves a "Capitalist" or a "Socialist" (for example), might as well call themselves "Idiot"; or more completely "I am incapable of seeing complex phenomena as complex phenomena". The same applies to Religion and Politics.

* It is best not to describe others as labels. Anyone who says "Ah, he's a Capitalist Pig" (say), might as well say "I'm an Idiot"; or more completely, "I'm incapabale of understanding people at none but the most trivial level of sophistication".

* It is best not to dismiss any statement as inane. If someone says "You are a Capitalist Pig", while that might reveal the said someone's weaknesses, it might also say something true about you. "You" are a complex phenomena; and all statements about complex phenonema are partially true.

* It is best to look outwards for common ground. Many partially true views have no "inner" common ground (e.g. Alice and Bob). In mathematical terms, "the set intersection is empty". Instead, it is best to understand what is true in what the other says. This leads to an expansion of truth to the outer common ground, instead of a reduction to the inner common ground. In math words, "the set union is bigger than any of its components". For example, a "Pro Lifer" would not be able to accept "Pro Choice", and vice-versa. But both might be able to accept "Life is sacred" and "Women should be able to control their bodies".

* It is best to give people a chance. Most people label people of the opposing view with that label. Hence, "Charlie is a Capitalist" and "Sally is a Socialist". One's prejudice for the label clouds one's view of others. Give-up the labels and clouds clear.

![Image](https://cdn-images-1.medium.com/max/800/1*UJ6T_mkn0j5keNq3YCqLLQ.jpeg)

#### Article 229 · March 19, 2020

# On Tiredness

### Some reflections on justice and vulnerability

## Washing Dishes and Traffic Lights

Late last night I was washing dishes. I was tired and wanted to sleep. As I placed one last spoon on the dish rack, the damn thing fell off its perch and slid into some unreachable nook.

I almost heard myself mentally scream, "Why?!"

It's not just dishes.

Traffic lights always pick on me when I'm tired. There's not one car at right angles, but it insists on taking a vacation in the red.

But it's not just trivial things like spoons and traffic lights.

Even larger injustices seem to befall me when I'm tired. Bad things happen at work when I'm tired. Even my best friends turn into bad people when I'm tired.

Even the big world outside my little life seems to team with injustice when I'm tired. Children die of disease when I'm tired. Terrorists plant bombs when I'm tired. Wicked politicians get elected when I'm tired.

What's going on? How come my tiredness is all-powerful? How come all these injustices happen when I'm tired?

## A Theory of Injustice

Justice is some expectation that the world past, present and future abide by some rules. We believe that these rules to be "right", and we also expect these rules to be "enforced".

Conversely, we feel "injustice" if A) we believe in rules that are "right"; and B) these rules are not enforced. Someone or something breaks the rules.

Why is it, when I'm tired, the world is full of injustice? I don't quite know. But I have this theory:

When I'm tired, I'm also vulnerable. When we are weak, we look around for anything or anyone that will aide our survival. "Rules" are some of the first things we "anchor" on, because they are some of the few "certainties" in an otherwise uncertain world. When we are vulnerable, we want the rules to work. We want justice.

And when the rules don't work, as is common in an uncertain world, our sense of justice vents.

Conversely, when I'm not tired, I don't feel as vulnerable.

I'm more open and understanding of the uncertainties of the world. I know that spoons sometimes wall off, and traffic lights turn red. That things don't always go according to plan at work, and my friends face problems and difficulties from time to time. Even children die of disease, and people commit acts of terrorism. All of these, sometimes for reasons that I don't understand.

That's my theory.

## Caveats and Purpose

Now, I don't mean that we shouldn't try to fix problems. It's more about understanding that problems are normal. And that we shouldn't let it affect us too much. Also, that we should understand ourselves, we are likely to be more vulnerable at some times as opposed to others.

Especially when we are tired.

![Image](https://cdn-images-1.medium.com/max/800/1*dUH2ge92VmoH4Rzw6Qjynw.png)

#### Article 230 · March 20, 2020

# On Good and Evil

### Are there such things?

## Shouting Matches

I was watching one of those YouTube "intellectual shouting matches". An Evangelical Pastor and a Celebrity Atheist each took turns bashing the other.

I hate these "debates" because they are not "constructive". No one gains anything; the speakers nor the audience. It's a popularity contest where one contestant tries to out-poll the other.

"But then why did you watch it?", I hear you ask.

Well, the topic interested me: "Which was "Good and Evil: Does it require God?"

## Common Ground

The Pastor claimed that all good and evil comes from God. And without God, there was no good and evil. The Atheist claimed that humans evolved our sense of good and evil, because it helped us with survival.

Despite disagreeing at high volume, the debaters did agree on somethings things. They agreed on "what good and evil consisted of". For example, both agreed that "theft" and "murder" were evil, or "bad things".

They even agreed on a more fundamental point: That good and evil were conventions; that had no other reason or explanation beyond the convention.

The Theist believed that the convention was "laid down by God" and hence one could not argue with it. The Atheist believed that the convention was a product of evolution; also, uncontroversial. While the Celebrity Atheist described himself as an "Atheist", he did have a sort of god. He was a firm "believer" in "Fact of Evolution", and he was even more devout and assured than the Man of God.

They even agreed on "incentives": or why people wanted to do good things, and not do bad things.

One argued that they wanted to please god, and receive their reward in heaven, post death. God's incentive. The other argued that doing "good things" made them feel pleasure and other good emotions. Evolution's incentive.

## The Golden Rule

So, were there no fundamental things that were "good" or "evil"? Was good and evil only relative to conventions? Either those of this world, or those of the next?

There seems to be one concept of good which is "not relative"; or strictly "not relative to anything else"; because it is relative to itself, though independent of everything else. That concept is "reciprocity"; also known as the "Golden Rule".

Being or doing something is "good" if you believe that the opposite is also good. For example, Alice doing X to Bob is "good", if Alice and Bob are happy with Bob doing X to Alice.

While I tried to "dress-up" the Golden Rule as an "absolute", at some level it is also a convention. Why should one follow it? Is there anything "below" the Golden Rule? Some more fundamental concept that is absolute?

## The Mother of Golden Rules

I don't have a good answer to this question, except that the Golden Rule's innate "recursiveness" gives it some "stability" and "concreteness". While Alice's sense of good could be unstable and arbitrary, joining it with Bob's concept makes it stronger.

This "joining" can be further extended. Whenever we have some concept of good, we could try and "join" it with the concept of good of everyone and everything.

Hence, the ultimate good is what everyone can agree on as good.

## Lost in Ignorance

"But hardly anyone agrees on anything", you lament.

True. And few people will agree on "sense of good" either. The violent disagreement we see between religious and political ideologies are proof of that.

But why do they disagree? Is it because the honestly disagree? Or is it for other reasons? Power, for example? Or even more "powerful" Ignorance?

What would "good and evil" look like, if everyone and everything had no Ignorance?

![Image](https://cdn-images-1.medium.com/max/800/1*2eH_d6Aaldkg7-nwRlIAtA.jpeg)

#### Article 231 · March 21, 2020

# An Eye for an Eye

### Makes the whole world blind

All crimes are forms of theft. A villain steals some "thing" from the victim.

When the thing is the truth, we call it fraud. When the thing is an object, we call it theft. When the thing is an eye, we call it grievous bodily harm. When the thing is life, we call it murder.

Justice is also theft. Where the victim, or society, or "the law" takes another "thing" back from the villain. In return for the crime.

When the thing is time, we call it imprisonment. When the thing is life, we call it capital punishment. When the thing is dignity, we call it "a warning".

...

Sometimes crime is justice. Especially in the eyes of the villain. Like Robinhood, who stole from the rich and gave to the poor. Because the rich had already stollen from the poor.

Sometimes justice is injustice, especially when the punishment is excessive or arbitrary.

Hence, crime and justice are the same things disguised as different things. They are both forms of theft and encourage further robbery. Both end-up propagating webs of theft and counter theft.

Some people might like to steal from others. But no one likes to be stolen from. Hence, both justice and crime ends-up making someone unhappy; regardless of who they end-up pleasing.

Hurting people cannot be right. Hence, justice is wrong; as crime is wrong.

...

The solution to crime is not to commit other crimes in return. But to find and destroy the sources of that crime. Often injustices like poverty, ignorance or illness. Often "justices" disguised as injustices: "It is just that the poor are poor", "It is just stupid are ignorant", "It is just that the weak are ill". Kill the source, and crime will die.

But many people believe in injustice as justice. "Evil" is one word that represents all injustice: "The criminal is not just poor, ignorant and ill, it is also Evil".

...

But perhaps we don't want solutions to crime. We want to commit crimes ourselves. And what better way to indulge our lust for stealing by seeing a man hang, and his families future evaporate? Not only is it legal, but it is also "just".

![Image](https://cdn-images-1.medium.com/max/800/1*S5xlBoeFm4J--cgQ5H4mjw.jpeg)

#### Article 232 · March 26, 2020

# On CoViD19 and Jobs

### The New Normal

CoViD19 is all about distance. The only way a human gets sick is if they are close to another human who is ill.

Hence, any "CoViD19 Defence Plan" is significantly about distance and "distancing"; making sure that humans are not too close to other humans.

## Economics

Economies are webs of people, buying and selling goods and services. Those with ability produce and sell. Those with need buy and consume. Often, especially in Market Economies, what you can buy is equal to what you sell.

We buy and sell different "things". If the "thing" is "touchable" we call it a "good", like a banana or a car. If not, we call it a "service", like a doctor's advise.

All human work consists of producing services, though some of these services might contribute to producing goods. For example, a "farmer" is selling a "farming service", which goes into producing a "farmed good", like a banana.

## Information Exchange and Services

Services involve the exchange of information. This information must travel back and forth between buyer and seller.

For example, you might tell a doctor your temperature. And in return, the doctor might tell you what to do about it.

Some information can travel over telecommunication lines, like text, sounds and pictures. Other's can't; like touch and smell.

If all the doctor needs to know is your temperature, then you can consult them over the phone. If he needs to feel your cheekbones, you need to consult him in person.

## CoVid19 and Jobs

Does "distancing" affect a human's work? That depends on the service they provide, and the information exchange involved.

If the information exchange can happen entirely over the telephone or internet, that human could work from home; assuming that the home is "connected".

If the information exchange doesn't involve other humans or being close to other humans, the human could work from work, like regular days.

The problem arises if the information exchange does involve other humans; many humans, in the worse case.

For example, a medical nurse has no choice but to interact with hundreds of humans every day; many of them might be sick. A teller at the supermarket does the same.

## Distancing Jobs

It's easy to understand why a nurse has to be close to many people. But why a supermarket teller?

Many reasons.

Logistics is one. If people could buy groceries and other items online, efficiently, there would be no need for grocery shops. The lack of such a system means that people need to flock to supermarkets.

Trust is another. Many people might not trust an e-commerce site to send them high-quality items. If they visit a physical store, they can hand-pick what they need.

And cost. A fancy electronics store could afford to list its wares online. A poor hawker on the Pettah pavement, cannot do the same. Cost is also proportional to development. We could imagine a more economically developed world, where any business could afford to list on the internet; and any consumer could afford to access and buy.

If we find solutions to these problems, more and more jobs may happen "from a distance".

## Localising Jobs

But what about Nurses? No amount of technology could distancify many aspects of the "nursing service".

A different approach to "distancing" could be to limit close contact to small clusters.

For example, what if hospitals and nurses only served patients who lived within a 5-mile radius of a hospital? The same could apply to schools and work. While humans would still be at risk, any epidemic restricts to clusters. Small clusters are robust, while a hyper-globalised world is fragile.

In the future, we might have to forgo various levels of "globalisation"; both nationally and internationally, especially if crises of all sorts are more common. We can't over-rely on more extensive networks.

## Equalising Jobs

And what about the day labourer who tends to your garden? You might pay them well, but only on the days they work.

While tending to plants is no CoViD19 risk, measures like curfews and #LockDowns mean that day labourers can't travel to their customers. And hence, can't work.

In a world where humans need separation from other humans, at the drop of a hat, these jobs become vulnerable. Hence, we need ways in which humans are protected from periods of lost work. Some form of insurance.

## Concluding Thoughts

The "New Normal", like all new things, is not innately better than the "Old Normal". It merely choses a different trade-off. Distancing, Localising and Equalizing are not "better". They are just different. They choose robustness over efficiency. Or, statistically, smaller means, over larger variances.

The history of history is the history of changing tradeoffs. And significant points of history involve substantial changes. CoViD19 might be one of the most significant.

![Image](https://cdn-images-1.medium.com/max/800/1*yEMU1IwQULJHwFn_dh2NaQ.jpeg)

#### Article 233 · March 28, 2020

# On Conscious Machines

### A thought experiment

In this article, I describe a sequence of machines; each more "conscious" than the previous.

Disclaimer: Since we cannot know if something else is "conscious" my definition and measurement of consciousness is indirect.

## Level 1 — Recording

A Level machine has sensors that record the external world: Cameras, Microphones, Touch Sensors, Smell Sensors and Taste Sensors.

We inspect what the machine records, to verify that the machine is sensing correctly. For example, we analyse the videos that it records, to see if those record the actual world.

## Level 2 — Reacting

A Level 2 machine can react to what it records. The reactions might be specific or arbitrary.

For example, a level 2 machine "might not like" bring light. If we flash a torch at it, it might emit an annoyed sound, or move away from the light source.

How do we know that it is actually "annoyed"? Or that it moved away because it didn't like the light?

Well, we don't. Our definition of "annoyed" is emitting the annoying sound or moving away. That is how we measure "not like".

## Level 3 — Abstractions

A Level 3 machine, not only records the physical world but also converts these recordings into abstractions. For example, it might classify the video frames it records, into having specific dominant colours; like red or blue.

While our machine reacts like a Level 2 machine, its triggers are abstractions. It might "not like" red light, but like other forms of light.

## Level 4 — Connections

A Level 4 machine is a Level 3 machine, with the ability to make connections between abstractions. It might connect "seeing red" with "feeling liquid" and "tasting metallic". It might define new abstractions around these connections. For example, it might call the red, metallic tasting liquid "blood".

Like Level 2 and Level 3 machines, the Level 4 machine would also react, not just to raw information, or abstractions, but also connections. For example, it might be "afraid of blood".

## Level 5 — Time

A Level 5 machines not only records the physical world, but it also records "snapshots" of these recordings.

For example, it could store a copy of "yesterday's world".

The frequency of the snapshots might differ from machine to machine, and defines "how fast time passes" for these machines.

![Image](https://cdn-images-1.medium.com/max/800/1*cKah3-1jpgjq_wnQEkeaiw.jpeg)

#### Article 234 · March 28, 2020

# On Logic

### Observation and Abstraction

## Logic

Consider these statements:

>>> "All swans are white".

>>> "Of all the swans I've observed, all swans are white".

The latter statement is a fact. The former statement is a generalisation of that fact; a "theory".

We can "falsify" the theory, by demonstrating that there are swans that are not white; black swans, for example.

But what about facts? Can we falsify facts?

## Observation

Suppose only white swans live in my country, and only black swans live in your country. And suppose we meet in a country with no swans.

For you, "Of all the swans I've observed, all swans are black" would be correct. And you would, reasonably, believe in the theory "All swans are black".

If I were unable to understand your "perspective", or that your country was a "black swan" country (and vice versa), we would never be able to agree. You would insist that swans are black; and I, white.

But there are even deeper problems.

## Abstraction

Suppose the swans in your country were precisely the same as the swans in my country. And they were neither black nor white, but some shade of grey.

The swans in your country live in sunny woods surrounded by bushes with bright white flowers. The swans in my country live in dark ebony forests with tall trees with the darkest barks.

Hence, because of their white background, the grey swans in your country appear black. And similarly, the grey swans in my country appear white.

Now despite the swans being identical, we disagree on two abstractions: "Whiteness" and "Blackness". Your "blackness" is the same shade as my "whiteness". But we can't agree that they are the same thing.

## The Problem

Logic depends on set theory.

Set theory, in turn, depends on two things:

* Our ability to observe. To assign something to a "white swan" set, we need to see a "thing" which exhibits both "swan-ness" and "whiteness".

* Our ability to assign things to sets, through abstractions. For example, to assign a swan to the "white swan" set, we need to define "swan-ness" and "whiteness".

Unfortunately, we have a flawed ability for both abstraction and observation. As long as these flaws exist, our the ability to reason with logic is also imperfect.

We might think we are logical. But we are not.

![Image](https://cdn-images-1.medium.com/max/800/1*u7J5Dib9roz7_l4LUbZ31A.png)

#### Article 235 · April 3, 2020

# Two sides of different coins

### On Justice and Karma.

Alice punched Bob in the face. Policeman Charlie locked Alice up for seven days; the punishment for punching Bobs. Justice!

Bob earned a black-eye, and Alice a jail-term. But was that all that happened? Not quite.

One might have expected Alice to show some remorse. But no. True — she had not enjoyed her week in chokey. But she did enjoy the punch, and Bob's subsequent dazed look. And the unique hue of blue and black that emerged, a few days later, around Bob's left eye.

No. Alice enjoyed the episode. She hadn't had this much fun in years.

But something else also happened.

The next week when Alice met Daisy, she noticed that she wanted to punch her in the face too. Even harder than she had hit Bob. Knock her block off proper. And so she did.

This time Alice earned a full month in jail. And three months of community service afterwards. And, on top of all this, a fine.

What did Alice feel about it? She felt magnificent. The attack on Daisy was a significant improvement compared to last time. Daisy had received, not one, but two black eyes. Alice had also succeeded in partially dislodging Daisy's upper right canine. She had never felt better.

Was Alice going mad? Did she need psychiatric help? Her defence seemed to think so. Maybe they were right. I don't know.

But what if things got worse? What if this need to punch people completely took-over Alice's entire personality? What if Alice became the people puncher? Karma!

![Image](https://cdn-images-1.medium.com/max/800/1*jdX5z_NRg8rNdPj6mV2Zeg.jpeg)

#### Article 236 · April 15, 2020

# On Fake News

### Ramblings of a Cynic

## On Falseness

* The "trueness" or "falseness" of a piece of news (or any proposition) lives in the mind of the consuming person.

* The "trueness" or "falseness" of a piece of news within a group is the collective "trueness" or "falseness" that live within the minds of the consumers that people the group.

* Beyond the simplest propositions (E.g. "2 + 2 = 4") there are few "absolutely provable" truths. The "bar for probability" is constantly rising (Especially with DeepFakes).

## On Fact-checking

* Fact-checking is the process of establishing a piece of news as true or false.

* For simple propositions, fact-checking is a process of connecting the proposition with absolute truths.

* For complex propositions, fact-checking is a process of convincing people that the proposition is true or false.

* Almost all pieces of news are collections complex propositions.

## On Influencers

* An influencer is someone who controls the "trueness" and "falseness" that lives within peoples minds.

* An independent thinker is someone who is not influenced by influences.

* Fact-checking could either influence or encourage independent thought. One is easier than the other.

* "Independent thought" requires deep thought. "Being influenced" requires shallow or no thought.

## On Social Networks

* A solitary individual is (by definition) an independent thinker. She/he cannot be influenced, because there is no other to influence.

* Influencers thrive on large social networks, with shallow interactions. The more extensive the social network, the more influence, the less independent thought.

## On Fake News

* Fake news is news that you believe to be false.

* Belief in fake-news necessarily requires a belief in true-news. One cannot exist without the other.

## On Free Thought

* A "free-thinker" is one with no beliefs.

* A free-thinker is necessarily an independent thinker. She/he is not controlled by the beliefs of others (influences)

* For a free-thinker, there is no fake or true news.

![Image](https://cdn-images-1.medium.com/max/800/1*GbnY1r2of2IU7IN_mGHNWA.jpeg)

#### Article 237 · April 17, 2020

# On Ability

### Aphorisms

* Ability is a prediction of whether one is "able" to do something in the future.

* The prediction might be binary ("I am able" or "I am not able"), or probabilistic ("There's a fifty-fifty chance than I'm able")

* Confidence is the ratio between what one thinks one can do, and what one can do. If the proportion is greater than one, one is "over-confident".

* Just as we can talk about future ability, we can also talk about the past ("I was able to..."). But what usually matters is "present" ability ("I am able...").

* Both past and future are misleading. We might not be (or be) able to do in the future, what we did (or did not) in the past.

* The only way of knowing for sure, if one is able to do something, is to just do it. Now.

![Image](https://cdn-images-1.medium.com/max/800/1*UByNeqytTXPTPZMYnCMe3g.jpeg)

#### Article 238 · April 25, 2020

### Geography of Sri Lanka

# Where can I see Adam's Peak?

### And other mountains

[If you're not interested in the Maths, please skip to the Appendix]

As the South-West monsoon picks up, the air quality in the South-West of Sri Lankan in general, and Colombo in Particular, improves. Coupled with the CoViD19 Lockdown in the Colombo District, and the resulting implosion of traffic, Colombo air is uncharacteristically clean.

The good air not only makes breathing easier, but also seeing easier. And so, unsuprisingly, the internets are full of sightings of mountains; Adam's Peak in particular. Here's one of my favourites by Namal Kamalgoda.

![Image](https://cdn-images-1.medium.com/max/800/1*gi4wbkf5mQewxaZd8nKqJQ.jpeg)

But from where can you see Adam's Peak? And what else can you see?

Read on to find out.

## How far can we see?

The curvature of the earth puts a limit on how far we can see. We know this from disappearing ships over the horizon, as we stand on the sea shore. But how far away is the horizon exactly?

A bit a simple maths, including Pythogoras's Theorem will tell us.

Suppose,

```
R = Radius of the Earthh = The height of the observer d = The distance to the horizon
```

Then, R, d and (R + h) form a right-angle triangle. (R + h) is the hypotenuse or the side opposite the right angle.

Then,

```
By Pythogoras's Theorem,R² + d² = (R + h)²
```

```
Therefore, d² = (R + h)² - R²= R² + 2Rh + h² - R²=(2R + h).h
```

```
Assuming that R is much larger than h, we can ignore the first h, giving,
```

```
d² = 2Rh
```

```
And finally,
```

```
d = √2Rh
```

For example, if you were 1.8m (just under 6ft tall, or 0.0018km), and given that the earth's radius is 6,371 km, we get,

```
R = 6371h = 0.0018d = √2Rh = 4.789
```

The horizon would be about 4.8km away.

Similarly,

* If you were 1.5m (or just under 5ft tall), the horizon would be about 4.3km away

* If you were standing at the top of a 150m tall building, the horizon would be about 44km away.

* If you were standing at the top of the Lotus Tower (350m), the horizon would be about 67km away.

![Image](https://cdn-images-1.medium.com/max/800/1*e09BRhFAPVaUKi1PLD12Rw.png)

Why did I bring up horizons and lotus towers? To make this simple point: The higher-up you are, the further away you see.

## What can we see?

Adam's Peak is about 80km away from Colombo. That's even further than the horizon from the top of the Lotus Tower. So, does that mean we can't see Adam's Peak from Colombo.

Not quite.

The curvature of the earth will hide the bottom part of a mountain that is far away. But if the mountain is high enough, the top part might be visible. Calculating how much, needs some more calculations and more Pythogoras.

Suppose,

```
D + d = The distance from the observer to the mountain(Note, D is the distance to the mountain, beyond the horizon)H = The height of the mountain b = The height of the bottom part of the mountain hidden by the curvature of the earth
```

Now, R, D and (R + b) form a right-angle triangle. (R + b) is the hypotenuse.

Since we know D, and R, we can compute b as follows:

```
By Pythogoras's Theorem,R² + D² = (R + b)²R² + D² = R² + 2Rb + b²
```

```
D² = 2Rb + b²= b(2R + b)
```

```
Assuming that R is much larger than b we getD² = 2Rbb = D² / 2R
```

For example, if we are looking towards Adam's Peak from a 100m tall building in Colombo, we get,

```
R = 6371d = 44 (See above)D = 80 - d = 36b = 0.1017
```

Hence, the bottom 102m of Adam's Peak would be cut-off. Since the mountain is 2,243m high, we should be able to see the top 2,141m of it.

What if we were not on a tall building, what we were 1.8m tall, and at sea level? Then,

```
b = 0.44381
```

Or, the bottom 444m of Adam's Peak would be cut-off, but leaving plenty off the top. Hence, we should be able to see Adam's Peak without the aid of tall buildings.

![Image](https://cdn-images-1.medium.com/max/800/1*vq31UdBMTjplGbyQcwETMg.png)

While in theory we should be able to see Adam's Peak from the ground, in practice, buildings and other obstructions get in the way. So unless your in a place with little obstruction (e.g. a large ground), some building is likely to block your view. That is why, in practice, you need to get on top of something.

## Modelling what we can see

We know we can see Adam's Peak. But what else can we see? Can we, for example, see Sri Lanka's tallest mountain Pidurutalagala (2,524m)? More generally, can we create a "model" to visualise everything we could see?

### α and ϐ

Suppose you are in the top floor of the World Trade Centre (WTC) in Colombo Fort. You are about 150m above sea-level. Suppose you are looking out of a window facing east, and your horizontal vision spans from North (0°) to South (180°). Let's call this horizontal angle α.

Now, we can look at the horizon (0°), at some point below the horizon, upto directly below us (-90°), or above the horizon, upto directly above us (+90°). Let's call this vertical angle ϐ.

Everything that we see has some α and ϐ. If two things have the same α and ϐ, whatever that is closer will block that which is further away. Hence, we can "model" what we can see by computing its α and ϐ, and seeing if there is some closer thing with the same α and ϐ, that will block it.

Suppose you are looking at Adam's Peak? How do you compute α and ϐ?

If you can see the mountain clearly, you can measure α with a compass, and ϐ by the angle at which you are looking up.

But what if you can't see the mountain? Or you see some mountain, but are not sure if it is Adam's Peak?

We can compute both α and ϐ using a map and altitude information.

### Computing α

The WTC is located at (6.9327° N, 79.8438° E). Adam's Peak is at (6.8096° N, 80.4994° E). α is the tangent of the line between these points.

![Image](https://cdn-images-1.medium.com/max/800/1*qDCloRJGr1bMoqPfa0CnHw.png)

Or,

```
lat0, lng0 = 6.9327, 79.8438 (World Trade Centre, Colombo 1)lat1, lng1 = 6.8096, 80.4994 (Adam's Peak)
```

```
Tan (α - 90) = (lat0 - lat1) / (lng1 - lng0)= (6.9327 - 6.8096) / (80.4994 - 79.8438)= 0.1878
```

```
α = Tan⁻¹ 0.1878 + 90= 100.7
```

So, Adam's Peak should be visible at about 100.7°, or 10.7° from East to South.

### Computing ϐ

![Image](https://cdn-images-1.medium.com/max/800/1*nHh5Tr5-N4VmdoJFareBbw.png)

```
By the symmetry of triangles, x = D (H - b) / (R + b)y = R (H - b) / (R + b)
```

```
Tan ϐ = y / (x + D + d)ϐ = Tan⁻¹ y / (x + D + d)
```

For our WTC scenario,

```
D + d = 80D = 36 (see above)(H - b) = 2.141 (see above)(R + b) = 6371.102
```

```
Therefore,x = 0.0121y = 2.1410
```

```
And, ϐ = Tan⁻¹ y / (x + D + d)= Tan⁻¹ 2.1410 / (0.0121 + 80)= 1.53°
```

Or 1.53° above the horizon.

Hence, now we can compute α and ϐ for every location in Sri Lanka. Using this information, we can visualize mountains. For the visualisations below, I use latitude and longitude information about Sri Lankan mountains from Wikipedia, and altitude information from USGS.

This is what Adam's Peak should look like if viewed from the top of WTC:

![Image](https://cdn-images-1.medium.com/max/800/1*PbXRzXU8pRVXptu0lQzbHA.png)

## Appendix: Examples

### Colombo (World Trade Centre, 150m)

![Image](https://cdn-images-1.medium.com/max/800/1*qryUbJ32JOlcVA7qV_gMUA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*R0catPoyG-OZesbcwXVTzA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*PbXRzXU8pRVXptu0lQzbHA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*y3j5zLcwiuzQMpOiJp-Ifg.png)

### Matara (Hypothetical 150m Building)

![Image](https://cdn-images-1.medium.com/max/800/1*zhOfd-Eebym0hOLdYbLQYg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*W2IViJ0Jz0mhC6SGOiqFDA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*7vyZEjIyvYUcqbUqnSKtWg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*atNuSqQDXopG4VrpBM8J2A.png)

![Image](https://cdn-images-1.medium.com/max/800/1*agJvc4gpMD9xCjVX1E7rJA.png)

### Batticaloa (Hypothetical 150m Building)

![Image](https://cdn-images-1.medium.com/max/800/1*9JLFt-hvREyDJgf1OGeweQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*rjKIh3f24w4RDUqGArDMXA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*oO7jipdrp6DxN9HK-wivkw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*tTNQpmDMoEJ0ncIGT_pfFw.png)

### Kadugannawa Rock View (500m)

![Image](https://cdn-images-1.medium.com/max/800/1*eANkTi1UntpZRZGCp0DcXA.png)

### Sigiriya (Top of the Rock, 349m)

![Image](https://cdn-images-1.medium.com/max/800/1*IvI7Ul6d3TpXnBAQun1IIA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*4Yk-wY1cDZgSiElzXg8mMg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*AQHNM5fxyLuFUQ5jDIUP0g.png)

### Anuradhapura (Hypothetical 150m Building)

![Image](https://cdn-images-1.medium.com/max/800/1*l7oRu3yyPoMp-YwuMjN_Iw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*OXqZpcs9Ou1iTwAGcOdZEA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*mqMVZ8hing3EjW-RI_4N_g.png)

### 20km West of Colombo Harbour (at 0m)

![Image](https://cdn-images-1.medium.com/max/800/1*Rw8iBIct2bDZmCCVnE_tcw.png)

### 30km West of Colombo Harbour (at 0m)

![Image](https://cdn-images-1.medium.com/max/800/1*Et9Kp_WCcaazmqa5dByIlQ.png)

### 35km West of Colombo Harbour (at 0m)

![Image](https://cdn-images-1.medium.com/max/800/1*NncPOO-WYRSHYJsxBtoZ3w.png)

## Appendix: Special Case of Nearby Mountains

What if the mountain is "before" the horizon?

![Image](https://cdn-images-1.medium.com/max/800/1*QHSQixid2EppExdviQatfw.png)

We modify computing ϐ as follows:

```
By Pythogoras's Theorem,R² + (d - D)² = (R + b)²R² + (d - D)² = R² + 2Rb + b²
```

```
(d - D)² = 2Rb + b²= b(2R + b)
```

```
Assuming that R is much larger than b we getD² = 2Rbb = (d - D)² / 2R
```

```
By the symmetry of triangles, (D - x) = (d - D) (H - b) / (R + b)Therefore,x = D - (d - D) (H - b) / (R + b)y = R (H - b) / (R + b)
```

```
Tan ϐ = y / xϐ = Tan⁻¹ y / x
```

#### Article 239 · April 26, 2020

### Geography of Sri Lanka

# Top 100 Mountains of Sri Lanka

### From First Principles

What are the 100 tallest mountains in Sri Lanka?

In this article, I answer this question from first principles, using altitude data from https://earthexplorer.usgs.gov/ (which can be downloaded for free).

## "Mountain" Defined

I define a "mountain" as a location with "topographic prominence" of 1000 ft (304.8m) or more.

"Topographic prominence" of a hill is defined as "the height of the hill from the lowest contour line surrounding it, which contains no higher peak".

More intuitively, it is the height of the hill from its "base".

![Image](https://cdn-images-1.medium.com/max/800/0*JjIzQfLP2ir7D9SA)

[My 1000ft limit might be somewhat arbitrary. As we will see, some "proper mountains" (like Kikilimana and Kudahagala) have lower prominences. Conversely, many mountains with higher prominences have not been named as mountains.]

## Top 10

Using this definition, and some python scripts, I computed the Top 100 mountains in Sri Lanka. These are the Top 10:

1. Pidurutalagala (2524m/2524m) — 7.001665N,80.772689E

2. Kirigalpotta (2395m/950m) — 6.799334N,80.766028E

3. [Unknown] (2361m/326m) — 7.009159N,80.757702E

4. Totapolakanda (2357m/398m) — 6.833472N,80.819317E

5. Adam's Peak (2243m/1083m) — 6.809326N,80.498751E

6. Great Western Mountain (2216m/462m) — 6.960866N,80.695254E

7. Hakgala (2170m/377m) — 6.918401N,80.810991E

8. Conical Hill (2166m/327m) — 6.912573N,80.776020E

9. [Unknown] (2127m/393m) — 7.076603N,80.732723E

10. Mahakudagala (2100m/395m) — 7.044130N,80.843464E

[The two heights indicated are total altitude from sea level, and topographic prominence. For example, Adam's speak has total altitude from sea level 2243m, and a prominence of 1083m.]

Wikipedia also defined a "Top 10" in its "List of Mountains in Sri Lanka" article. While most of the 10 were common, there were a few exceptions.

![Image](https://cdn-images-1.medium.com/max/800/1*M_uG3KUob9oyxx7qfKREEA.png)

Both Kudahagala and Kililimana didn't have sufficient prominence (<1000ft), because they were both very close to two other mountains, Kirigalpotta and Pidurutalagala respectivelly.

Kudahagala fell inside the 2160m contour that included Kirigalpotta.

![Image](https://cdn-images-1.medium.com/max/800/1*Q3kK3YNbLRFGebZXDC469g.png)

Kikilimana fell inside the 2000m contour that included Kirigalpotta.

![Image](https://cdn-images-1.medium.com/max/800/1*sKg8mXw_0vhAV12qEwKoSw.png)

One Three Hill also has insufficient prominence.

Conversely, my list had two Top 10 entries, not listed in Wikipedia. Nor did they seem to have names on Google Maps; though it was clear that they were mountains with high prominence.

![Image](https://cdn-images-1.medium.com/max/800/1*_imrTnbAUxaQqSMRi-86Dg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*9QYCda1tD7THTTRdLhjjLA.png)

## 11th to 20th

As with the top 10, there are some "Unknown" or "Unnamed" mountains. Also, names ending with a "?" might be incorrect. The only source I had was Google Maps.

11. [Unknown] (2072m/560m) — 6.830974N,80.684430E

12. Kotiyagala? (2049m/526m) — 6.768526N,80.657785E

13. Namunukula (2036m/1291m) — 6.932556N,81.113239E

14. [Unknown] (2035m/555m) — 6.764363N,80.587011E

15. Gonmollikanda (2034m/391m) — 6.766028N,80.810158E

16. [Unknown] (1990m/308m) — 6.791007N,80.569525E

17. Idalgashinna (1977m/564m) — 6.784346N,80.879267E

18. Ballanbedi hela (1963m/328m) — 6.829309N,80.494588E

19. Nayabadda (1949m/823m) — 6.804330N,81.017485E

20. Dell Estate? (1878m/334m) — 6.882598N,80.650291E

## 21st to 100th

21. Knuckles (Gombaniya) (1863m/1441m) — 7.455454N,80.750208E

22. [Unknown] (1860m/510m) — 7.448793N,80.760200E

23. Knuckles (Peak 4) (1856m/611m) — 7.401332N,80.810158E

24. Thangamale (1768m/460m) — 6.773522N,80.914238E

25. Haputale Mt? (1763m/485m) — 6.774355N,80.968360E

26. [Unknown] (1731m/320m) — 6.895087N,80.619484E

27. [Unknown] (1719m/306m) — 6.945046N,81.105745E

28. [Unknown] (1718m/473m) — 6.970858N,80.580350E

29. [Unknown] (1713m/534m) — 6.910908N,81.104913E

30. [Unknown] (1680m/435m) — 7.372190N,80.822648E

31. [Unknown] (1677m/324m) — 7.038301N,80.683597E

32. Knuckles (1671m/305m) — 7.439634N,80.769359E

33. [Unknown] (1671m/448m) — 6.990841N,80.919234E

34. Dumbanagala (1616m/775m) — 7.383847N,80.855121E

35. Knuckles (1598m/357m) — 7.440466N,80.809326E

36. Kurullangala (1582m/391m) — 6.804330N,81.054122E

37. Dothalugala (1570m/613m) — 7.332223N,80.850958E

38. Seven Virgins (1565m/306m) — 6.883430N,80.497918E

39. Narangala (1565m/719m) — 7.036636N,81.010824E

40. [Unknown] (1565m/379m) — 6.885096N,81.117402E

41. Kehelpathdoruwegala (1563m/725m) — 7.411324N,80.886761E

42. Kunu Diya Parwathaya (1554m/438m) — 6.812656N,80.449625E

43. Knuckles (1547m/763m) — 7.467111N,80.820150E

44. Knuckles (1532m/309m) — 7.474604N,80.753539E

45. Kolapathana (1525m/313m) — 6.992506N,80.616153E

46. [Unknown] (1515m/775m) — 6.653622N,80.624480E

47. Dobagasthalawa (1513m/309m) — 7.024147N,80.613655E

48. Warnagala (1510m/390m) — 6.836803N,80.452956E

49. Lunugala (1510m/871m) — 7.100749N,81.161532E

50. Kukulagala (1503m/627m) — 7.166528N,80.801832E

51. Kabaragala (1501m/930m) — 7.070774N,80.502914E

52. [Unknown] (1501m/554m) — 7.024979N,81.173189E

53. [Unknown] (1498m/411m) — 6.976686N,81.128226E

54. [Unknown] (1497m/575m) — 7.550375N,80.729392E

55. [Unknown] (1495m/357m) — 6.864280N,80.515404E

56. Monara Gala (1493m/576m) — 7.086595N,80.631141E

57. Pettigala (1492m/360m) — 6.649459N,80.641965E

58. Hunnasgiriya (1485m/478m) — 7.388010N,80.699417E

59. Pilkington Point (1469m/309m) — 6.763530N,81.054954E

60. Riverston (1467m/445m) — 7.530391N,80.732723E

61. [Unknown] (1462m/356m) — 6.865112N,81.013322E

62. [Unknown] (1460m/351m) — 7.153206N,81.119067E

63. Hawagala (1414m/530m) — 6.722731N,80.742714E

64. [Unknown] (1411m/398m) — 7.088260N,81.165695E

65. [Unknown] (1409m/397m) — 6.996669N,81.182348E

66. [Unknown] (1408m/498m) — 7.089092N,80.902581E

67. [Unknown] (1403m/356m) — 6.904246N,81.022481E

68. [Unknown] (1381m/307m) — 7.085762N,81.185679E

69. [Unknown] (1373m/402m) — 7.552040N,80.710241E

70. Beragala (1365m/1146m) — 6.438801N,80.572023E

71. Gongala (1358m/548m) — 6.386345N,80.653622E

72. [Unknown] (1333m/374m) — 7.199001N,80.701082E

73. [Unknown] (1330m/546m) — 7.025812N,80.463780E

74. Punugala (1324m/734m) — 7.046628N,80.402998E

75. Lunugala (Peak 2) (1320m/421m) — 6.947544N,81.172356E

76. Medamahanuwara Kanda (1318m/478m) — 7.288093N,80.844296E

77. [Unknown] (1318m/319m) — 6.991674N,81.127394E

78. [Unknown] (1317m/327m) — 6.921732N,81.152373E

79. Uragala (1309m/403m) — 7.229808N,80.636969E

80. Gammaduwa (1308m/510m) — 7.589509N,80.704413E

81. Rangala (1299m/341m) — 7.348043N,80.783514E

82. [Unknown] (1281m/323m) — 6.909242N,80.513739E

83. [Unknown] (1281m/319m) — 6.715237N,80.601998E

84. [Unknown] (1261m/305m) — 6.449625N,80.593672E

85. Ingurugala (1255m/484m) — 7.116570N,80.443797E

86. [Unknown] (1244m/320m) — 7.103247N,80.453789E

87. [Unknown] (1240m/397m) — 6.930058N,81.059950E

88. Pannila (1239m/426m) — 6.474604N,80.552040E

89. Ethipola (1239m/761m) — 7.490425N,80.581182E

90. Kimbullawa (1223m/337m) — 7.054122N,81.036636E

91. [Unknown] (1213m/796m) — 7.605329N,80.577019E

92. Wiltshire (1187m/505m) — 7.491257N,80.604496E

93. [Unknown] (1181m/311m) — 6.410491N,80.621982E

94. [Unknown] (1176m/423m) — 7.138218N,80.928393E

95. Narangamuwa Lakegala (1153m/327m) — 7.467111N,80.839301E

96. [Unknown] (1151m/408m) — 7.062448N,81.094921E

97. [Unknown] (1125m/339m) — 7.043297N,81.100749E

98. [Unknown] (1115m/322m) — 7.158201N,80.929226E

99. Kalugala (1110m/442m) — 7.149875N,80.431307E

100. [Unknown] (1109m/375m) — 7.320566N,80.892590E

## "Maps"

Here are some "map" visualizations of the mountains. There is some overlap between the groups.

### Matale Hills

![Image](https://cdn-images-1.medium.com/max/800/1*f2bKzvHDZBNFmQOHh68BKg.png)

### Western Hills

![Image](https://cdn-images-1.medium.com/max/800/1*Tl9EV6l9K3H89_vcBPdiyw.png)

### Eastern Hills

![Image](https://cdn-images-1.medium.com/max/800/1*tWTy8EeIH-rrftCxGeVnXg.png)

### Southern Hills

![Image](https://cdn-images-1.medium.com/max/800/1*wfVecaGOfwj9HjG-wh2KiA.png)

## Concluding Request

Some (or many) of the mountains that I list as "[Unknown]" might, in fact, be indeed known and have popular names. Please comment if you have information about them.

#### Article 240 · April 30, 2020

### CoViD19 in Sri Lanka

# CoViD19 "Recovery Rates"

### A Rough Analysis

As of 4/30 (morning), Sri Lanka had 649 confirmed cases of CoViD19, of which, 136 had recovered, and 7 had died.

![Image](https://cdn-images-1.medium.com/max/800/1*cv9hT_t6OlPwExGmLMo2Hg.png)

Do these numbers say anything about how Sri Lankan's recover from CoViD19?

More specifically, do they say anything about,

* What proportion of infected cases recover ("recovery rate")?

* How much time does recovery take?

This article is a rough attempt at a rough (and incomplete) answer to these questions.

## Data (and its Limitations)

In this analysis, I use data published at https://www.hpb.health.gov.lk. Here is a summary chart:

![Image](https://cdn-images-1.medium.com/max/800/1*s9Z63M-NWxH9KDuRI2WDmg.png)

How do we compute the "recovery rate"?

Ideally, we consider all the patients known to be infected on or before a particular date, and track their progress, until all have either recovered or died. The "recovery rate" is the number of recoveries divided by the number of total cases.

Unfortunately, we cannot compute this.

We do know "all the patients known to be infected on or before a particular date". This is the "Confirmed" number.

However, we do not know their progress. This is because all numbers are reported relative to the current date, not confirmation date.

For example, "136 had recovered by 4/30" includes every single "known to be infected on or before a particular date" — not a particular one.

## A Naive Approximation

We could compute a "naive recovery rate" as the ratio between "Recovered" as of some date, and "Confirmed" as of that same date. This is "naive" because patients take 2–3 weeks to recover from CoViD19.

Hence, a case "Confirmed" today might not recover for several weeks. Hence, the "naive recovery rate" significantly underestimates the recovery rate.

## A Less Naive (but still incomplete) Alternative

Instead of comparing "Recovered" to "Confirmed", we could compare it to "Confirmed" from some time ago; say 1, 2, 3 and 4 weeks.

Note, the "Confirmed (1 week ago)" line is the same "Confirmed" line "shifted to the right by one week. Similarly, "Confirmed (2 weeks ago) is shifted by 2 weeks, and so on.

We see that "Recovered" tends to lie somewhere between "Confirmed (3 weeks ago)" and "Confirmed (4 weeks ago)".

![Image](https://cdn-images-1.medium.com/max/800/1*gabqoPgDRnOZJ04cx-_exQ.png)

We can also compute and plot the ratio between "Recovered" and various shifted "Confirmed" numbers. "Recovery Rate (after x week)" is "Recovered" / "Confirmed (x week ago)".

![Image](https://cdn-images-1.medium.com/max/800/1*aMFUjXjW12YKpOsF77PnLg.png)

How do we intepret these results?

It's not straight-forward. This is why I qualify the "Recovery Rate" in quotes. The problem is with the "recovery window" we consider.

* "Recovery Rate (after 1 week)" is currently about 43%. Does that mean 57% of people will die of CoViD19? Of course not. The problem with this estimate is that the "recovery window" is too small. As I mentioned, recover takes 2–3weeks; sometimes more. So, most of the 57% are likely to recover in the future.

* "Recovery Rate (after 4 weeks)" is currently about 94%. The problem with this number is that the "Recovered" number is likely to have people who were infected with the disease after the "4 weeks ago" deadline. This is why "Recovered" is greater than "Confirmed (4 weeks ago)", and "Recovery Rate (after 4 weeks0" > 100%. Hence, a large "recovery window" is likely to overestimate the "recovery rate".

Is there some other window we can use? 2 weeks? 3 weeks? 2.5 weeks?

Sadly not. "In-between" recovery windows will also have the same problems associated with small and large windows to various extents. Hence, this metric, if not as naive, is also incomplete.

## Concluding Thoughts

I mentioned, that the "right" way to compute the recovery rate was as follows:

>>> ...we consider all the patients known to be infected on or before a particular date, and track their progress, until all have either recovered or died. The "recovery rate" is the number of recoveries divided by the number of total cases.

Sadly, even this number is likely to be wrong.

Because, the patients we choose to test is a biased sample. They are not a random sample of Sri Lankans. Currently, due to a shortage of tests, we only test people who are most likely to be infected (e.g. Display symptoms, in close contact with confirmed cases etc).

Hence, the "right way" would be,

>>> ...we consider all the patients known to be infected on or before a particular date, based off a statistically significant random testing sample, and track their progress, until all have either recovered or died. The "recovery rate" is the number of recoveries divided by the number of total cases.

## Appendix: Updated Graphs as of May 9th, 2020

![Image](https://cdn-images-1.medium.com/max/800/1*TSBKUApeoJWOsqsDvDwhaA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*bLjO0P946LTFRMBFS7hgug.png)

#### Article 241 · May 10, 2020

### Covid19

# CoViD19 Curves

### A Simplistic Summary of the Global CoViD19 Situation

If you are like me, you're probably overwhelmed with zillions of numbers, stats and dashboards about CoViD19. The goal of this article is to attempt a cure.

I create "A Simplistic Summary of the Global CoViD19 Situation", by doing the following

* For all countries (with at least 30 confirmed CoViD19 cases as of May 8), I plot the number of active cases, from the time active cases hit 30.

* For better visualization, I cluster countries by shape.

For simplicity, I chose five clusters. Here are the results.

Data Credits: https://github.com/CSSEGISandData/COVID-19 (the data repository for the 2019 Novel Coronavirus Visual Dashboard operated by the Johns Hopkins University Center for Systems Science and Engineering).

## Cluster 1 (Looking Great)

![Image](https://cdn-images-1.medium.com/max/800/1*JJPhrJTlBUnpYRPTBV0Njg.png)

## Cluster 2 (Looking Good, but too early to celebrate)

![Image](https://cdn-images-1.medium.com/max/800/1*PmY2xz009NaPEPhQ77E07w.png)

![Image](https://cdn-images-1.medium.com/max/800/1*HqNsonwbpkoZcx8DoqwOPg.png)

## Cluster 3 (Meh)

![Image](https://cdn-images-1.medium.com/max/800/1*rT9r9wlEnLj0emQQRcDOJg.png)

## Cluster 4 (Bad, but starting to get a bit better)

![Image](https://cdn-images-1.medium.com/max/800/1*eAu2WwNH8OdDOmbfcQijZw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*P6yVcEpsFskiidIeyAdjew.png)

## Cluster 5 (Still Bad)

![Image](https://cdn-images-1.medium.com/max/800/1*K6mhJwtw0cXJTxWCisRh9g.png)

![Image](https://cdn-images-1.medium.com/max/800/1*fHu0gNydURDpyIdte2NpZA.png)

## Huge Concluding Disclaimers

As I said, this is a simplistic summary. It hides valuable information like the "absolute number of active cases", or the " number of active cases per capital". Hence view with the appropriate pinch of salt.

#### Article 242 · May 19, 2020

# Managers & Bureaucrats

### And how to recognize them

## Managers and Individual Contributors

I joined Facebook, straight out of Grad School, as a Junior Software Engineer (SWE). "Junior" wasn't an official title. All SWEs Junior and not-so-Junior were "Engineers". For internal performance and remuneration purposes, I was an "E03". This "level" was private, and only visible to my manager, his manager and other "ancestor" managers, up to the CEO.

After some time, I got promoted to E04. My external title was still "Engineer", but my salary increased. "What was expected of me" also increased. My manager told me that E04 had to make 1.5x to 2x the contribution an E03 made. This ratio tended to be true for higher levels as well. It didn't necessarily translate into a similar increase in raw work. While it was true that most E04 SWEs would write more code than E03s, they also wrote "better" code. Code that did more by quality and not merely quantity. That made "more impact".

By the time I reached E05, in addition to writing code, I was also mentoring two other Engineers. While I mostly saw "mentoring" as answering questions, reviewing code, and generally nudging in the right direction, what I was effectively doing was helping these engineers make "more impact" themselves.

After I reached E06, I transitioned to management. Note, while my move from E05 to E06 was a promotion, my move from E06 to M01 (an entry-level manager) was not a promotion, but a transition. Sideways, not upwards.

E06s and M01s were "at the same level". They had the same salaries and had to make a similar sort of contribution to the company. How they made that contribution was different, though. While an E06 was known as an "individual contributor" (IC), the M01 managed a team (or sometimes two teams) of individuals.

[NOTE: I'm somewhat oversimplifying for clarity. Especially at senior levels, there were few "pure", 100% ICs or "pure", 100% Managers at Facebook. Both Managers and ICs wore the other's hat. Even as an E05, I did some of the "mentoring" types of "managing". "Impact" was evaluated by pro-rating the IC and Manager components of an individuals performance.]

## Management and Incremental Impact

Why did I transition to management? The reason was simple.

I believed that I could make more "impact" by enabling others. As opposed to being an individual contributor. I also framed this belief relative to promotions. The next level (E07 or M02) demanded the same level of impact. And I believed that I could make more impact as a manager than as an IC.

But what exactly is a manager's impact? An ICs impact is "what they do". The "individual contribution". A manager, on the other hand, makes impact through others.

So, is a manager's impact, the sum impact of their team? Not quite.

Each member of the team earned their impact. If we also credit the manager with this impact, we will be double counting. A manager's impact is the "incremental" impact their team made, over and above the impact they would have made without their support.

How to measure this "incremental" impact is its complex and fascinating topic. I'll leave that for another article (perhaps several). My main point is, a managers impact should be incremental.

## Bureaucrats

Sadly, many people who call themselves managers don't have an incremental impact. Some even have a "net-negative" incremental impact. In other words, their reports would have been better off without them. I use the label "Bureaucrats" to refer to these people.

How do you recognise a Bureaucrat? Here are some common patterns:

* Managers energise their reports. They find ways of making them better, in exciting and sometimes ingenious ways. I had the good fortune of having some fantastic managers at Facebook, and I remember leaving almost all of my one-on-one meetings with them with a new feeling of possibility and motivation. Bureaucrats suck the energy out of you. Just as you are not happy to meet them, they are not happy to meet you. Your encounters with them feel like a waste of time. Or merely, "a chore of the system".

* Managers always give you credit for your work. Especially in public. Bureaucrats don't. They might praise you in private, but in public, they tell everyone that it was their work. They claim your impact to be their "incremental" impact.

* When a Manager joins a team, it gets better. When a Bureaucrat joins a team, it gets worse. A particularly vicious type of Bureaucrat is one who jumps teams so that their weaknesses are not discovered. Often, they would join a successful team, take credit for the success (which should be due to the team, and, possibly, the previous manager), and then jump ship before it sinks. Usually, the next manager of that team takes the blame for the Bureaucrat's mismanagement.

* People typically join teams and even companies because of good Managers. Conversely, they leave teams and companies because of Bureaucrats. Often, if no one wants to work on a team, it's because a Bureaucrat manages it.

Happy Managing!

![Image](https://cdn-images-1.medium.com/max/800/1*ZtiqtPJ35pv8ll6tepuJKw.jpeg)

#### Article 243 · June 19, 2020

Great question.

The problem is a "bigness" of the idea. All big ideas tend to carry big risk.

The only "framework" I can think of to get around this is to try and break down the big idea into many small ideas. In parallel, if it is possible to test these small ideas very quickly, their low cost becomes even lower. This leads to the classic "test small + iterate fast" cycle.

#### Article 244 · June 19, 2020

# The Data Mafia

### And why we exist

![Image](https://cdn-images-1.medium.com/max/800/1*Ej7PudXet9WP_Uv4A4CKfA.jpeg)

Recently, a colleague accused me of being a "Data Mafioso". When I asked him to clarify what he meant, he said something like this.

"Whatever we say, you ask, ‘What does the data say?'. And when you learn that the data says nothing, you kill our idea."

## Red or Blue?

To make this more concrete, let us consider a (hypothetical) example of an idea.

Suppose you are designing the User Interface (UI) of a website. Suppose you want to decide what colour the "Accept" button should be. The default colour (that everyone seems to use for this type of button is "Blue"). But your designer believes "Red" is a better option.

So you do a "User Study" to figure out what colour you should use. You bring in seven potential users and show them the two options.

Now, suppose five think "Red" is better. Two think "Blue" is better.

Your designer colleague is triumphant. The data from the user study confirms his theory: 71% to 29%.

But does the data actually agree?

## What the data says

We use data to test theories. For example, we use the data from the "User Study" to test the "Red Button is best" theory.

How do we "test"? Data has no mind. It is not a human with subjective opinions. And so has no opinion on Red buttons and Blue buttons. So we can't ask the data "Is the Red Button best?". On the other hand, we can ask it to compare two different theories.

For example, we could ask, "Is the Red Button better than the Blue button?" Or to be more precise, we could ask "Does the User Study confirm the theory that the Red Button is better than the Blue button?"

Data answers this (more specific) question, but answering an even more specific question. "What is the probability that the User Study results occurred by chance?" Now if this probability is high, then we can't conclude that Red is better than Blue. In other words, "the data says nothing".

Now, if a user had an equal 50–50 chance of preferring Red or Blue, the possibility of a User Study with seven people picking Red five times or higher is about 23%.

Is 23% high enough? If we want to be very sure that the theory is correct, we tend to be conservative on what "probability is high" means. In other words, we pick a low limit for "high" — usually 5% or 10%. If we are less picky, we might choose a higher threshold like 20%.

## More Samples

The risk of putting a red button on a UI is probably low. So we could afford to be a bit liberal on how we use data. So while 23% is generally considered "high", we might cut some slack and use it in the UI.

There is a simple way around this. Show the button to a few more users. The more samples, the more sure data is. For example, if we had 14 users, and 10 picked "Red", the chance of a random result is down to about 9%. If we had 21 users, and 15 picked "Red", the random chance is down to 4%.

## Risk

But like I said, the risk of putting a red button is probably low. On the other hand, other situations can be more risky.

By Red-Blue example was inspired by a far more risky experiment. A prominent economist was proposing a particular development program for Sri Lanka. Seven other countries tried the same program. In five, the results were positive. In two, it failed. The economist was going around "pitching" the program's "success rate of over 70%".

I tried to explain that 5/7 was not enough. Pointing out that there is a high (23%) chance that the success thus far could be random. And unlike the red button, the program was costly — in terms of tax-payer money, and the opportunity cost of using that money for something else. Hence, we should have been more careful.

Sadly, the powers-that-be bought the "over 70%" pitch, and Sri Lanka became, not the sixth success case, but the third fail case.

## Theories upon Theories

Unlike Web UIs, where it is relatively cheap to run even millions of experiments, this is not true with large development projects. We can't run a $50M project in 30 countries, just to validate if the project would work. Hence, often we "override" the data with a high-level theory. We say the idea works because some theory says so.

In many cases, this works. For example, we know at what velocity and acceleration an apple falls to the ground. Because we have a higher-level theory. The laws of kinetic motion.

But in some cases, higher-level theories don't work. Because they themselves don't have enough evidence to back them up. You can only "replace data with a theory", if that theory itself is backed by data.

To confuse things further, some high-level theories are backed-up by even higher-level theories. Leading to end-less hierarchies of theories.

## #SkinInTheGame

Life is full of uncertainly. And sometimes we have to make decisions, without data. Not knowing if it would work.

Hence, we could have argued that Sri Lanka had to try the development project, even if the "data wasn't sure". However, when we do take such decisions, we should make sure that the decision makers and experts behind the decision take responsibility.

In ancient Rome, the engineer who designed a bridge had to sleep under it for some length of time. If the bridge collapsed, the engineer was killed. Similarly, experts should face some downside when their decisions turn out to be wrong.

While the Sri Lankan tax-payer is laden with more debt, the economist who proposed, the "Red" project is still a paid adviser to the government. He, sadly, had no skin-in-the-game. We took the punishment for his mistake.

## Concluding Serendipity

When there is a risk, we should trust the data as much as possible. And when data is expensive, we need to make sure that incentives are aligned. And that the appropriate people sleep under appropriate bridges.

On the other hand, when risk is low, we can ignore the data or interpret it liberally.

There is an even more extreme decision we could take. In the strange case of the red button, why did we choose between red and blue? Why not green? Or purple or black? Why did we accept the designer's theory? Real creativity comes from looking for solutions in a completely unconstrained manner. Maybe we should have implemented a button that changes colour randomly. Often the results could be poor. But if the risk is low, we could afford these "mistakes". On the other hand, we might also "stumble upon" a genuinely fantastic colour that no one else thought. Purely by chance.

A true Data Mafioso would understand all these factors. And the reason we (Data Mafiosi) exist is not to make sure data is used all the time. But, instead, to make sure data is used appropriately at the appropriuate time.

To summarise, the true Data Mafioso will make sure the following happens:

* Risky + Data is Expensive ⟶ Use Skin in the Game

* Risky + Data Not Expensive ⟶ Use Data Conservatively

* No Risk + Data Not Expensive ⟶ Use Data Liberally

* No Risk + No (Good) Theories ⟶ Forget Data, Forget Theories, Trust in Serendipity

#### Article 245 · June 21, 2020

# The Problem with Causality

### On Causality, Certainty, Process and Time

What do we mean when we say that "A caused B"?

We usually mean that there was some process, governed by a set of rules, that links A to B. And that A happened before B.

Hence, "causality" depends on two factors:

* Time

* A process, governed by a set of rules

## The Problem with Process

How do we know if processes happen? We "know" because of laws we've inferred about the universe. When we say that "A caused B", there are some laws that say that A must cause b.

Some of our "laws" are about abstract things. Like the laws of mathematics. If the two shorter sides of a right-angle triangle are of length 3 and 4, such a mathematical law says that the longest side must be of length 5.

Other laws about concrete things (like physical nature, biological systems, medicine, psychology, economics) base on empirical observations. When we observe many instances of A happened and then B also happening, we define a law that says "A causes B".

Strictly speaking, in the latter cause, we don't know if "A causes B". Our empirical observations only imply that "A correlates with B". This is the problem with process. There are no concrete processes where we know with certainty. Our knowledge of processes is purely correlation. Not causation.

## The Problem with Time

Physics defines time as the direction in which disorder in the universe increases. Or more intuitively, the direction in which information increases. For example, before you toss a fair coin, you don't know what the outcome will be. But after you toss the coin, you know (heads or tails). Hence, after the coin-toss, the amount of information in the universe has increased by one bit. This is the "pure" definition of time.

Now consider the following "points of time".

* Before A has happened

* After A has happened, but before B has happened

* After both A and B have happened

We can see how "information increases" with time when we observe what we know at each point in time.

* We don't know the answers to either question, "Has A happened?" or "Has B happened?"

* We know the answer to the first question, but not the second

* We know the answers to both questions

Now suppose that "A always and only causes B" is some universal law of nature. Then if A happens, we know that B will happen. Not necessarily instantly, but eventually. Hence, if we know the answer to the question "Has A happened?" we know the answer to the question "Has B Happened?". Hence, "After A has happened" we have all the information about the universe as if B has also happened. Thus, "purely speaking" there is "no passing of time" between A happening and B happening. We might as well say "B caused A".

Note, the more uncertainty, the more time. The less uncertainty, the less "passing of time".

## The Paradox

Hence, at one extreme we have "perfect certainty" where "A always and only causes B". In which case, there is no time. At the other extreme, we have perfect uncertainty, where there is time, but we can't say if "A causes B".

This is the problem with causality. Either there is perfect certainty, in which case there is no time, and hence no causality. Or else, there is no certainty, in which case the "process" that results in causality is flawed. In the middle we have an uncertain "no cause's land".

Conclusion?

Either,

"A and B cause each other with certainty, at the same instant of time."

Or else,

"The relationship between A and B is uncertain. We can't draw any "causal" inferences."

![Image](https://cdn-images-1.medium.com/max/800/1*fdfMIE8aqlBtkkGuG7aKWw.jpeg)

#### Article 246 · June 23, 2020

RE: Is knowledge impossible, or is pragmatism sufficient?

I'm assuming by "knowledge" you mean "absolute knowledge". As opposed to a "relative knowledge" (="pragmatic" knowledge), which depend on assumptions/context/simplifications, that plays an important part in pragmatic applications (as you described).

The latter ("relative knowledge") has been both useful and sufficient for many applications.

The former is, at best, itself a special case of the latter. Where we say something like "Given these assumptions/context/simplifications this knowledge is absolute".

At worst, the former is a delusion. Historically, this type of "knowledge" has been "defended" less by reason, and more by ignorance or violence.

#### Article 247 · June 25, 2020

# On Compassion

When a loved one is in pain, sad, or suffering, I tend to feel that suffering. I was told that such a reaction is not a bad thing. It is a good thing. And its called Compassion.

But the problem I have with Compassion is that, sometimes, it feels bad. As my loved one suffers, I suffer in parallel. And this feels bad.

And how can a good thing feel bad?

## Evolutionary Compassion

Just as hitting my thumb with a hammer causes physical pain, a loved one's in pain induces some form of physical pain in me.

There might be evolutionary roots to this reaction. My thumb was painful because that would alert me to the sickness, and possibly induce me to take curative action.

Similarly, the pain of a loved one would induce me to do something about that pain. Helping the loved one would cure their pain, and hence mine. And indirectly help me. Perhaps not immediately, but in time.

## Pseudo Compassion

But there seems to be another source of "compassionate pain" which is less constructive.

When a loved one or I am in pain, sometimes I consider the pain or the circumstances that led to the pain as unjust or unfair. I think to myself "My loved one is not the sort of person who should feel that pain. Why? Because they are "my" loved one. How unfair!!!"

Note, this type of thought assumes that "my world" operates according to specific rules: "My rules". Including those that say that "I and mine should not suffer".

This sort of thought is destructive because it is based on unrealistic assumptions. That normal things are not normal.

## Beyond Pain

On reflection, it feels to me that much of my pain comes from Pseudo Compassion. And when I let go of my unrealistic expectations for the world, this pain disappears.

On the other hand, while Evolutionary Compassion might be temporarily painful, it leads to constructive action, which, at some level, leads to a lessening of pain for both me and my loved ones.

Evolutionary Compassion seems to be like a rudimentary form of a broader, more general and perfect compassion. What if this basic instinct that only applies to loved ones can be expanded to a much broader set?

What if one felt "Everyone's pain is my pain"? How constructive might that be?

![Image](https://cdn-images-1.medium.com/max/800/1*M5kemwRiBf5nO_3FBn0WmQ.jpeg)

#### Article 248 · June 25, 2020

# The Marketing Algorithm

### And the Importance of Smart Marketing

Fifteen years ago, some friends of mine built a translation system. That would translate English into Sinhala. They "exposed" the system via an API ("application program interface") so that other people could also use it.

When a journalist asked my friends "whether the system was valuable", they replied that it was "fairly valuable". Especially for those who "wanted a tool to translate English into Sinhala".

The API is still available today (I think). But I doubt anyone uses it. If you want to translate English into Sinhala, it is much easier to use Google Translate.

![Image](https://cdn-images-1.medium.com/max/800/1*zMX19zF_8t5-ruR1ASK4wQ.png)

If you were expecting yet another story of how Google killed a promising startup, sorry. This article is not one of those. To begin with, my friends were not a startup. They all had "day jobs", and the project was just a hobby.

Instead, this article is about "Value". More specially, how people (like my coder friends) routinely underestimate the value of products (like the translation system); Why this mis-underestimation happens; And how to avoid this mistake.

## Reductive Value

All "goods" (i.e. product and services) satisfy needs. The "value" of the good is proportional to this "need", and also relative to all other needs a person has. Often goods don't satisfy needs in isolation.

For example, the product "salt" is commonly used with the products "pepper", "chicken" and "cooker", and service "cook". They combine to satisfy the need of "hunger". In this way, goods don't produce isolated value, but are part of "value chains".

By Reductive Value, I mean "describing the value of a good in terms of its contribution to the value chain". When my friends described their product as "a tool to translate English into Sinhala", they were doing exactly this. There was no reference to other goods or value chains. Nor an explicit reference to needs.

## Expansive Value

About a year after I first learnt about my friends' translation system, I met a man who described himself as an "entrepreneur". When I asked "Mr. Entrepreneur" what he did, he said his latest product was about "connecting Sri Lanka to the internet". At first, I thought he was trying to build some extensive telecommunication system. Or distribute free computers to our rural poor.

When I asked him if that's what he was trying to do, he shook his head, opened is a laptop (enormous by today's standards), and played a fuzzy video.

The video looked like a screen-capture of someone opening a browser, then going to the yahoo news website, and finally opening a New York Times article. Surprisingly, the article was written not in English, but in Sinhala.

Mr. Entrepreneur's strategy for connecting Sri Lanka was a web-browser. That translated all text from English to Sinhala.

[While this might seem a bit of a sham, it does make sense if you think about the numbers. Even today. Only about 10% of Sri Lankans are fluent in English, while over 70% have access to internet broadband.]

The video I was not of a real browser, but an animation of one. Mr Entrepreneur was still looking for a programmer to build his idea. I don't know what happened to him, but I was intrigued by his idea.

Engineering-wise, his product was the same as what my friends had built. But while my friends described their product as a humble "tool", Mr Entrepreneur framed his product as a grand vision for completely changing how the internet is used in Sri Lanka.

What intrigued me most was the difference in framing. Mr Entrepreneur considered a value chain (accessing the internet) where his product was a small (but essential) link. Then went on to expand the description of the value of his product in terms of the overall value of the chain. This is what I meant by "Expansive Value".

## But isn't this cheating?

Mr Entrepreneur had something of the air of a charlatan. With his big talk and fake videos. My friends, on the other hand, were naive software engineers. As honest as they come.

And weren't they more honest to describe their product in terms of precisely what it does? As opposed to something much larger? That depends. On what the point of the description is.

Honest and objective descriptions are all good. But at the end of the day, goods satisfy needs. And the description should describe the need, not just the good. My friends' description made no explicit reference to needs. Conversely, Mr Entrepreneur's "expansion" was not dishonest. Instead, he was doing what was necessary. Framing the good in terms of essential needs.

## Dumb Marketing and Markerters

In the Technology field, we tend to respect a solution more than we respect problems. We tend to appreciate "goods" (especially if they are complex and esoteric) more than we respective descriptions of needs that the same goods might satisfy.

Hence, how my friends behaved was utterly normal. They had built a solution and expected the requisite respect. What need the solution satisfied was someone else's business.

In Tech, these "someone elses" tends to be "marketing people" and other low-life. Undeserving of respect. Because they don't have to do difficult things. Like engineering.

This pre-judgement has become a self-fulfilling prophecy. Marketing departments are mostly communication departments for "translating engineer-speak" into language that "ordinary people understand". In other words, they are conduits for communicating "Reductive Value".

As a result, marketing departments tend to be underfunded, and comprise with dull and uncreative people. A vicious cycle that perpetuate the myth that marketing and marketers are dumb.

## Smart Marketing and The Marketing Algorithm

Instead, Marketers in Tech should instead be looking to maximise the "Expansive Value" of what is built. Or even better, what should be built.

If maximising Reductive value is hard, maximising Expansive value is even harder. It requires understanding the complex economics of value chains and a keen understanding of human behaviour and psychology. It consists of identifying every single value chain where a product might be a link and determine what value chain is most valuable.

This sort of "Smart Marketing" is what marketing should be.

Let me conclude by reframing the difference between reductive value and expansive value in a form techies would understand. Enter "The Marketing Algorithm".

```
def get_reductive_value(good):
```

```
"""This is what engineers maximise"""
```

```
return "value of the good in isolation"
```

```
def get_expansive_value(good):
```

```
"""This is what marketers maximise"""
```

```
max_value = 0
```

```
for value_chain in all values chains where good is a link:
```

```
max_value = max(
```

```
incremental_value of good in value_chain,
```

```
max_value       )
```

```
return max_value
```

## Acknowledgements

In his excellent book, Alchemy, Rory Sutherland describes "Expansive Value" as magic. Finding it is indeed a more "magical" process than merely engineering Reductive value. Mr Sutherland's ideas have significantly influenced this article.

![Image](https://cdn-images-1.medium.com/max/800/1*qWVfe61Ocvv7QdnoJhYSuQ.jpeg)

#### Article 249 · July 1, 2020

# Are you AI prepared?

### From first principles

"Are you Artificial Intelligence (AI prepared)?" is one of the most hyped questions on an already highly hyped topic.

At the same time, it is a very pertinent and timely question. I know this because many people ask me how their organisations can be more "AI prepared". Sadly, many also qualify the question with "whatever that means".

Answering the "Are you AI prepared?" is big business. Consultancies take millions to "study your organisation" so that they might produce a report that evaluates your "AI Preparedness". Oddly, a lot of the people who ask me the "Are we prepared?"-question, have already commissioned (and sometimes even read) such reports about their organisations. And yet they still ask the question.

The problem with the "Are you AI prepared?" question is that while many consider it important (and it is important), few have good answers. The goal of this article is to solve this problem. Provide a reasonably good answer.

"How can you succeed, where multi-national consultancies have failed?" you ask. Well, read on. If I provide you with a good answer, you will know for yourself.

...

Whether or not you are "AI Prepared" depends on the answer to two questions. We will consider each next.

## Are you Data Prepared?

People say there is an AI revolution. There is no AI revolution because most of the ideas around AI are old ideas. Some over 50 years old.

The real revolution is not in AI but in data. Data can be collected at rates and efficiencies never known before. The same applies to transporting data, storing data, and processing data. These revolutions in sensor, network, storage and processing technology have driven the "Data Revolution". If there is an AI Revolution, it has merely piggy-backed on this data revolution. For example, the theory behind Deep Learning is over 50 years old. But the data revolution has made it practical. Hence, if you are not Data Prepared, you are not AI Prepared.

What does it mean to be Data Prepared? Let me explain with a simple example.

Suppose you run a small shop. Each day customers walk and buy whatever they want. And once a week or so you replenish your inventory, and dispose of old stock. Each time someone buys something, you might enter the transaction in an exercise book, and you do similar "book-keeping" with replenishing and disposing of inventory.

In this "pre-digital" example, there is still much data. Most of it recorded on paper. "How data prepared you are" depends on what proportion of your data is in a form AI systems can process. If all your data is in such a form, then you are "100% data prepared".

Even today, many organisations are like this "pre-digital" shop. A lot of their data is on paper. Often, even data which is in some digital form cannot be easily processed by AI systems. Hence, "becoming data prepared" consists of transforming data collection and storage into an AI friendly format.

## Are you Decision Prepared?

Suppose our shop-keeper becomes 100% data prepared. She replaces the "exercise book" with a "digital inventory system". Now, every piece of data in the business is not only digital but "AI-systems friendly".

But now what? What's the point of all this data? To answer this question, we must first understand how AI uses data.

Most of AI is about using data to answer questions. If you have millions or billions of pairs of questions and answers, you can "train" in AI, to answer new questions. For example, if you have many pairs of human faces along with the name of the human, you can train an AI (a.k.a. a Face Recognition system), to answer the question "Who is this human?" given a picture of a face. Similarly, our shop-keeper could answer the question, "What inventory should I purchase?" given (inventory, "How much of that inventory sold?") data.

Hence, the power of AI comes from using it to answer questions that your business cares about.

Let's again consider our shop-keeper. She cares about maximising profit. She does this by selling goods that her customers want. And not selling products that her customers don't want. Hence, she has to make two decisions:

* What products to sell, and how much?

* At what price to sell the products? (Note, even products that customers want must be sold at the right price. Too high, and no one buys. Too low, and she makes a loss.)

Both these questions can be answered by an AI system that trains on the data that our shop-keeper already has. And if she uses such an AI system to answer both questions, we could say that she uses "AI optimally to make decisions".

This is what I mean by "decision preparedness". Whether you know what decisions you want AI to help you with, and whether you are using AI to help make those decisions.

If you are using AI to help you with all your decisions, you are 100% Decision Prepared. And if you are both 100% Data Prepared and 100% Decision Prepared, you are 100% AI Prepared.

## But I'm not a Shop-Keeper

"But I am not the small shop-keeper on the corner", you say. "My business is worth billions." Fair point. How do we go from small to big?

The principle is the same. If you run a large organisation with many parts, you need to break down the organisation and its decisions into smaller chunks. And ask the "Data Preparedness" and "Decision Preparedness" questions for these subsets. Then you can aggregate the results for an "aggregate preparedness" for the company as a whole.

We could even go beyond this. And aggregate multiple organisations or even a whole country.

## What Next?

If you run (or are part of) an organisation, and want to know if it is AI Prepared, I'd recommend trying and answering the Data Preparedness and Decision Preparedness questions for at least a small subset of your business.

After you identify some subset with an untapped opportunity, you could try and solve the problem (at least partially) using AI. Once you realise some value out of the exercise, you could move to other parts of the organisation.

"But wait!", you say. "We don't have any AI expertise. We don't have the people, and we don't have the technology".

That's ok. The hardest step is the first step: The Data Preparedness and Decision Preparedness questions. And, happily, you don't need any knowledge of AI (or AI people or technology) to answer these questions. All you need is a good understanding of your business (which, hopefully, you have). Once, this first, difficult step is complete, hiring people and building technology is easy (relatively). I will share my thoughts on these later steps soon, but in the meantime, you should worry about the first step.

So, are you AI Prepared?

![Image](https://cdn-images-1.medium.com/max/800/1*fVBVWFDm6j00Myn6CVa3aQ.png)

#### Article 250 · July 6, 2020

RE: Also, in the proposal to recalibrate it, would the recalibration happen prior to every election?

I believe it is calibrated before each election.

RE: And should there be other factors other than number of voters? e.g. perhaps poorer districts should have more representation?

Other factors do influence it. That mostly explains the disproportions. See https://en.wikipedia.org/wiki/Electoral_districts_of_Sri_Lanka for details.