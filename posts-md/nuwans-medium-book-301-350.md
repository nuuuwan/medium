# Book 7

#### Articles 301 to 350

#### Article 301 · January 12, 2021

### On Machine Learning

# Three Modes of ML Pipelines

### And How to improve the performance of ML Pipelines

"What does an ML Training Pipeline look like?"

In theory, in its simplest form, you train a model based on some data. In practice, all but the most trivial ML systems include a few more steps:

* The raw data might need some preprocessing, and before you do that, you might need to inspect the data.

* You might have to choose what Model to use and set the various hyperparameters of the Model.

* After training the Model, you would want to evaluate it and inspect the results. Any learnings from this inspection process might influence the previous two steps.

* You iterate, until the model is satisfactory.

![Image](https://cdn-images-1.medium.com/max/800/1*aX4gUw685lK2OA7j4x9LFA.png)

While even this more elaborate pipeline is somewhat simplistic, it is sufficient to explore my next question, namely, "How might we improve the performance of this ML Pipeline?"

Broadly, there are three ways:

* Better Data. ML consists of "learning" patterns in past data and using this knowledge to make decisions about the future. For example, learning how to give better product recommendations to a customer on an e-commerce site, based on that customer's and other customers' past behaviour. Better past data, usually helps you make better decisions about the future.

* Better People. Several steps (inspecting data, model choice, inspecting results) benefit from human intelligence, knowledge and experience. Hence, the more intelligent, knowledgeable, and experienced people you have working on your ML systems, the better results you will get.

* Better Process. While a pipeline might feel "linear" our ML Training Pipeline contains a feedback loop. Once you train a model, you evaluate it, inspect the results and iterate; until you have a good enough Model. The better you do this, the getter your models will be, and, hence, the better the performance of your ML Pipeline. In the case of this process, "better" mostly means one thing: "faster". ML is a "search" for the best Model. And the fast you can iterate, the faster you do this search; and the quicker you'll reach a better model.

Which brings us to my third question: "How might we iterate faster?" This question finally brings us to our title topic: "Three Modes of ML Training".

The "Three Modes" are three contrasting yet complementary ways to run the ML pipeline. When used together, they enable fast iteration, and as a result, more performant ML Pipelines.

## Test Mode

What are good qualities would you expect from Unit Tests?

Firstly, you'd want them to execute quickly (i.e. in a few seconds). If it took several hours for your tests to run, you'd probably give up and do something else. Secondly, you'd want them to execute "seamlessly"; for example, it would be convenient if the tests ran automatically each time you made a change or a commit; without you having to run the tests manually.

What have Unit Tests got to do with ML Pipelines?

A significant proportion of ML consists of basic software engineering. Many ML practitioners, especially those who consider ML somehow more superior to "plain programming" don't want to admit this, but this is, nonetheless, true. You can't build efficient ML systems if you aren't a good software engineer (SWE). A good SWE is not just someone who writes good code, but also someone who follows other best practices like Testing.

Sadly, while Testing is vital for ML Pipelines, it is often completely ignored. The only Testing is "testing in production". You know there is someone wrong with your ML Pipeline when it crashes.

ML Training in Test Mode consists of the following: You run every step of the ML pipeline as if it were a test. "As if it were a test" means the following:

* Since tests should execute quickly, you modify any steps that take a lot of time. The most obvious source of slowness in an ML pipeline is the size of data. There is no way you can execute the pipeline in seconds if you need to crunch Terabytes of data. Hence, in Test Mode, you test the pipeline on a small amount of data, say a few thousand rows.

* You will have all the "hooks" in place to ensure that the pipeline runs in Test Mode each to a significant change is made.

* You don't expect the results of Test Mode to be of high quality. For example, a Model trained in Test Mode would not be perfect. However, you won't expect it to be complete garbage either. Hence, you can write UnitTests to validate the pipeline's various steps (like the Model produced).

## Human Mode

As we saw earlier, there are several steps in the ML Pipeline that depend on human intelligence. Human Mode makes it as easy as possible for the humans in the loop to be as intelligent as possible. Let's look at each of the human steps in more detail.

* Inspecting Data. In most ML systems, raw data is stored in vast data lakes, often on specialized servers in the cloud. While these are optimized for storage and processing, they are not optimized for humans. It is not easy for a human to get an intuition for the data on these specialized data sources. When I want to get a "feel" of the data, I download a few thousand rows of data to my local machine and use a combination of standard tools (e.g. Excel) and custom scripts to slice and dice the data. If the data involves images, video, audio and media, I will build a basic dashboard for inspecting the data.

* Model Choices. When you first tackle an ML problem, you usually don't know what algorithm is best. For example, you might want to choose between Boosting and a Neural Net. Even for a single type of algorithm (say a Neural Net), you might not know what Hyper-Parameters (e.g. The number of layers) are optimal. Human mode should make it easy to A) try out, and B) validate many choices quickly. "A)" is enabled by different algorithms having a common interface. "B)", similar to Test Mode, is enabled by training and validating models on a smaller set of local data. You could afford a little more time for the models to train than in TestMode; but you can't afford hours, as the humans involved would get bored. Hence, like the data inspection step, you'd want your data to live locally, or in someplace where access is fast.

* Inspecting Results. In many ways, this is similar to Inspecting Data. You want the humans in the loop for getting a sense of how the models are doing. This involves looking at the data in more detail than a few performance metrics. For example, judging a model on False Positive/Negative Rates or a Confusion Matrix might be insufficient. Instead, the human inspector would want to see what types of features led to False Positives, and what led to Negatives. Like Inspecting Data, this would involve a lot of visualization, custom dashboards and slicing/dicing at will.

There are more and more automated Test Mode tools, but few effective tools for Human Mode; probably because each human and ML problem is different. Humans need to be allowed to apply creativity and adapt. The best ML organizations are those that perfect Human Mode.

## Production Mode

Production Mode is the final Model in the ML Pipeline. By this time, almost all the productive work is complete. Test Mode ensures that the code and other steps work properly. Human Mode ensures that humans have applied their human intelligence and expertise to solve the problem. All that remains is to train the final production model. This almost always involves running the entire pipelines just once, without iteration. These steps rarely need to repeat, or we need to go back to the Human or Test Mode, usually when some specific data breaks the pipeline.

Sadly, many ML pipelines operate only in Production Mode. "Testing in Production" slows down development significantly, and the lack of Human Mode means that models are hardly optimal.

## Some Concluding Thoughts

Having different modes requires some initial investment and thought, but is well worth it — the gains in speed more than make up for the initial cost. Also, many of the principles behind these "modes" make future development more efficient. For example, adhering to "common interface" described in Human Mode make it easy to apply the same pipeline to new problems. Contrastingly, when the only mode available is Production Mode, pipelines need to be rebuilt for every problem.

The organizations that have perfected the "Art of the ML Pipeline", have completely Automated Test Mode and Production Mode. Hence, humans only need to focus on Human Mode; which makes sense because that is the step that depends on Human Intelligence. They also tend to attract the best human ML experts because such experts have the opportunity to exercise their expertise and creativity. In contrast, organizations stuck in Production Mode force their humans to be machines, and waste time drudging in mundane tasks.

#### Article 302 · January 20, 2021

# Parts of Mind

### Experiencing, Thinking, Remembering, and Identifying

## Experiencing

I can see a flag waving in the sea breeze.

When I see the flag, I see its colour. I experience it. This "experiencing" is, I don't doubt, carried out by some part of my Mind. Let me collectively refer to it as the "Experiencing Mind". Now, I don't know where this experiencing Mind is situated; whether in my brain or somewhere else; or even if it takes a physical form. For now, let's just consider it a label.

## Thinking

This flag that ways in the sea breeze: Is it Red or Orange? Could it be either?

As I mentioned earlier, I can see the flag. I experience its colour. I don't try to "name" the colour; or abstract it into some category of colour; like Red or Orange. Until now, while the flag was some colour, I hadn't formed an opinion on which colour.

Now, when I ask myself whether the flag is Red or Orange, I slot the flag into the set of things that are Red; or Orange. By choosing "Red", I have divided the universe into two sub-universes. In one, the flag is Red; in the other, not Red. And I've chosen the Red sub-universe as reality.

All of the above, again I don't doubt, must be happening in my Mind. Let's label whatever part of the Mind where these happenings happen as the "Thinking Mind".

## Remembering

I have a confession to make. I don't see a flag, and I'm not by the sea.

But the "Experiencing" and "Thinking" that I describe above are real enough; because these are things that I have actually experienced and thought some months ago; when I was, indeed, by the sea. What I'm describing is what I remember.

This remembering is also happening somewhere in my Mind. Let's call this part the "Remembering Mind".

## Identifying

So I think I possess an "Experiencing Mind", a "Thinking Mind" and a "Remembering Mind". Do I have any other sorts of Mind?

A few hours ago, I was having a debate with myself. I was debating whether or not I should write this article. A couple of times, I was tending towards not writing this article; particularly since I had other things to do. But not going to write this article, caused me some slight pain or irritation. Why?

Well, something in me told me "I'm the sort of person who writes articles like this"; and if I don't write this article "I will deny some part of my self". In other words, I was "identifying" with writing this article.

Now, no doubt, this identifying also happened in my Mind. So why not label that also? As the "Identifying Mind"?

![Image](https://cdn-images-1.medium.com/max/800/1*wx1300uKGXauej4UtUa2aw.jpeg)

#### Article 303 · February 16, 2021

# On Generalized Racism

### Definition, Examples & Exercises

## From Racism to Generalized Racism

The OED defines racism as:

>>> Prejudice, discrimination, or antagonism by an individual, community, or institution against a person or people on the basis of their membership of a particular racial or ethnic group, typically one that is a minority or marginalized.

Let me define generalized racism as:

>>> Negative treatment of a person or people based on their membership of some group.

The latter definition generalizes two characteristics of the former, namely,

* C1: What negative treatment constitutes racist treatment

* C2: What groups constitute as racially relevant groups

Both these characteristics must meet the racist bar, for the treatment to be considered racist.

## Illustrative Examples

For example, consider the following statements:

* A. Alice doesn't serve Black people at her shop

* B. Alice doesn't serve people who are not her friends at her shop

* C. Alice doesn't serve people who are not her friends the special drinks in her special drinks cabinet at home

Example A satisfies both C1 and C2. Most people would agree that "not serving someone in a shop" would meet the racist treatment bar. And also that Black people are a racially relevant group. Hence, most people would agree that Alice's behaviour is racist

Example B, satisfies C1, but not C2, and is hence not racist, though many would consider Alice's behaviour still abhorrent at some level.

Similarly, Example C satisfies neither C1 nor C2, and is, hence, not racist. But like B, many would agree that there is still something unpleasant about Alice's behaviour; not as significant as Example B, but unpleasant none-the-less.

## Optional Exercises

Hence, let me leave you with the following questions:

* Which concept do you find easier to understand: Racism or Generalized Racism?

* Which behaviour do you find easier to avoid: Racism or Generalized Racism?

* In general, is racism worse than Generalized Racism? Or vice-versa?

* Are any types of Generalized Racism acceptable in society? What types? Why? (Feel free to define what you mean by society if it might be helpful)

* Are any types of racism acceptable in society? What types? Why?

![Image](https://cdn-images-1.medium.com/max/800/1*NQ8x4_VYDH0zyVuRKRCD7Q.jpeg)

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

#### Article 305 · February 21, 2021

# What is Artificial Intelligence (AI)?

### Another attempt at a definition and other ramblings

"What is AI?" you ask.

"I don't know.", I reply. "It's not something I think about often."

"But don't you earn a living out of AI?"

"Well — yes.", I muse. "But that's like asking a Taxi Driver about an internal combustion engine or continuously variable transmission (CVT). You don't need to know how a car engine works to earn a living out of a car."

"A Taxi Driver might not know. But an Automobile Engineer will. Are you saying that you're more like a Taxi Driver when it comes to AI?"

"No, no", I reply hastily. "I do think about what AI is — sometimes."

"So then, what is it?"

## Chess

"Well, it's complicated. Artificial is easy enough to define. Intelligence is harder."

"Is it? I know what I mean when I say that my ten-year-old niece is intelligent. What's the difference?

"Well — what do you mean when you say your niece is intelligent?"

"Well — she does intelligent things. She can play Chess, for example."

"How did she learn to play chess?"

"I taught her"

"How?"

"I first taught her the names of all the pieces. Then, where they go on the board. And finally, what moves the pieces make."

"Anything else?"

"Well, after a few games, I taught her to "look ahead" for a few moves. Not to move her Bishop, for example, because it would expose her Queen."

"A computer that plays Chess is the same. It knows the rules, and it can look ahead for the best moves. The most powerful chess computers can look ahead for billions of combinations of moves."

"What you're saying is that the Computer is intelligent because it does things that make humans intelligent?"

"Sort of. Some AI experts defined AI this way. As in, "Computers that can do human tasks considered intelligent".

"Is that what AI is?

"I don't like that definition because it is "relative" to Human Intelligence. And we don't define what Human Intelligence is either. It is also subjective. If playing Chess is intelligent, what about playing Tik-Tak-Toe? Not everyone might call a Tik-Tak-Toe playing computer an AI."

## Expanding Data

"Do you have a better definition?"

"Well, we could think about what a Human or a Computer does when it does a supposedly intelligent task?"

"Like "thinking ahead"?"

"Exactly. The intelligence of playing Chess seems to come entirely from thinking ahead. You start with the rules and expand this to millions of combinations of Chess games."

"And this is intelligent?"

"Yes — at least it is the essence of intelligent."

"Thinking ahead?"

"Well, thinking ahead is an example of the essence. The essence is taking some data, like the rules of Chess, and expanding it to more data, like millions of combinations of future games, which will tell you what the best next move is."

"So AI is Machines extending data?"

## Cats and Dogs

"That's the essence. Let me give you another example: Recognizing Cats and Dogs."

"Like an AI that can tell Cats and Dogs apart?"

"Yes."

"How do these "Expand data"?"

"Well, you train a model that can tell the difference, using millions of examples of images of Cats and Dogs, labelled CAT or DOG. "Training a model" consists of building a mathematical function that transforms the image into some other representation which can accurately represent either CAT or DOG."

"But where is data expanded?"

"The model is an expansion of the training data."

"But is this ability intelligence? A child can learn to recognize a Cat or a Dog after seeing just one or two animals. Why can't a Machine do the same?"

"I think that's because the child has mostly learnt to recognize Cats and Dogs before it is born."

"Before? How is that possible?"

"Well, the "model training process" in humans has happened through millions of years of evolution. Most of the model is complete. Only the very last step is necessary. That is why just a few examples are sufficient. That's because millions of our ancestors have already seen millions of Cats and Dogs."

## Technology

"So, what drives AI? How come AI has developed so fast in the last couple of decades?"

"It's because Machines have got better and better at data expansion."

"How?"

"Take the example of the Chess Computer. The algorithms for "looking ahead" are relatively simple and have been around for years. It's just as computers have got faster; it's possible to look ahead for more and more moves."

"I see. And what about Cats and Dogs? Are Object Recognizing AIs also running faster algorithms?"

"Yes. We can train models quicker. A model that previously took many years now takes a few minutes. But it's not just faster models."

"What else?"

"There's also been an explosion of data. Even if we could train models fast, they would not work without millions of Cat and Dog photos. And if platforms like Facebook and YouTube didn't have these photos and videos, it would not have been possible to train models."

"So how come YouTube have so many Cat videos?"

"Well — a combination of many things. Advances in technology have led to bigger data stores, faster networks, and ubiquitous devices like Smartphones, all of which are also much cheaper. As a result, products like YouTube and Facebook, which encourage humans to post Cats and Dogs, also become possible."

"So, it is all about technology?"

"Yes."

## Human Intelligence

"So tell me something: Do you think computers are more intelligent than humans? Will they ever be?"

"I don't know."

"But why? How can my 1.5 Kg brain be more intelligent than millions of racks of computers combined?"

"Why did you mention your brain?"

"Isn't that where all the intelligence happens?"

"How?"

"Isn't that where all the processing happens? And where we store our memory?"

"Well, we don't know that for sure. We know that humans can use memory sources outside our bodies, like taking notes in a notebook. Hence, the whole universe could be a sort of memory, and I don't know what fraction of it we use and what we don't use. The same applies to processing. We don't know where exactly "processing" happens. Most of our processing is subconscious, and we don't even know where the conscious part happens."

"Will machines start using the universe as a memory? They seem to be doing that with things like the "Internet of Things"."

"Yes."

"So why do you think machines will never be as intelligent as humans?"

"I didn't say that. I said — I don't know."

"Why don't you know?"

"Well, because I don't think that I or anyone else knows exactly how intelligent humans can be. And if we don't know that, how can we say that something else (like a machine) will be more so?"

"So you think humans might be capable of being more intelligent that they are? To use your definition, they might be able to "expand data" more than they are already doing?"

"Yes."

"How?"

"I don't know. But we should be more interested and enthusiastic about questions like this."

"Like we are interested and enthusiastic about AI?"

"More so!"

![Image](https://cdn-images-1.medium.com/max/800/1*IIWYQHakviPAQ9UnIiHjKw.jpeg)

#### Article 306 · February 22, 2021

# Charities in Sri Lanka

### A very rough audit

I've been searching the web and elsewhere for a list of Sri Lankan charities. The best I could found was this list of 81 approved charities on the Inland Revenue Department Website. It was last updated in December 2019 — so there might be some charities not on the list.

This article is a summary of my findings.

## Donate Online

The most important thing I wanted to learn was whether it is possible to donate to a charity online via a Credit Card or other service.

Sadly, only 5 of the 81 charities had this option.

* ​HelpAge Sri Lanka (https://www.helpagesl.org/)

* Prithipura Infants Home (https://www.prithipura.org/)

* SOS Children's Villages Sri Lanka (https://www.soschildrensvillages.lk/)

* Sri Lanka Cancer Society (https://www.slcs.lk/)

* St. Joseph's Educational Foundation for the Hearing Impaired (https://www.candleaid.org/our-projects/completed-projects/st-josephs-school-for-the-hearing-impaired/)

## Donate Offline

The next best option was to donate offline via bank transfer.

In addition to the 5, which had the online option, another 12 websites had an option to pay via bank transfer.

* Canadapura Children's Home (http://canadapura.com/Projects/CanadapuraVillage)

* Centre For Handicapped (http://www.cfhsrilanka.org/)

* Colombo Friend-in-Need Society (https://cfins.org/)

* Colombo Young Men's Buddhist Association (https://colomboymba.org/

* FRIDSRO Children's Home (https://www.facebook.com/FridsroSriLanka)

* ​Hospital Services Council (https://hsclk.org/)

* Seemasahitha Matara, Arogya Seva Samithiya (http://arogyasewa.org/)

* Siyane Korale East — Social Service League Obesekara Elders Home (http://www.achome.lk/)

* Sri Lankadhara Society Limited (https://srilankadhara.org/)

* The Ceylon Moor Ladies Union (https://www.cmlu.lk/)

* Udaya Children's home (http://www.udayalamanivasaya.org/)

* YMBA Maharagama (https://www.ymbamaharagama.org/)

Disclaimer: I have not checked if the transfer details are legitimate or accurate. If you plan to donate, more diligence is advised.

## View Website

Another 23 charities had some information online, usually via a Website or Social Media page, though no visible method for donations.

* All Ceylon Buddhist Congress (https://www.acbc.lk/)

* Cancer Care Association — Sri Lanka (https://cancercaresl.com/)​

* Ethanamadala Sahana Elders Home (http://sahanaudaya.org/)

* Hindu Bord of Education (http://www.thehinduboard.org/)

* Hindu Women's Society Limited Colombo (https://www.facebook.com/CYWHA/)

* Isha Athul Islam Home for the Orphans (https://www.facebook.com/pg/ishaathulislam)

* Kalutara Bodhi Trust (https://www.kalutarabodhiya.org/)

* Kanadarawa Thapowana Vihara Building Fund (http://www.thapowanaya.org/)

* Kandy Friend-in-need society (http://kandyfriendinneed.blogspot.com/)

* Little Sisters of the Poor (https://mclloydbis.com/profile/237768/little-sisters-of-the-poor.html?fbclid=IwAR3Xnr6tWDPCO40pO-vJPdEkOQ4V5959e58lXcP6s5ghaGVrKuqmMfqV2JU)

* Mallika Nivasa Samithiya (Society) Limited (https://www.mallikahomes.org/)

* Moors" Islamic Cultural Home (http://www.michsl.org/)

* ​Moratuwa Social Service Society (Elders Home) (https://homeforelders.wordpress.com/contact-us/)

* Ramakrishna Sarada Mission (https://rsmlanka.webs.com/)

* Rohana (blind, deaf )Special School and Hostel (https://www.rohanaspecialschool.org/)

* Sahanoda Elders Home (http://www.sahanaudaya.org/)

* Saviya Development Foundation (https://www.peaceinsight.org/en/organisations/sdf/)

* Seemasahitha Sarvodaya Suwasetha Seva Samithiya (https://www.sarvodayasuwasetha.org/)

* Shilpa Children's Trust (https://shilpa.org/)

* Sisters of Charity of Jesus and Mary (http://www.scjm.lk/)

* Sri Lanka Technical Institute & Diyagala Boy's town (http://www.diyagalaboystown.slt.lk/)

* Sudaya Trust (https://dayamina.weebly.com/about.html)

* The Brave Hearts Fund of the Seva Vanitha Army Unit (https://alt.army.lk/sevavanitha/)

## No Online Presence

The remaining 41 Websites had no online presence (as far as I could find).

You can find a spreadsheet with more details here.

## Concluding Thoughts and Caveats

Like I said, this is a very rough audit. A lot more work is needed to get a complete picture of Charities in Sri Lanka.

Also, if you know of any charities not on the list or incorrectly represented, please comment.

Having said that, I'm curious about the following:

* Why don't more charities have online donation options? Especially those that already have offline donation options? It should be fairly low-cost to connect their bank accounts to donations products.

* Why do many charities have no donation options? Is it because their donor base is locked in? Or is it because donors are not online?

* Finally, why do many charities not have an online presence? Is it a lack of resources for building websites etc? Perhaps a lack of expertise?

![Image](https://cdn-images-1.medium.com/max/800/1*V9EWu9UuHCNW4abwunpJ7A.png)

#### Article 307 · March 8, 2021

# All News is Advertising

### And what to do about it

## News & Money

News is information: information that has been grown, harvested, processed and distributed; rather like food, say carrots. The carrots are grown (say) on a farm in Nuwara Eliya; they are harvested, washed and cleaned; and distributed to various consumers via various intermediaries. Similarly, a politician or their press team conceives some nugget of news. Then, some journalist harvests the sound-bite at the big-wig's press conference. They package the blurb into a "folks, you heard it here first" tweet. And finally, Twitter beams the tweet to millions of consumers in the twitter-sphere.

More complex examples of news, say a well-researched investigative news report, is communicated by a more complicated process. Like a more complex food, like a well-balanced rice and curry plate, there are many food sources, processing happens in many places, and the distribution is more elaborate, involving many intermediaries.

But the fundamentals are the same. It is information; information that has been grown, harvested, processed and distributed.

![Image](https://cdn-images-1.medium.com/max/800/1*sRiehmdyaWn7CzqBKbgI9Q.jpeg)

...

News costs money, like anything harvested, processed and distributed. The politician's press conference costs money. Journalists cost money. And giant platforms like Twitter cost a lot of money. Hence, many individuals and entities know and unknown pay for even the simplest piece of news like "She said, he said" tweet". A well-researched investigative news report involves a far more complicated set of benefactors.

Hence, money and news go hand in glove because whoever pays for the news determines its content. And when many people pay for the news, they choose the content in proportion to how much they paid.

## Subscription & Advertising

There are two ways of paying for news: a "push" model and a "pull" model.

In the "push" model, producers of information pay money to "push" information to consumers; a model also known as advertising. In a "pull" model consumers spend money to "pull" information from producers; also known as subscription.

Push and Pull are theoretical extremes. In practice, most newspapers are a mix of subscription and advertising.

...

On the one hand, Newspapers full of advertisements are more push. In addition to official advertisements, they are also full of unofficial advertisements, like sponsored stories, where a journalist writes something that looks like an article but is an advertisement. But even such media often have some aspect of subscription. For example, you might need to pay to purchase it, even if the revenue from such purchases are a small fraction of advertising income.

On the other hand, newspapers that seem to be 100% subscription (say, because there are no advertisements in sight), have hidden advertising. They might, for example, benefit from various donors, charities and foundations, and the publication might consciously or unconsciously promote the views of these.

Hence, to even a small extent, all news is advertising. Producers of information, with interests, both hidden and transparent, are pushing information towards the consumers.

## Benefits & Mindfulness Aides

On the one hand, for me at least, there is something liberating by accepting the fact that "all news is advertising". Consider the following benefits:

* One is not bothered by biased or ignorant news articles. It merely reflects the opinions and knowledge of the people paying for it. These people have a right to expression (even partial views), and ignorance (i.e. the lack of knowledge) is not a crime.

* One is not bothered by fake news, alt-facts etc. Similar to bias, phoney news simply implies that the sources of news are inclined to pathological lying. A lie is only a problem if you don't know the liar.

...

On the other hand, this level of liberation needs an almost super-human mindfulness level when consuming news. You might know that a tweeter is a congenital idiot, but you might still, at least for a moment, be annoyed at the tweet; before your better sense kicks in and dismisses it for what it is.

Hence, for humans who (like me) are not super-humans, a few "mindfulness aides" might be helpful. The following have helped me:

* Consume news in pull mode. In other words, control what you consume, when and how. I've expanded on this in How I consume information.

* Know the source and who pays them. The most important thing to know about a newspaper is not how qualified or famous their journalists are, but who pays for it. You can get some sense of this from articles and advertisements run in the newspapers. However, to get a more profound sense, you'll need to dig into more concrete financial information; like who the paper's shareholders are, who their parent companies etc. Ideally, I'd like a "this was sponsored by or the author was sponsored by" blurb follow every article, and a disclosure on donors, shareholders and parent companies to contain each edition of a newspaper.

...

(Eh, who pays me? I write as a hobby, and hence, I'm entirely self -funded. For my "real" occupation and sources of income, see my LinkedIn profile.)

#### Article 308 · March 11, 2021

# Programming Subjectivity

A Metaphor

## An Objective Universe

Suppose you observe a flag flying in the distance. And suppose you ask yourself, "What color is that flag?"

The following snippet of code can represent this act of observation:

```
const flag = Object({  name: 'flag',  color: 'red',  weight: 'light',  texture: 'soft',})
```

```
function observe(x, attributeName) {  return x[attributeName];}
```

```
>> print(observe(flag, 'color'))'red'
```

Your observation would tell you that the flag is red. In this universe, we assume that (at least around the time when the flag was observed), the flag and the flag's properties (like color) are both constant and objective.

## A Subjective Universe

But what if the universe behaved differently? What if the act of observing actually created the flag?

```
function observe(x, attributeName) {  x = Object({    name: 'flag',    color: 'red',    weight: 'light',    texture: 'soft',  })  return x[attributeName];}
```

```
>> print(observe(flag, 'color'))'red'
```

In this subjective universe, observing the flag would yield exactly the same observation as in the objective universe. "What color is the flag?", you ask. "The flag is red", replies the universe. But, if you didn't ask, there would have been no flag.

## A Subjective Universe (v2)

But what if we went further? What if the universe created, not a flag, but a flag that was (even more) objectified to your question?

```
function observe(x, attributeName) {  x = Object({    attributeName: 'red',  })  return x[attributeName];}
```

```
>> print(observe(flag, 'color'))'red'
```

In such a universe, the flag would only have properties that you (the observer) cares about. You care about color — the flag has only color. You care about texture — then, the flag has only texture, and so on.

## A Subjective Universe (v3)

Could we go even further? We could.

```
function observe(x, attributeName, attributeValue) {  x = Object({    attributeName: attributeValue,  })  return x[attributeName];}
```

```
>> print(observe(flag, 'color', 'red'))'red'
```

Why might such a hyper-subjective universe be possible? Consider the following:

What exactly is "red"? It has nothing to do with the nature of the flag. True — the flag's material absorbs all types of light except that which represents red. But even this has nothing to do with the "experience of red".

As far as I can tell, this "experience of red" exists nowhere but in the mind of the observer.

![Image](https://cdn-images-1.medium.com/max/800/1*jILh6RAkW6JYpYpybzuOww.jpeg)

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

#### Article 310 · March 14, 2021

# Statistical Significance

### Yet another layperson's guide

Imagine if everyone in the medical profession had no idea what temperature and its consequences meant. Ignorance of such a fundamental concept would result in confussion and carnage. Statistical Significance is like temperature, but significantly more significant and consequential. Not just consequential to the medical profession, but to anyone or any profession doing experiments, making claims on data, and or theorizing.

I have written and talked about Statistical Significance often. And to many, I might be preaching to a choir. But when something is important, there is no harm repeating it. So here goes: This article is yet another attempt at a laypersons guide to Statistical Significance.

## Superpowers

"I have a superpower", suppose I tell you.

"What superpower?" you say doubtfully.

"I can predict the future.", I say.

"The future? Like what the price of bitcoin will be in a week?"

"Well, not quite.", I clarify. "I can predict the future in one special case."

"What special case?"

"Well, if you toss a coin, I can predict its outcome before you toss the coin."

## Evidence

"How can I believe you?" you continue, sceptically.

"Well, ask our mutual friend Amali. She tossed a coin twice last Sunday. And I was able to predict it correctly both times."

"Really?"

"Yes. I said heads and then tails. And that's what happened. Amali's coin landed heads and then tails."

## Statistical Significance

The probability of guessing the outcome of a coin toss randomly, and getting it right, is 50% (assuming the coin was balanced or fair). The probability of getting it right twice is 50% x 50% or 25%. Hence, the probability that "the evidence for me having a superpower being a result of randomness" is 25%.

The "probability that the evidence was a result of randomness" is the intuitive definition of statistical Significance. For a more formal definition (involving more concepts like "Null Hypotheses", "Alternative Hypotheses" and "P-Values"), you can read this excellent Wikipedia article on the topic.

## A step-by-step guide to using Statistical Significance

* When someone makes a claim (especially dubious people like Astrologers and Economists) ask for evidence. When you get the evidence, calculate the Statistical Significance

* If the Statistical Significance is low (say less than 5%), you can accept the claim; the chance of the evidence being a result of randomness is low.

* If the statistical Significance is high (say more than 5 or 10%), take one of the following steps.

* Ask for more evidence. If you get more evidence, repeat the steps.

* If the claimant refuses evidence and says something like, "well, this data is not the only evidence, many other theories supported by more data also support my claim", ask for this additional evidence and repeat the steps.

* If the claimant dithers further, then summarily dismiss the claimant and the claims. Both are frauds.

* Alternatively, make sure that the claimant suffers severe repercussions if their claim turns out to be false. For example, demand that they forfeit their entire consultation fee plus an additional 50% of their claim turns out to be wrong. In other words, make sure they have #SkinInTheGame.

![Image](https://cdn-images-1.medium.com/max/800/1*IgmbwlLTYwpIdvV5wbg3eA.png)

#### Article 311 · March 15, 2021

# Heaven on Earth

### On freedom from Chocolate and Mosquitos

Heaven is an integral part of most religions. For many theists, heaven is the end goal and where one desires to spend eternity. Life is a mere test of a few years that will determine entry.

For atheists, on the other hand, heaven is a curse. At best, it distracts people from life; at worst, it motivates people to do horrendous things on earth so that they might reap rewards in heaven.

I belong to neither camp. I'm intellectual honest and humble enough to say, "I don't know", if there is a heaven or hell, or when and how one will get there. Hence, this article is not about heaven; instead, the idea of heaven inspires this article.

...

Theist, atheist or agnostic, we all probably agree on one thing. We all desire happiness and contentment. Or equivalently, we desire freedom from suffering. For the theist, heaven is the ultimate happiness and contentment and freedom from suffering.

We all also probably agree on another thing: We are willing to behave in such a manner that will enable us this happiness, contentment and freedom from suffering. We might disagree on specifics, but we all agree on the principle that some behaviour is worth it.

Hence, what behaviour on earth would result in happiness, contentment and freedom from suffering on earth? Or in other words, what behaviour would result in "Heaven on Earth"?

...

Let's start with suffering. To me, broadly, suffering comes in two flavours:

* Wanting something and not getting it (e.g. wanting a bar of chocolate and none being present)

* Not wanting something and getting it (e.g. not wanting a mosquito to sever your leg, and the said worthy doing precisely that)

To me, happiness and contentment is the negation of suffering; that is, the "state of mind" when there is no suffering. And the above "definition" also indirectly defines happiness.

So what behaviour would result in "Heaven on Earth"? It is simple in theory; if you don't want anything or not want anything, you are incapable of suffering.

...

But what does it look like in practice? To be honest, I don't have a complete or satisfactory answer. Only inklings and patterns.

But let me share these.

* Generosity and vicarious joy: One way of "not wanting a bar of chocolate" is to give it to someone else, if not wholly, at least partially. The happiness of seeing the other enjoy the chocolate might compensate for the unhappiness of not getting a sugar hit.

* Compassion: When you consume chocolate, your body needs to produce extra insulin to process the sugar in your blood. If you overdo the chocolate, your poor, overstressed body would eventually lose its ability to process sugar (also known as diabetes). Hence, you could convince yourself to avoid excesses through compassion. Alternatively, you can feel compassion for your friend who also desires the chocolate.

* Expanding your "self": The mosquito might be a pain, but she is also a mother-to-be. Without the protein and iron in your blood, she cannot produce eggs. Suppose a human mother-to-be would ask you for some food. In that case, you'd probably be more than willing to provide it because you consider it part of your "self" to help; it's the sort of thing "you" do. Why not expanding this idea to include other things?

..

PS: Everything said here also applies to "hell", which, for clarity, I exclude.

![Image](https://cdn-images-1.medium.com/max/800/1*p-PfwOMvyrBwgRwfnhfrCA.jpeg)

Related Articles

#### Article 312 · March 15, 2021

# The Table of our Ancestors

### Fixing Sri Lanka's Carb Problem

On the one hand, all humans have similar dietary needs. A healthy diet should contain macronutrients (Carbohydrates, Fats, Proteins, and Fiber), micronutrients (Vitamins and Minerals), fluids (water), and in combination, provide enough calorific energy.

On the other hand, within these similarities, there are differences. For example, there are significant regional differences in how humans consume milk.

Lactose intolerance is high in East Asia and low in much of Northern Europe. Evolution probably played a role here. In regions where milk was a crucial part of the diet, humans who could process it quickly had a survival advantage — those who didn't died out. In regions where milk was less critical, digesting it was unnecessary and, hence, an evolutionary burden that evolved out.

![Image](https://cdn-images-1.medium.com/max/800/1*SXXQC2B3uqRnkrnPXywbyg.jpeg)

Hence, to some extent, what we should eat is what we've evolved to eat. In other words, it's probably a good idea to eat what our ancestors ate and avoid what they didn't. In general, that is. There might be a few particular cases where we need to disobey this rule.

If you are a Sri Lankan, the odds are that 500 years ago, your ancestors were farmers. Farmers who burned 5,000 or more (kilo) calories per day. With such a high-energy life-style, they needed to consume a lot of carbs. Nutritionists today recommend that the adult male consume about 2,000 calories per day; 55% of our calories in carbohydrates, about 25% in fats and the remaining 20% in protein.

In contrast, our farmer ancestor probably needed to consume an additional 3,000 calories, mostly in carbs. As a result, their ratio of carbs-fats-proteins was perhaps more like 80%-10%-10%.

Sadly, many Sri Lankans probably still eat like our ancestors. While the idea of "eating at our ancestors' table" might be good in general, it is bad that too many Sri Lankans are eating too many carbs. This imbalance is usually at the cost of protein, of which many Sri Lankan meals are deficient. The abundance of carbs also leads to alarmingly high rates of diabetes and related maladies.

What's the solution? Several things might help:

* Education. Even many Sri Lankans who can afford more protein don't eat enough. More robust education on nutrition will help.

* Cheaper and Greener Protein. For many people, protein means animal protein (i.e. Fish, Meat and Eggs), which is expensive and increasingly environmentally destructive. More affordable and greener alternatives like soya, TVP and tofu should be promoted more.

* State programs. The state already intervenes in several nutrition programs, e.g. meals for school children. These programs could push for higher consumption of cheaper/greener protein.

* Light touch regulation. Additional nutritional information like nutrition labels is increasingly common in Sri Lanka. More information and regulation around encouraging lower sugar and refined carb consumption and higher protein consumption would help.

What else? Please comment with your own ideas and thoughts.

![Image](https://cdn-images-1.medium.com/max/800/1*hmxP7VaapGAGRLWAfXEK-g.jpeg)

#### Article 313 · March 17, 2021

Thanks Fred for those kind and generous words. I'm glad you enjoy my writings.

#### Article 314 · March 17, 2021

# When will Sri Lanka win another World Cup?

### A brief history of the Men's ODI Cricket World Cup, and some predictions

Today (March 17th) is the 25th anniversary of Sri Lanka's first and only win in a (Men's ODI) Cricket World Cup. We celebrated that win for months, perhaps years. From time to time, I still watch the epic final, the hammering India got in the semi-final and the inimitable "Chokra" song.

![Image](https://cdn-images-1.medium.com/max/800/1*u-FaVs1Rmmo-wj6InpjIPg.png)

The days around the 1996 World Cup were incredibly dark. A terrorist attack on the Central Bank killed 91 people and injured over 1,000 just a few weeks before the final. Australia and the West Indies refused to play in Colombo, citing security concerns. These circumstances make 1996 particularly significant and even more memorable.

While hardly a comparison, the present is pretty dark for Sri Lankan Cricket. While in the past we used to cheer winning tournaments, these days we cheer winning matches. Will Sri Lanka win another World Cup? Given the current state, I doubt many people are even considering the question.

But since it's Christmas (or at least a comparably important day for Sri Lankan Cricket), I will attempt it. Since I'm no cricket pundit, I attempt an entirely data-driven (i.e. quantitative, as opposed to qualitative or opinion-driven) answer.

## The Invincibility Score

In my previous article, The Invincibility Score, I proposed "a more meaningful alternative to Cricket Ratings". The idea was to design a rating system that had some real-world meaning. The "invincibility score" of a team was the probability that it beats all the other ODI teams.

## "Probability of Winning the World Cup"

For this article, I adapted the invincibility score's underlying statistics to compute the "probability of winning the world cup" at a given time. [It assumes that the world cup is played in a neutral location (i.e. a sort of average of all the venues), assumes a league-style world cup (like 2019 and 1992). For simplicity, I only look at the 9 test playing teams.]

When we plot the "probability of winning the world cup" for each team by time, we get the following graph:

![Image](https://cdn-images-1.medium.com/max/800/1*Hxpt6OTW52S3uRbdJJl3BQ.png)

## A Brief history of the Men's ODI Cricket World Cup

The West Indies had an almost 100% chance of winning the 1975 and 1979 World Cups. And as expected, they did.

While the said West Indies had similar odds of winning in 1983, India, considered an almost impossible underdog, won. 1983 was the first in a series of world cups that were won, not by the favourites but by underdogs, or at least "not so favourites". West Indies were expected to win again in 1987, but Australia ended up winning. England were favourites in 1992; instead, Pakistan won. Australia were top-seeds in 1996, instead Sri Lanka won. Finally, in 1999, favourites South Africa was choked out, while a down-but-steadily rising Australia won.

Like the West Indies in the '70s and '80s, Australia dominated the 2000s, and were favourites and won the 2003, 2007 and 2015 World Cups.

The exception was 2011 when there was a resurgence of both India and Sri Lanka. The two nations met in the world cup finals, and India (marginally favourites) won.

The lead-up to 2019 was a battle between India and England. The latter was the favourite and ended-up winning the world cup.

[Above, by "favourites", I mean "favourites according to my statistical model". I don't mean favourites according to the then zeitgeist or what historians say.]

## So, When will Sri Lanka win another World Cup?

Let's look at Sri Lanka in more detail.

![Image](https://cdn-images-1.medium.com/max/800/1*BeMSjfmPba4-wquEqtyJJQ.png)

Sri Lanka's odds of winning a world cup were almost zero until about 1993. It began to gradually increase in the lead-up to 1996. Sri Lanka's odds peaked after 1996. If there was a World Cup in late 1997, Sri Lanka would have almost certainty (77%) won.

There was a slight peak (23%) in the lead-up to 2003, when Sri Lanka were Semi-Finalists. Oddly, Sri Lanka's odds in 2007 were relatively low (<5%), despite reaching the finals. The next prominent peak (over 40%) was in 2011 when Sri Lanka was Runner-up to India.

After a peak in early 2014, the odds crashed and have not recovered. Since about 2017, Sri Lanka's probability of winning a world cup has been almost zero.

## Philosophical Conclusions

Statistically, Sri Lanka has no chance in hell of winning a Men's ODI World Cup anytime soon. That's the bad news.

However, I'll conclude with two fragments of philosophical hope:

* World Cups have been won by underdogs in the past — many pundits considered 1996 impossible — the future is fair game; and

* Sri Lanka's growth in the lead up to 1996 and beyond, as impressive. There is no reason why this cannot be repeated.

Until then we can always celebrate 1996!

#### Article 315 · March 24, 2021

Thanks! 🙏

#### Article 316 · March 24, 2021

# The Solutionist Manifesto

### Solving Sri Lanka's Problems with Five Precepts

Corruption is a common topic in Sri Lankan conversation. And many wonder why I'm usually silent when it comes up. Those who've known me a short while assume that I might be a direct or indirect supporter of the maroon team or whoever the corrupter is. Those who've known me longer know that I've been similarly silent when discussing the green(ish) team's corruption. Hence, they assume that I might be apathetic or might have given up.

"Don't you care about these problems?", you might have asked.

I have a simple answer to this question. "No — I don't care about these problems". And, for that matter, problems in general. I care about solutions.

This article is about how I think about solutions. If you also care about solving problems in general, and Sri Lanka's in particular, you might be interested.

## 1) Identifying with Solutions

Most people who say "I care about problem X" have done nothing to solve the problem. In other words, they identify with the problem and not the solution.

A "Solutionist" (i.e. someone who abides by this manifesto's precepts) identifies with the solution. "I care about solution Y", they might say.

## 2) Individual Responsibility

If you ask a "Problemist" (i.e. someone who says "I care about problem X", but does nothing to solve it), "who is going to solve problem X?" the answer is always someone else. Often the government, or the municipality, or Dialog, or Ratnapala's cousin's mother-in-law. Anything and anyone, up to and including the kitchen sink, but not "me".

A Solutionist considers it their individual responsibility to solve the problem. They might get help from others or play a supporting role to a more involved solutionist. But, for them, it is still "my problem". And "nothing is someone else's problem".

## 3) Skin in the Game

There are industries devoted to the well-being of Problemists. Many Problemists are professional Problemists who get paid for saying stuff like "X is a serious problem".

More information about problems is always helpful, but solutions are not a priority for many of these problem-industrialists. Hence, the problemists are part of the problem. Not the solution.

Solutionists, on the other hand, have skin-in-the-game in the quest for a solution. They align their well-being and sense of success with the solution. They never profit from problems.

## 4) Direct Democracy

In theory, in a perfect representative democracy, it is sufficient to alert your representative of whatever problem you have. They will do what it takes to solve it. In practice, there are no perfect representative democracies. The "representative" part of democracy is only one tactic in a solution.

Hence, if you think it is sufficient to petition the powers that be about a problem or threaten not to vote for them, or just talk a lot about how they should solve the problem, you're not a Solutionist; because you've already broken the "Individual Responsibility" precept.

While a Solutionist takes representative democracy seriously, they also take other measures to solve the problem. One of the most potent tactics is in a "flawed" democracy like Sri Lanka is to do whatever is needed independent of official representatives. Planting a single tree in your backyard is better than complaining to your neighbour about all the trees at Sinharaja.

## 5) Baby Steps

All big plans fail. Big plans that appear to have succeeded are post-rationalizations. Someone with the benefit of hindsight, aggregates a string of baby plans into a supposed big plan, after the fact.

Problemists usually talk about big plans ("a complete overhaul of this" or "master-plan for the mass deployment of that") because they have no skin-in-the-game and don't care about a solution.

Solutionists, with skin-in-the-game, cannot afford failure. And hence, cannot afford big plans. The best Solutionists are experts at baby-steps, trying out creative ideas, and iterating like mad.

## Concluding Confessions and Calls

There are many times when I'm not silent when discussing corruption; usually when I'm around fellow Solutionists. At these times, I'm generally in my element — because nothing excites me more than an exciting solution to a tricky problem.

Also, I must confess a weakness. I have a terrible habit of prematurely jumping to conclusions about people. I might have "classified" you as a "Problemist" when you're a card-carrying "Solutionist"; perhaps even one more willing and able than yours truly.

If that is the case, please let me know. Tell me how you identify with solutions, how you've taken responsibility for seeing them through, how you have your skin in the solution, etc. And how I might be able to help. It might be the beginning of something big (in baby steps of course)...

Solutionists of Sri Lanka unite!

![Image](https://cdn-images-1.medium.com/max/800/1*aszdhzi6J0iE3x_yBwkFMA.jpeg)

#### Article 317 · March 25, 2021

Might be easiest to discuss a concrete example. Could you propose one as specific as possible?

#### Article 318 · April 1, 2021

# Describing Software Engineers (SWEs)

### On Titles, Levels, Salaries and Effective Experience

What's the difference between a "Software Engineer" and a "Senior Software Engineer"? Is a Senior SWE in one company better than a plain SWE in another company?

The problem with "titles" like "SWE" and "Senior SWE" is that there is no standard convention around what they mean. Technically, anyone can use any title.

This article summarizes how I think about "titles" in general and how I "translate" titles into other particular factors.

## Titles and Levels

Most established tech companies have a progression of titles. Titles are also usually associated with some numerical "level". For example, Google has (had?) the following titles and levels.

![Image](https://cdn-images-1.medium.com/max/800/1*RqVju16eLI1p7SRmvmKgQA.png)

Note, Google does not hire E1 and E2s. Google hires Entry-level SWEs (e.g. "straight out of university") are usually as E3s. Facebook (my former workplace) used the same levels but did not use publicly visible titles.

## Salaries

There was an unwritten rule at Facebook that anyone at level X + 1 about 1.5x more impact than anyone at level X. Since it was reasonable for the organization to compensate employees in proportion to their impact, salaries also reflected this "exponential". An E5's salary (roughly) was 1.5x the salary of an E4.

I haven't done a proper analysis of SWE salaries in Sri Lanka, but here is a rough mapping of levels and titles to salaries for presentation's sake.

![Image](https://cdn-images-1.medium.com/max/800/1*A_1_eeFIeALwkFR7vpz9nw.png)

The critical takeaway is less the actual numbers and more the multiplier between levels.

Why 1.5x? Why not 1.25x or 2x? The 1.5x is somewhat arbitrary. It seemed reasonable for Facebook but might be different in other circumstances. A market with slower growth would have a smaller multiple and vice versa.

## "Effective Experience"

Many associate titles with experience. Some companies "promote" SWEs purely due to how many years they've spent at the companies. I've even heard some SWEs demand promotion based on their "seniority".

Experience is essential; but not "raw experience" measured in time; instead "effective experience, which is time multiplied by how effectively you spent that time. For example, one year spent in an exciting role learning many new skills every day is far more "effective" than one where you do the same thing every day. "Effective experience" can even be negative; especially when the experience consists of mundane and obsolete technology.

"Effective experience" is also directly proportional to the SWE's impact capability. Hence, ideally, it should be proportional to salary. Hence, this is my rough mapping of Title, Level, Salary and Effective Experience.

![Image](https://cdn-images-1.medium.com/max/800/1*CeCl75YDPzgEga5upQIwPg.png)

Like Salary, Effective Experience also follows the 1.5x exponential rule. Hence, gaining effective experience for higher levels takes more time and becomes increasingly difficult. Often, once a SWE reaches a certain level, the new skills they learn are barely sufficient to compensate for old skills that have become obsolete. The SWE's effective experience remains constant, and they remain at the same level.

How come an "Entry Level" SWE has 4.5 years of experience? Because they already should have acquired a range of skills from University, School and Coding Projects relevant to the SWE role. "Work" is not the only means of "effective experience".

Finally, where do you get 77 years of effective experience? You either live (and work) till you've passed a 100, or you are a genius who can acquire several years of effective experience every raw calendar year. Both are highly unlikely, and, not surprisingly, there are almost no Fellows at Google or E10s at Facebook.

## Concluding Thoughts

So "What's the difference between a "Software Engineer" and a "Senior Software Engineer?" It is difficult to say, merely based on titles. But a combination of Levels, Salary and Effective Experience, will give you a better picture.

#### Article 319 · April 2, 2021

# Forgive them; for they know not what they do

### On Forgiveness, Justice and Pain

To forgive, they say, is divine. It is often difficult for us humans to forgive; certainly compared to other things we excel at, like erring.

I've tried to forgive whenever I can, and a few times have even been successful. However, this article is about failures. More specifically, some reflections on two reasons why I've been unable to forgive.

## Justice

For you to forgive me, I should have wronged you. Without this wronging, forgiveness is meaningless. I might have punched you in the face, or spoken to you rudely, or knocked your bishop over, when your eyes were averted from the chess-board.

In all such "wrongings", great and small, there is a pattern. There are rules that define "right"; rules for decent behaviour, rules for speech, and rules for playing games like chess. And in all cases, doing a "wrong" involves breaking these rules. In other words, "wronging" is relative to some system of justice.

This "sense of wrong" is the first part of the justice system. The second part involves "putting the wrong right"; I might have to pay your medical bills (to compensate for the face-punching); or apologise in front of all our friends (for being rude to you), or forfeit that game of chess (for cheating).

Collectives like countries, organisations, or even two friends playing chess, need rules such that they may operate smoothly. Without justice, systems tend to descend into chaos. And hence often, and not unreasonably, justice is hailed as a virtue.

However, justice has problems. It is relative and arbitrary. It depends on who defines the rules. The people who define the rules (often plutocrats and politicians) tend to legislate as it suits them. For example, I could define some "laws" that make punching you, or being rude to you, or cheating at chess, "just" and "justifiable".

Hence, it is best to be mindful of justice's weaknesses, use it only when necessary, and not be too profoundly identified or "married" to it. It is a tool, like a knife, that, when used carefully and correctly, is useful. But when it is not essential, it is best not to cut others and oneself with it. "Judge not", as they say.

More relevant to this article however, justice has a deeper problem. It often undermines forgiveness.

Often I've tried to forgive people but have not been able to, because justice reminds me loud and clear, "You are in the right! And you have been wronged! You should demand justice!" And at some level, forgiving seems to feel like undermining justice.

## Pain

Pain is the other thing that gets in the way of forgiveness.

I have never been scourged and nailed through my hands and feet. Nor, I assume, have you, dear reader. And I hope neither of us ever will be.

But at times, when I have been "wronged", I have felt significant physical and mental pain. When your mind or body is in pain, forgiveness becomes even more difficult.

How do you forgive someone who has caused (or is causing) you real pain?

The path for me begins with "they know not", or the realisation that people wrong and cause pain through ignorance. Not ignorance of justice, but ignorance of how fellow beings are and feel.

The opposite of this ignorance is compassion: the ability to internalise another's suffering. If I genuinely had such an ability, I would not have punched you in the face.

But even more profoundly, if you could understand and internalise that I too was "suffering", not from a painful face, but from ignorance, you too would have found it easier to forgive me. If the punching were reversed, I too, you, I'm sure.

## Concluding Confessions

Reflecting on the limitations of justice and the distractions of pain have made forgiving a little easier. However, it is still a challenge, and I do not forgive as much as I should. Nor do I expect you do.

But I hope we can forgive ourselves for that.

After all, to err, is human.

![Image](https://cdn-images-1.medium.com/max/800/1*fuH6u51SVY5F_C80Q7I8NA.jpeg)

#### Article 320 · April 14, 2021

Fixed the typo. Thanks!

#### Article 321 · April 21, 2021

Thanks! Kind of you to say so.

#### Article 322 · April 25, 2021

# Liberation from ToDo Lists

### From commandment to reminder

Do ToDo lists intimidate you? They do me.

On the one hand, ToDo lists are incredibly useful. They make sure we get things done, and don't forget.

On the other hand, they can be intimidating. They are a voice in ones head that continuously mutter, "You have to do me, you have to do me, you have to do me"; ad nauseam. They can be a sort of debt, which one is eternally guilty of not paying. They can even feel like some impending doom...

Hence, do the pros of ToDo lists, compensate for putting up with the cons?

#### Article 323 · May 17, 2021

# Bath (බත්) Packet 2.0

### Redesigning a venerable institution

For most Sri Lankans (and an increasing number of non-Sri Lankans), nothing beats a good Bath (බත්, rice) to quench hunger. And ubiquitous Bath (බත්) Packet (or BP for short), available everywhere, from a humble way-side hawker to the poshest five-start hotel, is a fairly convenient and efficient way to imbibe a Bath into your system.

![Image](https://cdn-images-1.medium.com/max/800/1*c013Na6WpTOn4L3Mt0Ws4w.jpeg)

## The Problem

However, the venerable BP in particular, and the way we consume rice in general, has a serious downside. When you open a BP, you will notice the mountain of rice. Perhaps 80% or more of its calorific content is from rice, which itself is mostly carbohydrates. This excess of carbs, along with a spike in the consumption of refined sugars, is causing a diabetes epidemic and a host of other related disorders like heart and kidney disease.

The excess of carbs also means that the BP is deficient in other things, especially protein and vital minerals like Iron. The lack of the latter has also resulted in severe growth stunting, particularly in children, and Anemia, especially in women.

## The Root of the Problem

The excess of carbs is not surprising, given that for much of history, most Sri Lankans were farmers or engaged in similarly energy-intensive professions. Today fewer and fewer Sri Lankans are farmers, and more and more Sri Lankans have desk jobs. However, the farmer might have left the farm for the office, but hasn't given up the farmer's diet.

What if we can redesign the venerable BP to be more healthy? And particularly adapt it to our current lifestyle, which is far less energy-intensive? What if we can also use it to address other problems like protein deficiency?

## The Solution (BP 2.0)

What would be the "characteristics" of a healthy BP? I assumed the following:

* About 800 Cal (given that an adult male needs about 2,000 Cal per day)

* 55% of calories from Carbs, 25% from fat, and 20% from protein.

* 2 portions (or 160g) of vegetables

Also, assuming a fairly standard set of ingredients, I got the following "recipe"*:

* Rice (73 g uncooked, about ⅓ cups or hundus)

* Soya Meat (54 g)

* Dhal (16 g)

* Egg (half an egg)

* Brinjal (40 g)

* Pumpkin (40 g)

* Carrot (40 g)

* Onion (40 g)

* Coconut (29 g)

* Coconut Oil (7 g, or one and a half teaspoons)

* Green Chilli (8 g)

* Lime (4 g, or about a teaspoon)

[* For simplicity, I've excluded spices and salt, which shouldn't impact the price and nutrition much]

The raw ingredients (i.e. not counting labour and energy) would cost about Rs. 85, assuming Narehenpita Retail Prices published in the Central Bank's Daily Price Report published on May 13, 2021. Adding labour and energy, it would probably cost close to Rs. 150.

## Concluding Observations

The most obvious observation is that how drastically different BP 2.0 is from a "normal" BP. For example,

* About half the plate would be vegetables

* About a quarter by sources of (Soya Meat, Eggs, Dhal)

* And only a quarter would be rice

Given this drastic change in ratio, the "curries" (i.e. soya, dhal, and vegetables) would have to have far fewer spices and far less salt; otherwise, the meal would be uneatable.

As you might have noticed, to keep things simple, I didn't address Iron and other deficiencies. I'll address those in a v2.1.

Finally, I haven't cooked this recipe, so please point out if there are significant "impossibilities". I have already been told that the "coconut oil budget" is far too stingy.

#### Article 324 · May 17, 2021

# On COVID Vaccination

### A Notification System

Over a million Sri Lankans have got at least one dose of some CoViD-19 Vaccine. And plans are afoot to vaccinate many more people.

However, the vaccination drive so far, has been marred by complaints and process inefficiencies. Many people, some of them old and infirm, have had to queue in the sun or rain for hours. Many have been turned away after the ordeal, because the centre ran out of shots. Others have missed the opportunity for vaccination because of miscommunication or confusion.

I have a list of PHI and MOH phone numbers, and I have got into the habit of calling officials in the morning, asking them if there are any vaccination drives in my neighbourhood. When they reply "No", I ask them if there are plans for drives in the next few days. The usual reply is, "We are only notified the night before — so call again tomorrow".

What if there was a better system? For example, what if there was a system that sent me an SMS saying something like this:

>>> Hi Nuwan,

>>> Please report to *CAMPBELL PARK, COLOMBO 8*, at *9 am on Tuesday, May 18th, 2021*, to get your *Sinopharm* COVID Vaccine.

>>> Please bring your National ID Card and medical documents if relevant.

>>> -Thanks!

>>> Public Health Department — Colombo Municipal Council

![Image](https://cdn-images-1.medium.com/max/800/1*jo8FBsiEfcaISN-E-n9fQw.png)

## Can such a system be built, and will it work?

To answer these questions, we need answers for a few "sub-questions".

### Can this system reach all Sri Lankans?

Yes — almost all Sri Lankans have a mobile phone.

### Can we filter people by age?

Yes — all mobile phone numbers (AFAIK) are associated with the National ID Card (NIC) Number of the owner. The first several digits of the NIC represent the year and date of birth, which we can use to filter notification-receivers by age.

### Can we filter by location?

Yes — mobile phone companies have data that can accurately pinpoint the location of a phone. Hence, if the vaccine is administered at Campbell Park, Colombo 8, phones within a (say) 2km radius can be notified.

### Can we specify time windows for vaccinations?

Yes. Again, we can use NIC numbers for that. The last digit of your NIC is a checksum, that is a function of the other numbers, and evenly distributed between 0 and 9. Hence, about 10% of any large-enough population will gave an NIC ending in a particular digit.

Hence, vaccination time windows can be structured by NIC number. For example, NICs ending in 1 and 2 get 9 am, 3 and 4 get 10 am, etc.

### Can health authorities easily communicate their plans with the phone companies?

Yes. For each vaccination location, health authorities need to communicate the following information to the phone companies:

* Vaccination location (e.g. Campbell Park, Colombo 8)

* Vaccination audience approximate radius (e.g. 2km)

* Vaccination time windows (e.g. "NICs ending in 1 and 2 get 9 am, 3 and 4 get 10 am, etc.")

* Vaccination Information (e.g. "Vaccine Name", "bring medical documents" etc.)

This information can be communicated the day before (as local vaccination officials seem to be), and whether there is a change in schedule. For example, if Campbell park is facing delays, they can send an updated SMS asking me to come at 10.30am and not 9am.

## Concluding Question

Sri Lanka is not exactly technologically deficient. We have so many technology companies for whom the above system is peanuts to build. Software Engineers reading this will tell you that this system is probably a day or two of work.

But if this is the case, then why doesn't such a system already exist? I don't have a good answer. Perhaps you do.

Also, if you'd like to collaborate on building such a system, please let me know.

#### Article 325 · May 23, 2021

# Plotting Maps of Sri Lanka with GeoPandas and MatPlotLib

### A Simple Tutorial

Disclaimer: This article describes a work-in-progress. Please comment on how we might improve the underlying libraries, especially what additional features you would like.

## Geo-Spatial Data

The only real barrier to plotting maps of Sri Lanka with Python libraries GeoPandas and MatPlotLib is the difficulty of accessing geographical data for Sri Lanka. I've attempted to solve this problem by scraping geographical data from various sources, sharing it on GitHub, and providing a simple python library geo-nuuuwan for conveniently accessing this data.

Begin by installing geo-nuuuwan

```
pip install geo-nuuuwan
```

## Example 1: Basic Maps

Module geodata in geo (geo-nuuuwan) implements method get_region_geodata, which returns geographical data (as a GeoPandas.GeoDataFrame) for some region of Sri Lanka, split by some region.

For example, the following snippet returns geographical data for Sri Lanka split by province.

```
from geo import geodatagpd_df = geodata.get_region_geodata('LK', 'province')
```

The GeoPandas.GeoDataFrame can be plotted using MatPlotLib as follows:

```
import matplotlib.pyplot as pltfrom geo import geodata
```

```
gpd_df = geodata.get_region_geodata('LK', 'province')gpd_df.plot()
```

```
plt.show()
```

The result is:

![Image](https://cdn-images-1.medium.com/max/800/1*_-I6L4h0_f7L-b4e9-JKLQ.png)

## Example 1a

Similarly, we can plot Colombo District ("LK-11") by DSDs (Divisional Secretariat Divisions) with:

```
gpd_df = geodata.get_region_geodata('LK-11', 'dsd')
```

![Image](https://cdn-images-1.medium.com/max/800/1*4YMw52TMcWfn0tJO06wZYA.png)

## Example 2: Plotting some useful data

In addition to geographical coordinates, the GeoPandas.GeoDataFrame includes some additional basic data like parent regions, population and area data.

This additional data can be inspected as follows:

```
import matplotlib.pyplot as pltfrom geo import geodata
```

```
gpd_df = geodata.get_region_geodata('LK', 'district')print(gpd_df)
```

Output:

![Image](https://cdn-images-1.medium.com/max/800/1*l6oEkw1ZCM5av6yL9qrVpw.png)

Using the population and area data, we can color the map by each region's (say district's) population density as follows:

```
gpd_df = geodata.get_region_geodata('LK', 'district')
```

```
gpd_df['density'] = gpd_df['population'] / gpd_df['area']gpd_df.plot(column='density', legend=True, cmap='OrRd')
```

```
plt.show()
```

![Image](https://cdn-images-1.medium.com/max/800/1*c6DALweaAY3zkdzSUS7JRw.png)

## Example 2a

Similarly, population density of Sri Lanka's DSD.

```
gpd_df = geodata.get_region_geodata('LK', 'dsd')
```

```
gpd_df['density'] = gpd_df['population'] / gpd_df['area']gpd_df.plot(column='density', legend=True, cmap='OrRd')
```

```
plt.show()
```

![Image](https://cdn-images-1.medium.com/max/800/1*ZIMDazKI7P7E1KRxSPnHOg.png)

## Example 2b: Prettifying the Plot

We can add a title, legend, better color scheme to our plot, and resize it as follows:

```
gpd_df = geodata.get_region_geodata('LK', 'dsd')
```

```
gpd_df['density'] = gpd_df['population'] / gpd_df['area']
```

```
gpd_df.plot(    column='density',
```

```
scheme='UserDefined',    classification_kwds={        'bins': [100, 200, 400, 800],    },    legend=True,    legend_kwds={        'labels': [            '< 100',            '100 - 200',            '200 - 400',            '400 - 800',            '800 <',        ],    },    cmap='OrRd',    figsize=(7, 9),)plt.title('Population Density of Sri Lanka by DSD')
```

```
plt.show()
```

[Note, these are all GeoPandas and MatPlotLib features. Not features from geo-nuuuwan.]

![Image](https://cdn-images-1.medium.com/max/800/1*sU8pcimzbq6PDqTdQb3aIA.png)

## Example 2c

Similarly, "Population Density of Sri Lanka by GND":

```
gpd_df = geodata.get_region_geodata('LK', 'gnd')...plt.title('Population Density of Sri Lanka by GND')
```

![Image](https://cdn-images-1.medium.com/max/800/1*coK7FOTZwS_f6XEwUzHVzg.png)

## Example 2d

And "Population Density of the Central Province by DSD":

```
gpd_df = geodata.get_region_geodata('LK-2', 'dsd')...plt.title('Population Density of the Central Province by DSD')
```

![Image](https://cdn-images-1.medium.com/max/800/1*L6_JvyGAXtJI2q2eAOEfVg.png)

## Coming Soon

The goal of this article was to introduce geo-nuuuwan, and plotting basic maps of Sri Lanka and its regions. In future articles, we'll look at:

* Plotting more elaborate data (e.g. census, election)

* Plotting different types of maps and cartograms

* Anything else? Please comment with your wishlist.

#### Article 326 · June 11, 2021

# Analyzing COVID19 in Sri Lanka with Python

### In under 10 minutes

In this tutorial, we will build some graphs that will give a data-driven description of Sri Lanka's COVID19 situation. End-to-end, it should take you less than 10 minutes.

The data is from two sources:

* The COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University, which we can access at https://github.com/CSSEGISandData/COVID-19 and in aggregate at https://pomber.github.io/covid19/timeseries.json.

* The Health Promotion Bureau of Sri Lanka, which we can access at https://www.hpb.health.gov.lk/api/get-current-statistical.

## Part 1: Getting the data

You can either pull the above data yourself. Or we can use my python library, covid19-nuuuwan, which enables convenient data access. To install run,

```
pip install covid19-nuuuwan
```

[You can find the complete source code on GitHub. Feel free to fork this code, or report issues.]

To access the complete Johns Hopkins University data set (which contains up-to-date time series of confirmed cases recoveries and deaths for 189 countries from Afghanistan to Zimbabwe),

```
>>> from covid19 import covid_data>>> jhu_data = covid_data.load_jhu_data()>>> len(jhu_data.values())189
```

```
>>> country_ids = list(jhu_data.keys())>>> country_ids[0], country_ids[-1]
```

```
('AF', 'ZW')
```

Each country entry looks like,

```
>>> jhu_data['LK']
```

```
{ 'country_name': 'Sri Lanka',  'country_alpha_2': 'LK',  'country_alpha_3': 'LKA',  'population': 21803000,  'timeseries': [  {   'date': '2020-01-22 00:00:00',    'unixtime': 1579631400.0,    'cum_confirmed': 0,    'cum_deaths': 0,    'cum_recovered': 0,    'active': 0,    'new_confirmed': 0,    'new_deaths': 0,    'new_recovered': 0,   'cum_vaccinations': 0,   'cum_people_vaccinated': 0,   'cum_people_fully_vaccinated': 0,},   ...  ...  ...  {   'date': '2021-06-09 00:00:00',    'unixtime': 1623177000.0,    'cum_confirmed': 213396,    'cum_deaths': 1910,    'cum_recovered': 180427,    'active': 31059,    'new_confirmed': 2735,    'new_deaths': 66,    'new_recovered': 2168,   'cum_vaccinations': 2450965,   'cum_people_vaccinated': 2089320,   'cum_people_fully_vaccinated': 361645,  } ]}
```

Similarly, the Health Promotion Bureau contains a time-series of PCR tests, information about hospitals and various cumulative statistics.

```
{ "success":true, "message":"Success", "data":{  "update_date_time":"2021-06-11 11:33:36",  "local_new_cases":2738,  "local_total_cases":216134,  "local_total_number_of_individuals_in_hospitals":31986,  "local_deaths":1910,  "local_new_deaths":67,  "local_recovered":182238,  "local_active_cases":31986,  "global_new_cases":421019,  "global_total_cases":175332051,  "global_deaths":3780265,  "global_new_deaths":14097,  "global_recovered":159186733,  "total_pcr_testing_count":3690770,  "daily_pcr_testing_data":[   {    "date":"2020-02-18",    "count":"1"   },...
```

## Part 2: Analyzing the data

Now that we have the data, you can use your favourite analytics library to dig deeper into it. In this tutorial, we'll build some graphs with MatPlotLib.

[You can find the source code for these examples on GitHub.]

### Example 1: Deaths per 100,000 people

We can access the COVID19 time-series for Sri Lanka with,

```
jhu_data = covid_data.load_jhu_data()country_data = jhu_data['LK']timeseries = country_data['timeseries']
```

This data also includes the population for each country, which can be accessed with,

```
pop = country_data['population']
```

To plot a line plot with MatPlotLib,

```
x = list(map(        lambda d: datetime.datetime.fromtimestamp(d['unixtime']),        timeseries,    ))    y = list(map(        lambda d: 100_000 * d['cum_deaths'] / pop,        timeseries,    ))    plt.plot(x, y, color=country_meta_data['color'])
```

After some cosmetic improvements (see example code for details),

![Image](https://cdn-images-1.medium.com/max/800/1*on0jLK9C0Yq51af6cISmTw.png)

### Example 1a: Active Cases per 100,000 people

Similarly, we can plot Active Cases:

![Image](https://cdn-images-1.medium.com/max/800/1*mAt-hxFMAVRcssgh99hYyw.png)

### Example 1b: Active Cases per 100,000 people — minus the Maldives

(Since Maldives is an outlier)

![Image](https://cdn-images-1.medium.com/max/800/1*yUeSENvkMMPliuFB-sNhcw.png)

### Example 2: Daily COVID19 Active Cases, Total Recovered Cases and Total Deaths in Sri Lanka

With the same JHU dataset, let's focus on Sri Lanka. We can plot a stack plot of Active Cases, Total Recovered Cases and Total Deaths as follows:

```
country_data = covid_data.load_jhu_data()['LK']timeseries = country_data['timeseries']
```

```
x = list(map(    lambda d: datetime.datetime.fromtimestamp(d['unixtime']),    timeseries,))y1 = list(map(    lambda d: d['active'],    timeseries,))y2 = list(map(    lambda d: d['cum_recovered'],    timeseries,))y3 = list(map(    lambda d: d['cum_deaths'],    timeseries,))
```

```
plt.stackplot(x, y1, y2, y3, colors=['blue', 'green', 'red'])
```

We get,

![Image](https://cdn-images-1.medium.com/max/800/1*NjEkorjavn_mwVQsKYAwiA.png)

### Example 2a: Total COVID19 Deaths in Sri Lanka

If we remove y1 and y2 from above (because the red stack can, thankfully for now, hardly be seen),

![Image](https://cdn-images-1.medium.com/max/800/1*xktxUsp0Awh-Ugrrkbt14A.png)

### Example 2b: Daily COVID19 Active Cases, Total Recovered Cases and Total Deaths in China

We can plot the above charts for any country we like by simply modifying,

```
country_data = covid_data.load_jhu_data()['CN']
```

![Image](https://cdn-images-1.medium.com/max/800/1*d4JgdbKpdDc5mOr8AOHQBg.png)

### Example 2b: Daily COVID19 Active Cases, Total Recovered Cases and Total Deaths in Israel

```
country_data = covid_data.load_jhu_data()['IL']
```

![Image](https://cdn-images-1.medium.com/max/800/1*8tc7Rx1kKi_kLPvfdiKk5g.png)

Note, the effect of vaccination.

### Example 3: Daily New COVID19 Cases and PCR Tests in Sri Lanka

In addition to the JHU data for Sri Lanka, the HBP dataset also proviceds PCR Tests. The combined time-series for Sri Lanka can be accessed as follows:

```
from covid19 import lk_datatimeseries = lk_data.get_timeseries()
```

Important: lk_data, not covid_data

Plotting with MatPlotLib gives us,

![Image](https://cdn-images-1.medium.com/max/800/1*yoZZSsGvd9A0oY31ThDhXg.png)

### Example 4: Daily New COVID19 Cases per PCR Tests in Sri Lanka

Finally, let's plot the ratio of the two plots above. In addition to the raw Cases per Test, we also plot the 14 day moving average, for a smoother analysis.

![Image](https://cdn-images-1.medium.com/max/800/1*uDQLO8dlJEZwa16HlEbyVw.png)

### Example 5: % People vaccinated in South Asia

```
x = list(map(        lambda d: datetime.datetime.fromtimestamp(d['unixtime']),        timeseries,    ))    y = list(map(        lambda d: d['cum_people_vaccinated'] / population,        timeseries,    ))    plt.plot(x, y, color=country_meta_data['color'])
```

![Image](https://cdn-images-1.medium.com/max/800/1*2IGwTJ64EIt5ds1Vn54_rg.png)

### Example 5a: % People vaccinated in South Asia — without the Maldives and Bhutan

![Image](https://cdn-images-1.medium.com/max/800/1*kD7R9361u3VF2dzUZPs3RQ.png)

### Example 6: Total People Vaccinated in Sri Lanka

```
x = list(map(    lambda d: datetime.datetime.fromtimestamp(d['unixtime']),    timeseries,))y1 = list(map(    lambda d: d['cum_people_fully_vaccinated'],    timeseries,))y2 = list(map(    lambda d: d['cum_people_vaccinated'] - d['cum_people_fully_vaccinated'],    timeseries,))
```

```
plt.stackplot(x, y1, y2, colors=['green', 'lightgreen'])
```

![Image](https://cdn-images-1.medium.com/max/800/1*YTq5xGGA9lRVnua8kDPiIQ.png)

...

If you enjoyed this article, you might also like,

#### Article 327 · June 12, 2021

# The Many Levels of Digital Data Processability

### From pixels to consistent structured information

Humans use computers to solve real-word problems. For example, I (a human) might use my laptop (a computer), to build a model that predicts the number of COVID19 cases in Sri Lanka in the next few weeks (a problem to solve).

In such situations, humans need to supply computers with data that might help find solutions. For example, statistics about COVID19 cases during the past few months (data) might result in a better prediction model (the solution).

By "Processability", I mean how easily a computer can process the data. The better the processability, the more efficient the processing, and the more efficiently the computer can arrive at a solution to the real-world problem.

In this article, I present a 6 levels of Digital Data Processability — from the least processable to the most processable.

## Level 1 — "Pixels"

Consider the latest COVID Press Release from the Department of Government Information (DGI).

![Image](https://cdn-images-1.medium.com/max/800/1*xr00gK7Z1GUCo3rFDTxmDQ.jpeg)

On the one hand, it contains some interesting (be they sombre) statistics about the COVID19 situation in Sri Lanka. It is reasonably well written, and easy for a human to process. On the other hand, it is shared as two JPEG files, one per page, on the DGI's website; very difficult for a computer to directly process.

Digital data in the form of images, where a computer is forced to process pixels, is the least processible form of accessible digital data. If a computer is to process this data, we need to resort to Object Recognition or Optical Character Recognition (OCR). Often these techniques are too expensive or tediious or both, and a human might need to manually convert the digital image into a more processable form.

Hence, Level 1.

## Level 0 — No Data

Before we continue, I must stress, bad data is better than no data. Hence, for completeness, let's call "no data" Level 0.

## Level 2 — Characters

What about PDFs? Is a PDF bextter than an image (like a JPEG)?

Only marginally. When text is presented in a PDF, the PDF file format defines locations to show each text character. For example, if "hello" is presented, the PDF will store the page coordinates of "h", "e", "l" etc. It doesn't explicitly say that "hello" is a word.

Hence, when a computer "sees" a PDF, it only sees characters. Isolated characters are not much of an improvement over isolated pixels. Not unsurprisingly, most data analysts consider PDFs a curse. But since they are marginal better than raw images, let's promote them to Level 2.

## Level 3 — Natural Language

Fortunately, there are ways of converting "lower-level" data into "higher-level" data. For example, I used the python package tesseract to perform OCR (Optical Character Recognition) on the JPEG press release . These days there are highly elaborate and effective OCR systems based on complete Machine Learning.

The OCR results looked like this:

```
Department of Government Information
```

```
12.06.2021Release No: 566/2021Time : 3:00Chief Editor / News EditorDirector (News) / News Manager
```

```
07 COVID deaths reported from 08 May to 31st May:55 COVID deaths reported from 01* June to 10 June:
```

```
No COVID deaths reported yesterday (11):
```

```
Death toll due to COVID 19 from 08 to 31 May 2021 as confirmed yesterday (11) by the DirectorGeneral of Health Services — 07,
```

```
Death toll due to COVID 19 from 01* June to 10 June as confirmed yesterday (11) by the DirectorGeneral of Health Services — 55
```

```
No COVID death was reported so far yesterday, June 11.
```

```
May 08 - 01 death
```

```
May 15 - 01 death
```

```
May 23 - 02 deathsMay 26 - 01 death...
```

[Complete output: https://github.com/nuuuwan/nopdf_data/blob/master/nopdf.dgigovlk.ref566.page001.txt]

Now, unlike the pixels of the JPEG, or the characters of the PDF, the computer has complete words, sentences and paragraphs. Level 3.

## Level 4 — Structured Information

While it is clear to a human what the Natural Language "Total number of COVID 19 deaths as confirmed so far yesterday (June 11th) — 2073" means, we need to help a computer make sense of this data.

To do this, we need to "parse" the data and extracts the nuggets of information that it contains. The "parsing" technique could be as simple as a set of rules, or a complex Machine Learning driven Natural Language Understanding model.

I built a simple rulel based parser that processes press-release text and generates structured information like this:

```
{  "ref_no": "566",  "unixtime": 1623447000,  "datetime": "2021-06-12 03:00",  "deaths_by_day": [    {      "unixtime": 1620412200,      "date": "2021-05-08",      "deaths": 1    },    {      "unixtime": 1621017000,      "date": "2021-05-15",      "deaths": 1    },    ...    {      "unixtime": 1623263400,      "date": "2021-06-10",      "deaths": 5    }  ],  "deaths_by_gender": [    {      "gender": "Female",      "deaths": 27    },    {      "gender": "Male",      "deaths": 35    }  ],  "deaths_by_age": [    {      "age_range": [        0,        20      ],      "deaths": 0    },    {      "age_range": [        20,        29      ],      "deaths": 0    },   ..    {      "age_range": [        99,        130      ],      "deaths": 0    }  ],  "deaths_py_place": [    {      "place": "In Residence ",      "deaths": 13    },    {      "place": "On admission to hospital ",      "deaths": 5    },    {      "place": "While being treated in hospital ",      "deaths": 44    }  ],  "areas_of_residence": [    "Alubomulla",    "Ambakote",    ...    "Waskaduwa"  ],  "causes_of_death_lines": [    "Acute kidney injury",    "Acute respiratory failure",   ...    "Stroke"  ]}
```

[Complete output: https://raw.githubusercontent.com/nuuuwan/nopdf_data/master/nopdf.dgigovlk.ref566.json. You can access the parser on GitHub. Feel free to fork it, or share feedback.]

Level 4.

## Level 5 — Consistent Structured Information

Level 4 is good enough for most data analytics tasks. But perfectionists could go one level further.

Consider the following section of another DGI COVID press release,

![Image](https://cdn-images-1.medium.com/max/800/1*RH1HKcGMFi8CA78OIj3ccw.png)

...and its corresponding Level 4 structured information:

```
...{      "district_name": "Monaragala",      "police_areas": [        {          "police_area_name": "Sewanagala",          "areas": [            {              "area": "Bahirawa"            },            {              "area": "Habarattawela"...
```

Do you see anything wrong?

The official spelling of Monaragala is actually, Moneragala. Consistent, structured information is structured data where such inconsistencies are removed.

On top of having standard spelling, consistent, structured information would also contain data like IDs in addition to names, which are more difficult to misspell. For example, the Moneragala District has ISO code "LK-82", and our Level 5 data would look like this:

```
...  {      "district_id": "LK-82",      "district_name": "Moneragala",      "police_areas": [        {          "police_area_name": "Sewanagala",          "areas": [            {              "gnd_id": "LK-8233045",              "gnd_name": "Bahirawa"            },            {              "gnd_id": "LK-8233070",              "gnd_name": "Habarattawela"            },            {...
```

[Complete output: https://github.com/nuuuwan/nopdf_data/blob/master/nopdf.dgigovlk.ref561.json]

You might argue that the Level 5 version of the press release is more difficult to process, at least for a human. While this might be true, it is trivial to render this into a more attractive format; even one much better than the original press release.

## Concluding Thoughts

Sadly, the DGI's COVID19 press release is representative of a lot of digital data online — both in Sri Lanka and abroad — shared by both public and private organizations. The vast majority consists of Level 1 (images) and Level 2 (PDF) data.

Even sadder, a lot of information which should be shared and accessible, is not (Level 0). For example, the vast proportion of Sri Lanka's public data (i.e. data that Sri Lankans have the right to access and use) is not accessible.

While many techniques transforming low-level data to high-level data (including those I describe), are effective and valuable, they are a waste in situations where high-level data can be shared in the first place. I hope owners of data realize this and are smarter in how they share data. I, for one, will be happy to help them achieve this goal.

![Image](https://cdn-images-1.medium.com/max/800/1*DhggRGMXoYRPsuMdqFwPSw.png)

#### Article 328 · June 18, 2021

# Lies, Damn Lies, and Statistics

### And how to rescue science

## Lies

We all know what lies are. For example, if I toss a coin, and it falls heads, but I tell you,

>>> "the coin landed tails",

then that is a lie.

## Statistics

Many of us also know what statistics are. If I told you,

>>> "There is a 50% chance of the coin landing heads",

then that is a statistic.

## Damn Lies

I couldn't find a credible definition of "Damn Lies", so I thought of inventing one myself.

We usually use the word damn "to emphasize or express anger or frustration with someone or something" [2]. More severely, in Christianity, it means "be condemned by God to suffer eternal punishment in hell". I thought of borrowing from both these usages and defining a Damn Lie as,

>>> "A lie that is so egregious that it should instantly generate anger or frustration in the audience and summarily condemn the liar to suffer eternal punishment in hell."

## Characteristics of Damn Lies

So, what would be an example of a "lie so egregious"?

To me, the worst sort of lie is a lie that we believe to be true. The more people who believe the lie to be true, the more dangerous it is.

For example, consider my previous statement,

>>> "There is a 50% chance of the coin landing heads."

On the one hand, if you read this is an elementary mathematics textbook that says, "assuming the coin is fair", then this statistic is true.

On the other hand, what if this statement refers to a real-world coin toss? Would it be true?

Consider why the previous textbook example is true. It is true by tautology; because a "fair coin" is one, by definition, that lands 50% heads and 50% tails. However, in real life, there are no fair coins.

You counter,

>>> "But what if we design a symmetrical coin? Then wouldn't it be fair?"

The only way we can say an "absolutely symmetrical" coin is "fair" is by conducting a scientific experiment. We toss the symmetrical coin many (say 1,000) times, and if the number of heads is close to 50, we conclude the coin is fair.

But what if we get 511 heads and 489 tails? Is the coin fair or not? This is where statistics comes to the rescue.

## Damn Lies and Statistics

Now, suppose the coin was fair. If one were to toss this fair coin 1000 times and repeat this experiment (of 1000 tosses) many times, in all but 5% of the experiments, the number of heads would be between 469 and 531.

Since 511 is in this range, a statistician might conclude that "There is no evidence that the coin is not fair".

The (somewhat arbitrary) 5% is the probability that we conclude the coin is "not fair" when it is fair, and we could want this probability to be small. "5%" is often a statistician's preferred value for "small".

So if the coin were fair, our test would have a "small" probability of getting it wrong (i.e. concluding that it is not fair).

## Deduction and Induction

>>> "All dogs have four legs. Snowy is a dog. Therefore, snowy has four legs."

is an example of deductive reasoning. We have some premises ("All dogs have four legs" and "Snowy is a dog") and a conclusion ("Snowy has four legs") that logically follows from the premises. Hence, if the premises are true, the conclusion must also be true.

Inductive reasoning is the reverse. We assume that if the conclusion is true, the premises must also be true. For example,

>>> "All dogs have four legs. Garfield has four legs. Therefore, Garfield is a dog".

Note, inductive reasoning is flawed; for example, Garfield could be a cat.

"If the coin were fair, then all but 5% of experiments would have between 469 and 531 heads" is a deductive argument. "If the experiment result is between 469 and 531 heads, then the coin is fair" is an inductive argument.

Our statistical conclusion above is based on such an inductive argument and is hence flawed. For example, a non-fair coin could yield the same results, just as a cat has four legs.

## What Science Really Says

Our examples about tossing coins and dogs that might be cats are trivial. Sadly, more serious scenarios fall into the same bucket.

Consider, for example, a Vaccine. The WHO says that

>>> "If the vaccine works, then it will provide more than 50% of takers with full immunity"

A sound, deductive argument. However, to test the vaccine, we vaccinate a large number of test subjects. If more than 50% have full immunity, we approve the vaccine. However, this is based on an inductive argument:

>>> "If more than 50% of takers have full immunity, the vaccine works".

All conclusions resulting from the scientific method are similar. They are not sound conclusions based on deductive reasoning, which we can "know" to be true. They are flawed conclusions based on inductive reasoning, which we can only "believe" to be possibly true.

## How Science became a Damn Lie

I'm no anti-vaxer. I've taken dozens of vaccines in my life and am impatiently waiting for my COVID19 vaccination. So don't I "believe" in science?

I don't believe in science because I don't "believe" in anything. "Belief" is code for "I don't know, but I pretend to know"; a dangerous excuse of a word. I do know a few things, and with the many things I don't know, I'm happy to say "I don't know" instead of saying "I believe".

Then, don't I "know" any scientific theory to be valid?

Science doesn't say,

>>> "The Vaccine works".

Science only says,

>>> "If the vaccine works, then we would expect these results"

and

>>> "We got those results".

If we conclude,

>>> "Therefore, the vaccine probably works"

...is belief based on induction, not knowledge.

Conversely, if, as in the case of many vaccines, the full immunity rate was less than 50%, then we can deduce (not induce) that "The vaccine does NOT work". Hence, the only truths in science are invalid theories. All claims about "valid theories" are beliefs, not truths.

Hence, again no. I don't "know" any scientific theory to be valid. I do "know" some to be invalid — but none to be valid.

Sadly, many people, including eminent scientists got say that many scientific theories are true. Richard Dawkins famously talks about the "fact of evolution". Science doesn't say that the Theory of Evolution is true; it merely explains the evidence — for now. As Einstein replaced Newton, a new, different theory might explain the evidence better. Hence, Richard Dawkings cannot possibly "know" that that the Theory of Evolution is true. At best, be "believes" it to be true.

This is why, sadly, much of science has acquired "Damn Lie" status, and this is what is really killing science.

## How to Rescue Science

Some readers might conclude that I'm an anti-vaxer-intelligent-design conspiracy theorist. But hopefully, the more discerning will see my real point.

Obviously, Anti-Vaxing and intelligent Design are damn lies; since they are lies that many humans believe to be true. Sadly, many advocates of vaccines and evolution have countered one set of damn lies with another set of damn lies. When a fundamentalist theist says,

>>> "God created the world in 6 days, and that is a fact",

Dawkins says,

>>> "No, the world is a result of evolution, and that is a fact".

To counter religion, Dawkins turned science into religion; and, thus, nailed it to a cross.

My real point is that just as you can't fight fire with fire or anger with anger, you can't fight lies with lies. You have to fight it with something else.

If one is confronted with a lie, the easiest response is the truth. But if we don't "know" the truth, we shouldn't pretend. We risk degrading something that might be true into a damn lie (just as Dawkins has degraded evolution).

If we don't know the truth, the best thing to do is to say, "We just don't know" — as all true scientists have been saying throughout the ages.

### ...

![Image](https://cdn-images-1.medium.com/max/800/1*Oak1DblnxyW7PUS7R75cDA.png)

### References and Notes

[1] https://en.wikipedia.org/wiki/Lies,_damned_lies,_and_statistics

>>> Mark Twain popularized the saying in Chapters from My Autobiography, published in the North American Review in 1907. "Figures often beguile me," he wrote, "particularly when I have the arranging of them myself; in which case the remark attributed to Disraeli would often apply with justice and force: ‘There are three kinds of lies: lies, damned lies, and statistics.'"

[2] "Damn" — https://languages.oup.com/google-dictionary-en/

* Used to emphasize or express anger or frustration with someone or something

* (In Christian belief) be condemned by God to suffer eternal punishment in hell. E.g. "be forever damned with Lucifer."

[3] https://stattrek.com/online-calculator/binomial.aspx

[4] https://en.wikipedia.org/wiki/Deductive_reasoning

[5] https://en.wikipedia.org/wiki/Inductive_reasoning

#### Article 329 · June 26, 2021

# Making the World Better with Data (in 4 Steps)

### A Solutionist's Playbook

"Data" has, for some time now, been quite a buzzword. Governments talk about how they want to be "Data-Centric". Corporates talk about being "Data-Driven". In both public and private organizations, "Chief Data Officer" or equivalent designations are, at the very least, loudly discussed.

Sadly, while "Data" has featured in much talk, for most people, it has underdelivered. We have all this data, but the problems data promised to solve haven't gone away; and in many cases, the problems have multiplied.

Hence, it's not unreasonable to throw one's arms in the air, be honest, declare that data doesn't work, and walk away. I, however, disagree. Not because I'm a "data optimist" who believes we need to continue to "believe" in data, no matter what. But instead, because I see why data has underperformed and see a realistic path to make data deliver.

## Step 1: Data-Driven Definition

All pieces of "data" are descriptions of the real world. Hence, one can use them to describe and define problems.

For example, we can define an individual being "underweight" as one whose Body-Mass-Index (BMI) is below some threshold, say 18.5.

While words like "underweight" are vague and subjective, data helps give them an objective meaning. This objectivity helps communication and agreement. While your "underweight" might not be my "underweight", your 18.5 BMI is a lot closer to my 18.5 BMI. If I tell you, "don't drive too fast", you might not know what that means? Is 60 KMPH too fast? 100 KMPH? However, if I tell you, "Don't exceed 80KMPH", you know exactly what I mean.

Hence, the first step to solve a problem with data is to define it in terms of data.

## Step 2: Data-Driven Measurement

A data-driven definition of a problem makes the problem objectively recognizable. The next step is to recognize concrete instances of the problem.

For example, we could survey Sri Lanka to understand where people with BMIs below 18.5 live. Following such a survey, we might conclude that 11% of Sri Lankan adults and 37% of children are underweight.

Sadly, many self-described data-driven organizations stop with Step 2. Definition and measurement are relatively easy and highly lucrative. Many "research" organizations specialize in this, conveniently stopping short of solving the problem; charlatans selling expensive speedometers for cars without engines.

## Step 3: Data-Driven Ownership

Step 3 is not exactly about starting the engine but pledging to start the engine and go some distance. Once a problem has been measured and defined, anyone wishing to solve it must take ownership of at least part of the problem.

For example, if you want to "solve part of the underweight problem", you might pledge, say, "reduce underweight-ness in children from 37% to 30% in the next five years" or pledge the same goal in some specific part of Sri Lanka (say the Uva Province).

Now, you might have heard plenty of people (often politicians) going around saying things like this. However, the "pledge" is only the first part of Data-Driven Ownership. The second and more important part is "Skin in the game". Not only should one pledge to solve part of the problem, but must also pledge a significant amount of your own resources and reputation to solving it.

The "your own" part is very important. A research organization or a politician who pledges the countries (i.e. not their own) resources has no "Skin in the game".

## Step 4: Data-Driven Iteration

Once one has taken ownership of a problem or part of it, the next step is to solve it.

All big problems have small solutions. Obviously, not one small solution, but a large collection of small solutions that meld together to solve the bigger problem. For example, solving Sri Lankas underweightness problem involves solving the problem for each underweight person and, perhaps, for each meal of each underweight person.

Small problems have at least two benefits. Firstly, the cost of failing is disproportionately smaller for small problems. Secondly, it is easier to apply data to solve small problems; whatever the data says is more "Statistically Significant".

If anyone tells you that big problems need big solutions, they are either politicians or classical economists. Neither has any skin-in-the-game and hence won't care about failing. Nor does either understand Statistical Significance.

Invariably, the more successful problem solver is not the smarter problem solver but the faster problem solver. The faster one can iterate through a large number of small candidate solutions, the more likely you are to solve the big problem.

This final step is the most important of Data-Driven problem-solving. The problem-solving process is not one monolith but an iterative process.

## Concluding Questions

To summarize, if anyone tells you that they are "Data-Driven", you should ask them the following questions:

* What is the problem you are trying to solve, and what is its data-driven definition?

* What is the extent of the problem, measured in data-driven terms?

* What subset of the problem are you solving? And what is your own skin-in-the-game? (described in data-driven terms, obviously)

* What is the data-driven iterative process that you've set up to solve the problem?

![Image](https://cdn-images-1.medium.com/max/800/1*6kZAdXbE6YF72hgaWSvyNA.jpeg)

#### Article 330 · July 13, 2021

# Drawing Dorling Cartograms of Sri Lanka

### A Tutorial with Python, MatPlotLib and GeoPandas

Consider the following map of Sri Lanka, presenting the results of the 2019 Sri Lankan Presidential Election.

![Image](https://cdn-images-1.medium.com/max/800/1*LEYyVKBHh0VWwP965mZZ0A.png)

In my previous article, The "Map", I wrote about two problems with this representation.

* It assumes everyone in a polling division voted for one party. For example, 42.45% of valid votes in the Ratmalana Polling Division were for the NDF. However, on the map it is colored maroon.

* It gives more sparsely populated polling divisions disproportionately more visual space. For example, some of the most densely populated polling divisions in the Colombo District are barely visible.

I described "progressive coloring" as a solution to the first problem, where we color polling divisions where the winning party got a larger proportion of the votes in a stronger color. I proposed Dorling Cartograms as a solution to the second problem.

This article is a tutorial, where will will discuss how we can draw Dorling Cartograms for Sri Lankan Election Results. You can easily extend the ideas to other data.

[You can find the complete source code for this tutorial, including examples at github.com/nuuuwan/infographics.]

## What is a Dorling Cartogram?

A "Cartogram" is a special type of diagram, that modifies a geographical map to better represent statistical informaiton (like the distribution of populations of the results of elections).

A "Dorling Cartogram" represents each area with a geometric shape (e.g. a Circle, a Rectangle or a Hexagon), and the area of the shape is proportional to the statistical data we want to represent (e.g. Population or Valid Votes).

## (Before we begin)

This tutorial assumes you have python 3.7 installed. You also need MatPlotLib and GeoPandas.

```
pip install matplotlibpip install geopandas
```

I've implemented Dorling Cartograms, and a few other convinience functions in PyPI Package infographics-nuuuwan.

```
pip install infographics-nuuuwan
```

Also, you can access data about Sri Lankan elections from PyPI Package elections_lk-nuuuwan.

```
pip install elections_lk-nuuuwan
```

## Example 1: True-Area Map

In all our examples, we will be drawing maps for the 2019 election, and drawing these maps for the entire country.

```
year = 2019region_id = 'LK'
```

Let's first draw a true-area map of Sri Lanka with LKMap, and color each polling division by the winning party.

```
true_map = LKMap(   region_id=region_id,   sub_region_type='pd',   figure_text='a) True-Area Map',​   func_get_color_value=_func_get_color_value,   func_value_to_color=_func_value_to_color,   func_format_color_value=_func_format_color_value,   func_render_label=_func_render_label,​   left_bottom=(0.1, 0.1),   width_height=(0.8, 0.8),)
```

Each of the "func" parameters, pass functions that determine how the map should be colored, and how labels should be rendered.

```
def _func_get_color_value(row):   result = pd_to_result[row.id]   return presidential.get_winning_party_info(result)['party_id']​​def _func_value_to_color(party_id):   return party_color.get_rgb_color(party_id)​​def _func_format_color_value(party_id):   return party_id​​def _func_render_label(row, x, y, spany):   pass
```

We embed the map inside an infographic with Infographic as follows:

```
Infographic(   title='%d Sri Lankan Presidential Election' % year,   subtitle='By Winning Party',   footer_text='\n'.join(      [           'data from https://elections.gov.lk',           'visualization by @nuuuwan',      ]  ),   children=[       true_map,  ],).save('/tmp/infographics.%d.png' % year)
```

The saved image looks like this:

![Image](https://cdn-images-1.medium.com/max/800/1*LEYyVKBHh0VWwP965mZZ0A.png)

## Example 2: Dorling Cartogram

We can represent the election results on a Dorling Cartogram with LKDorlingCartogram, as follows.

```
dorling = LKDorlingCartogram(   region_id=example3.region_id,   sub_region_type='pd',   figure_text='b) Dorling Cartogram',​   func_get_color_value=_func_get_color_value,   func_value_to_color=_func_value_to_color,   func_format_color_value=_func_format_color_value,   func_render_label=_func_render_label,   func_get_area_value=_func_get_area_value,   func_format_area_value=_func_format_area_value,​   left_bottom=(0.55, 0.1),   width_height=(0.4, 0.8),)
```

LKDorlingCartogram is very similar to LKMap, with the exception of the two functions that define the area of the Dorling Cartogram Circles; note, we want to make the area of the circle proportional to the number of valid votes in the polling division.

```
def _func_get_area_value(row):    result = pd_to_result[row.id]    return result['summary']['valid']
```

```
def _func_format_area_value(area_value):    return '{:,.0f}\nvalid votes'.format(area_value)
```

We can display the previous True-Area Map, and the Dorling Cartogram, side-by-side, as follows:

```
true_map.set_position(    left_bottom=(0.05, 0.1),    width_height=(0.4, 0.8),)
```

```
Infographic(    title='%d Sri Lankan Presidential Election' % year,    subtitle='By Winning Party',    footer_text='\n'.join(        [            'data from https://elections.gov.lk',            'visualizaiton by @nuuuwan',        ]    ),    children=[true_map, dorling],).save('/tmp/infographics.example4.%d.png' % year)
```

[Note, we change the size and position of the True-Map]

We get,

![Image](https://cdn-images-1.medium.com/max/800/1*YH9z7V-X9iR_tyVvFY_e_Q.png)

## Example 3: Dorling Cartogram with Progressive Coloring

For completeness, let's also draw the True-Area Map and the Dorling Cartogram with progressive coloring. To implement progressive coloring, we tweak the color functions (_func_get_color_value etc) to consider the proportion of votes the winning party got.

```
def _func_get_color_value(row):    result = pd_to_result[row.id]    party_info = presidential.get_winning_party_info(result)    party_info['p_votes'] = party_info['votes'] / result['summary']['valid']    return party_info
```

```
def _func_value_to_color(party_info):    return party_color.get_rgba_color(        party_info['party_id'],        party_info['p_votes'],        p_to_a=lambda p: max(p - 0.3, 0) / 0.7,    )
```

```
def _func_format_color_value(party_info):    return '{party_id} {p_votes:.0%}'.format(        party_id=party_info['party_id'],        p_votes=party_info['p_votes'],    )
```

We can plot all four permutations (True-Area + Dorling Cartogram x Not-Progressive Coloring + Progressive Coloring) on a single Infographic as follows:

```
Infographic(    title='%d Sri Lankan Presidential Election' % year,    subtitle='By Winning Party',    footer_text='\n'.join(        [            'data from https://elections.gov.lk',            'visualizaiton by @nuuuwan',        ]    ),    children=[        true_map,        dorling,        true_map_prog,        dorling_prog,    ],).save('/tmp/infographics.example6.%d.png' % year)
```

This gives,

![Image](https://cdn-images-1.medium.com/max/800/1*zQAqQpsCTtpKO4zkzMQfSw.png)

## How are Dorling Cartograms Rendered?

The rendering process begins with drawing the circles in their geoprphically correct locations, like this:

![Image](https://cdn-images-1.medium.com/max/800/1*4GJ8VAGUYcLTr4gYIg6goQ.png)

As you can see, circles in densely population areas (like Colombo) overlap. In the next step, we move the overlapping circles away from each other, by making them repel each other.

![Image](https://cdn-images-1.medium.com/max/800/1*YH9z7V-X9iR_tyVvFY_e_Q.png)

## Variations: Bigger and Smaller Circles

LKDorlingCartogram has a parameter "compactness", which defines have much space the circles take. A "compactness" of 100% will be the largest possible extent possible, where the circles will spread across the entire bounding box of the map.

In practice, about 30% is a good compactness.

![Image](https://cdn-images-1.medium.com/max/800/1*SW7U4jGKn5WifLBL4QdsRQ.png)

## Variations: Other Regions and Years

You can draw the same graphs for sub-regions of Sri Lanka by updating the region_id parameter.

```
region_id = 'EC-04'  # Kandy Electoral District
```

![Image](https://cdn-images-1.medium.com/max/800/1*GNmeSdKV6Tww5CY9DdXCaQ.png)

Similarly, you can update year to build results for other years.

```
year = 2015
```

![Image](https://cdn-images-1.medium.com/max/800/1*y04vDQnVMw-DWzv2A0Odvg.png)

## Variations: Other Shapes

You can tweak LKDorlingCartogram to replace circles with other shapes.

```
plotx.draw_circle((x, y), r, fill=color)
```

## Concluding Requests

Please share your thoughts on how these visualizations and the underlying libraries can be improved. Also, feel free to fork or update the code as you feel fit.

#### Article 331 · July 14, 2021

# On Language

The world has two parts: a subjective world that we experience; and an objective world full of information. We cannot say, with certainty, that the latter exist, as we can only experience it through the former. But let's leave that for later.

What is relevant is experience, and how we communicate experience. Communication consists one sharing an experience with another. There is no guarantee that the experience communicated is identical, but there might be some validation that it is at least similar. When I tell you, "there is a cat on the mat", you might look at the mat and confirm, "yes — so there is.". There is no guarantee that what appears to me as a cat, does not appear to you as a dog or an abstract painting. But, at least, we have the same name for experiences that might be different.

This "naming" is the foundation of language. We communicate experiences through giving its various component forms, names; the "cat" and the "mat", for example. The "names" themselves are experiences. They exist only in terms of their sound (the sound of "cat"), what they look like (the shape of the letters that make up the word "cat"), and perhaps other experiences (like how the word "cat" might feel when embossed on wood).

In this way, language is a convention that translates experience to experience. A world where I tell you "there is a cat on the mat", is equivalent to a world where such is the case (assuming I am not lying and not mistaken).

![Image](https://cdn-images-1.medium.com/max/800/1*2xYfcDV26fvtDQlHwgToWA.jpeg)

#### Article 332 · July 14, 2021

# On the Experience Economy

What comes to mind when you hear the words "Experience Economy"?

You might imagine the latest social-media oligarch proselytizing his latest idea to get teenagers to look at cats or babies doing amazing things.

But "Experience Economy" extends far beyond instant gratification and influences. Economics is fundamentally the Economics of Experience, and there is no economy outside the experience economy.

"But wait!" you might say. "I'm an ascetic. I don't care about experiences. I only eat to sustain my body. I gain neither pleasure nor pain from it."

At some level, eating is about objective, real-world things; about sustaining the atoms and molecules of our bodies; about gaining our daily allowance of 2000 calories (or whatever it is).

But no one really eats for objective reasons. We all eat because we want to experience feeling full (or not experience feeling empty), because we want to experience the feeling of strength and health (or not experience weakness or sickness), because we want a "good" experience (and not "bad").

Wikipedia says, "Economics is the social science that studies how people interact with value". They should say, "Economics is the social science that studies how people interact with experiences".

![Image](https://cdn-images-1.medium.com/max/800/1*fAei9IedAWKeelideBR4fQ.jpeg)

#### Article 333 · July 15, 2021

RE: learn how to execute code written...

Fortunately, if you're hitting roadblocks, the odds are that so are other people.

So, whenever you do (e.g. get an error), you should Google it and see how other people dealth with the problem.

https://stackoverflow.com is the usual, goto place for issues. It is usually the top hit when you google a problem/bug/error or other issue.

#### Article 334 · September 3, 2021

# On Data

### Random thoughts

The universe is made of information. You might even say that the universe is information. And with time, the quantity of information is increasing. A physicist might tell you that this is the only credible definition of time. The direction in which information increases.

It's difficult to separate (or even distinguish) data from information. One could say that information and data are two incarnations of the same thing. Information is what something means. While data is what that something is.

Regardless, and just like information, there is a lot of data in the world. A useful subset of this is "digitised data", or data processable by computers. Digitised data is particularly useful because it provides precise (though not always accurate) snapshots of various aspects of our life. For example, your finances listed on a spreadsheet will precisely tell you if you are over-spending (if you have entered the correct data, i.e. the data is accurate).

Digitized Data in particular, and Data in general, is roughly useful in three ways.

* Communication. You can use data to communicate various ideas. The data itself remains unchanged, but when data possessed by one person is shared with another, we can solve more problems.

* Reduction. You can start with a dataset and solve a narrow problem with that data set. For example, you can start with income statistics for the whole of Sri Lanka and conclude which areas suffer from the most amount of poverty.

* Expansion. You can start with a data set and expand it to represent more knowledge. For example, you can start with the results of past elections in Sri Lanka and cluster the country by various areas with specific political affiliations.

All three ways of using data have one thing in common: They all try to answer questions or solve problems. Whether or not data is useful depends on whether we can use it to answer useful questions.

Conversely, if you don't have useful questions, you probably have no use for data.

![Image](https://cdn-images-1.medium.com/max/800/1*NuPKYcXZF_06j0MrtLGn5Q.jpeg)

#### Article 335 · September 25, 2021

### Visualising Sri Lankan Startups

# #StartupScapeSL

### A User Manual

## What?

#StartupScapeSL is a tool for visualising Sri Lankan Tech Startups, various categories of Startups and various information about the Startups on a TreeMap.

Its data source is Startup SL: a platform run by the Information and Communication Technology Agency of Sri Lanka (ICTA).

Currently, there are about 550 Startups. I will update the tool's data every few weeks.

![Image](https://cdn-images-1.medium.com/max/800/1*ZIClNKSjD6_lH2-FfISDBg.png)

## Where?

#StartupScapeSL is currently hosted at https://nuuuwan.github.io/startup-scape-sl/.

I might move it to a more dedicated URL once I get more feedback and clean up the design.

## How?

### Filtering

By default, the tool displays all startups on Startup SL's listing. You can filter by startup category, startup stage or funding stage by clicking the filter icon at the top right of the screen.

![Image](https://cdn-images-1.medium.com/max/800/1*SmRiiOCF89g4uIwbtYHwnQ.gif)

For a description of categories, startup stages and funding stage, please refer to my December 2020 Review of Sri Lankan Tech Startups:

### Detailed Information

You can get more details about a startup by clicking on its image icon:

![Image](https://cdn-images-1.medium.com/max/800/1*bjZPj6m1UQdHF-AhPvhHpQ.gif)

### High-Resolution Downloads

You can download a high-resolution PNG image of #StartupScapeSL by clicking the download icon at the top right of the screen.

![Image](https://cdn-images-1.medium.com/max/800/1*wnOkcX763Llwd8qUYB9E8w.gif)

## Code, Data and Issues

The underlying code is at nuuuwan/startup-scape-sl on GitHub. Feel free to fork or expand on the code.

The underlying data can be download in JSON format from startups.json.

You can report bugs, Feature Ideas or any other issues on the Issues page on the GitHub repo.

## Disclaimers & Caveats

* The listing on Startup SL might not be exhaustive. There are interesting and valuable tech startups known to me that are not listed here.

* Much of the information is self-reported by the startups. Some of it, particularly regarding funding, looks suspect.

Please heed the caveats. The underlying data seems approximate at best. However, with some improvements to data quality and coverage, analyses of this type are likely to be useful.

#### Article 336 · September 27, 2021

Glad it was useful!

#### Article 337 · October 3, 2021

### Sri Lankan Parliamentary Elections

# Proportional Representation, First-Past-the-Post or Both?

A select committee of the Sri Lankan Parliament, headed by Dinesh Gunawardena, is considering reforms to the electoral system and election laws. Among other topics, the electoral system for Parliamentary Elections is under review.

Up to and including 1977, Sri Lankan Parliamentary Elections were conducted under the First-Past-the-Post (FPTP) system; since 1977 under Proportional Representation (PR). The said reforms might consider a return to FPTP, some mix of FPTP and PR, or retaining PR.

This article contains my own thoughts on these various options. As those of you who've read my past articles on Politics known, I'm no expert on Elections or Politics. I'm merely an interested citizen.

## First-Past-the-Post (FPTP)

Until 1977, all our Parliamentary Elections were under FPTP. The country was divided into 160 electorates, each* electing one member to parliament. The candidate winning the most votes got elected.

[* except a small number of "multi-member" electorates. More on that later]

### "Unrepresentative"

A serious problem of FPTP is that it can be "unrepresentative"; the final seat allocation is not proportional to the votes cast; because the winning party gets the seat, irrespective of how many votes it gets.

For example, if three parties contest a seat and get 34%, 33% and 33%, the first party gets the seat. This outcome is no different from a 100%, 0%, 0% vote division.

![Image](https://cdn-images-1.medium.com/max/800/1*36Nm-hMclV2orUrnHSuwMQ.png)

In 1977, the SLFP won ~30% of the votes, but only 8 out of 168 seats (~5%). After winning just over half the vote, the UNP won 140 of 168 seats (exactly 5/6ths).

![Image](https://cdn-images-1.medium.com/max/800/1*V64_cM567YaS7Sxf7p0wNg.png)

In 1970 and July 1960, "unrepresentativeness" reversed the unfairness; the UNP received more votes than the SLFP but won fewer seats.

"Unrepresentativeness" is particularly sensitive when it favours certain groups (e.g. ethnic, economic or religious) over others. Unscrupulous officials can use techniques such as Gerrymandering electorate maps to exploit this weakness. For this reason, within the pre-1977* FPTP system, certain electorates (e.g. Colombo-Central and Nuwara-Eliya), deemed ethnically diverse, were assigned multiple members. Hence, FPTP was adapted to ensure more representativeness and, in this way, making the overall system (a little) more like PR.

![Image](https://cdn-images-1.medium.com/max/800/1*t6RQ3T6d4idAIPG5HNo7Mg.png)

[*By pre-1977, I actually mean "Up to and including 1977]

## Proportional Representation (PR)

Under PR, the number of representatives elected was proportional to the number of votes received. Since (most of the) the pre-1977 electorates had only one member, and since it was not possible to "proportion" one member into "fractions", the concept of "electoral districts" was introduced. An electoral district (ED) is a "super-electorate" with multiple seats. Each party wins a number of seats proportional to the number of votes it wins in the ED.

In the November 2020 Parliamentary Election, 12 Seats were assigned to the Kandy electoral District. The SLPP won 8 seats after winning 59% of the vote, while the SJB won 4 with 29% of the vote. If we used FPTP, the SLPP would have won all the seats in Kandy, having come top in all electorates.

![Image](https://cdn-images-1.medium.com/max/800/1*k8xngiO7ne4xSFnI7y_4pQ.png)

### "Working Majorities"

PR also has its problems. In 5 of the 8 Parliamentary Elections since 1977, the party with the most seats failed to win a majority in parliament and sought smaller parties' support, often after dubious rounds of horse-trading. Hence, some claim that PR makes it difficult to form "working majorities".

![Image](https://cdn-images-1.medium.com/max/800/1*89YYUeEAbKrMi-DI6x9RqQ.png)

To me, this argument is weak. A parliament should be representative of the people, and if no party has the support of a majority of the population, none should enjoy a majority in parliament. More empirically, many countries (including many successful democracies) have "weak parties" forced to form coalitions with other weak parties. Often, weak parties lead to strong democracy — and vice versa.

However, there is a second, stronger argument.

### Weakening the Voter-Representative Link

![Image](https://cdn-images-1.medium.com/max/800/1*gWnwWVOvBhvSk9TiUT2MYg.png)

Consider my home ED, Colombo. In 2020, Colombo elected 19 MPs. Each party and independent group could nominate up to 22 candidates. With over 40 parties and groups contesting, over 800 candidates were contesting Colombo. It is almost impossible for the ordinary voter (myself included) to get one's head around so many candidates. Voters either end up voting for a few candidates with ED spanning brands and bases (E.g. Ranil Wickramasinghe in Colombo, Mahinda Rajapakse in Kurunegala, Chandrika Bandaranaike in Gampaha, etc.) or else vote for only a party and no candidate.

>>> 

It also made it impossible for smaller, more local parties to contest elections. Suppose I wanted to represent my home electorate of Borella. In 2020, the SJB came top in the Borella electorate with 20K votes. Hence, under FPTP, just 20K votes would have won me my home seat. However, under PR, since candidates and parties need to compete across the vast electoral district, spanning about 1.7M voters, a significantly larger number of votes are needed. The JBB, which won a single seat in Colombo, received 67K votes, marginally above the 5% cut-off (60K votes) to make a party eligible for seats.

Hence, PR shifts representation from concrete candidates to abstract (and especially large) parties. It becomes difficult for voters to hold their representatives accountable and for the said representatives to feel accountable towards their voters. The link between voter and representative is weakened or even broken. Small parties have no choice but to join larger parties in (often disadvantageous) collisions.

## Mixed Options

In summary, FPTP can result in unrepresentativeness, while PR can weaken the Voter-Representative Link.

Can there be some compromise? Can we have it both ways? Can we have a system that is both representative and where the link between voter and representative is maintained?

There are several candidate solutions — none perfect. Here are three popular options.

## Option 1: Mixed Member Majoritarian (MMM)

In a Mixed Member Majoritarian (MMM) system, a proportion of the seats are allocated to FPTP and the remainder to PR.

Consider the 2020 Parliamentary Election and the Kandy ED, which was assigned 12 seats. We could split these 12 seats 50%/50%, 6 to FPTP and 6 to PR. Since the SLPP won all the Kandy Electorates, it would get all 6 FPTP seats. If the remaining 6 PR seats were divided, the SLPP would win four and the SJB 2. The final result would be ten seats to the SLPP and two seats to the SJB.

![Image](https://cdn-images-1.medium.com/max/800/1*brgsYAh-JGHB2BA2ZrHxng.png)

While more "unrepresentative" than pure PR, MMM is less "unrepresentative" than pure FPTP.

MMM is used for Parliamentary Elections in many countries, and the FTPT/PR ratio tends to vary significantly. The PR fraction is 18.7% in South Korea, 30% in Taiwan, 37.5% in Japan and 68.7% in Armenia.

## Option 2: Mixed-member proportional representation (MMPR)

Like MMM, in a Mixed-member proportional representation (MMPR) system, seats are split between FPTP and PR. However, unlike MMM, in MMPR, the PR seats are allocated in such a way as to make the final seat allocation proportional.

For example, in the previous Kandy case, of the 6 PR seats, the SLPP would get two, and the SJB would get four so that the final result would be as it was under PR.

![Image](https://cdn-images-1.medium.com/max/800/1*DaVi6ZAK74XxdUPFBXGd8Q.png)

### Overhang

MMPR has the advantage of being as "representative" as pure PR. However, it has the problem of "Overhang seats", where one party wins more FPTP seats than it would win under pure PR.

For example, consider the 2001 election. The Colombo ED had 20 seats, of which the UNP, UPFA and JHU won 9, 8 and 3, respectively. Of the 15 electorates, the UPFA and UNP won 9 and 6, respectively. If we assigned seats according to MMPR with an FPTP-PR ratio of 15–5 (75%-25%), then to achieve the same result as pure PR, we would need to assign the UNP and the JHU 3 seats each take-away one seat from the UPFA.

In practice, one of two solutions is applied to the overhang problem.

* The first is to ignore the overhang. For example, the 5 PR seats might be assigned 3 and 2 to the UNP and JHU, respectively, in our example. The disadvantage of this approach is imperfect proportionality, and hence some "unrepresentativeness". In this example, the unrepresentativeness favours the UPFA against the JHU.

* The second is to add more seats to enable proportionality. For example, if Colombo had 23 seats, the PR assignment would be 10, 9 and 4 to the UNP, UPFA and JHU. After the 15 FPTP seats are assigned, the remaining 8 PR seats can be assigned 4 and 4 to the UNP and JHU, resulting in a match with perfect PR. The downside of this approach is that adding seats might result in parliament having a variable number of members. Also, adding seats to Colombo would mean that seats would have to be added to other EDs to ensure overall representativeness.

## Option 3: Smaller EDs

The weaker link between voters and representatives under PR is worst in large EDs like Colombo and Gampaha, with 18 and 19 seats respectively, and a correspondingly large number of candidates per party and group.

It is less problematic in a smaller ED like Trincomalee, with only four seats. With fewer electorates and fewer candidates, the connection between voter and representative is stronger than a larger ED.

![Image](https://cdn-images-1.medium.com/max/800/1*wgVD6rWxz3SCWo6Sqob5ZA.png)

We can achieve the same effect in a large ED like Colombo by splitting it into smaller EDs. For example, the 19 seats could be split across five smaller EDs, with a maximum of 4 seats each.

While "Smaller Electoral Districts" is not strictly a mixed option and not referred to as one, I listed it here for the following reason: FPTP is an "extreme case" of PR where each electoral district has exactly one seat. General PR puts no limit on the size of the ED. Hence, PR with "Smaller EDs" is somewhere between FPTP and general PR.

On a historical note, the smaller EDs would not be dissimilar to the small number of Multi-Member Electorates that operate within the FPTP system. For example, in 1977, the Colombo-Central and Nuwara-Eliya Electorates (not to be confused with the Colombo and Nuwara-Eliya Districts) had three seats each. The three candidates getting the most number of votes won these seats.

## Concluding Questions

The topics discussed above lead to the following questions:

### Question 1: What would the electorate map look like if we returned to FPTP or adopted some mixed system?

If the Parliamentary Select Committee proposes a return to FPTP or a mixed system, we must redefine electorates and redraw the electoral map. This is because the current electoral districts vary significantly in size.

For example, at the 2012 census, Colombo-West had a population of ~54K, while Kaduwela had 252K or almost five times as large. It would be unrepresentative for both to have one seat each. Hence, Colombo-West would need to be merged into some other electorate, or Kaduwela is split into multiple electorates or both.

![Image](https://cdn-images-1.medium.com/max/800/1*gMWyMYackhuvJJoXohYVBg.png)

### Question 2: How would we split large EDs like Colombo into smaller EDs?

The question would be relevant to Option 3.

### Question 3: How would past election results be different, under different systems?

For example, if the 2020 Parliamentary Election was held under FPTP or some mixed system, would the SLPP have won a 2/3 majority?

I hope to answer these questions in future articles.

...

If you enjoyed reading this article, you might also like,

#### Article 338 · October 7, 2021

# 5 Properties of Good Electoral Maps

### Redrawing Sri Lanka's Electoral Map

In Proportional Representation, First-Past-the-Post or Both, we discussed three alternatives to Proportional Representation (PR) — the Electoral System currently used in Sri Lankan General Elections.

We concluded with three questions, the first of which was,

>>> "What would the Electoral Map look like if we returned to FPTP or adopted some mixed system?".

Before we answer this question, we need to answer a meta-question, namely,

>>> "What properties make a Good Electoral Map?".

In this article, we discuss five such properties.

## 1) Population Balance

(and why we can't use the existing Electoral Map)

The population of an Electoral District or Polling Division must be proportional to the seats assigned to it. We call this property "Population Balance".

For example, Since Sri Lanka has about 20.3M people*, if our new EM has 160 electorates, each must contain about 130K people.

[*All population statistics quoted in this article are from the 2012 census.]

The current EM has significant differences in Population Balance.

At one extreme, the Kayts PD has 40K people. At the other extreme, the giant Nuwara-Eliya PD has 420K. If both PDs elected one MP, Kayts would have 10x as much representation (per capita) in parliament as Nuwara-Eliya.

![Image](https://cdn-images-1.medium.com/max/800/1*sZG3WmyhCbtp4n6HDi-l5Q.png)

Similarly, some EDs have a disproportionately larger or smaller number of PDs than the assigned seats.

If we assigned 160 seats across each ED in proportion to population, Jaffna ED (697K people) would get five seats, while Colombo ED (2.32M) would get 18. However, currently, Jaffna has 11 PDs, while Colombo has only 15. Hence, if we assigned one seat to each existing PD, Jaffna would have almost 2.5x as representation (per capita) as Colombo.

In other words, if we are to use First-Past-the-Post or a Mixed Electoral System, we need a new Electoral Map.

#### Article 339 · October 7, 2021

# How to Draw Sri Lanka's New Electoral Map

### The Electoral Map Mapping Algorithm (EMMA)

We concluded Proportional Representation, First-Past-the-Post or Both? with the three questions including,

>>> "What would the Electoral Map look like if we returned to FPTP or adopted some mixed system?"

In 5 Properties of Good Electoral Maps, we answered a meta-question needed to answer the above, namely,

>>> "What properties make a Good Electoral Map?".

In this article, we describe an "Electoral Map Mapping Algorithm" (EMMA) that will programmatically generate a new Electoral Map for Sri Lanka that both obey the "5 Properties" and might be suitable for FPTP or mixed elections.

#### Article 340 · October 7, 2021

# The New Electoral Map of Sri Lanka

In How to Draw Sri Lanka's New Electoral Map, we discussed the workings of an Electoral Map Mapping Algorithm (EMMA).

As we saw, EMMA takes the Old Electoral Map of Sri Lanka as input. It modifies it step-by-step, gradually making it more and more optimal in terms of the five properties proposed in "5 Properties of Good Electoral Maps". Once "sufficiently optimal", EMMA outputs the New Electoral Map.

In this article, we will look at EMMA's output.

## Assumptions

Before we proceed, let's look at two assumptions that we've made.

### Electoral Map with 160 Polling Divisions each with one seat

EMMA generates an Electoral Map dividing Sri Lanka into 160 Polling Divisions, each with one seat. Since EMMA respects Electoral District (ED) boundaries, these 160 seats are first allocated amongst the 22 Electoral Districts.

![Image](https://cdn-images-1.medium.com/max/800/1*5SoytupXNB1idn3Hcf9PNA.png)

The seats allocated by EMMA to each ED differs from the 2020 (and other) Parliamentary Election Allocations because EMMA allocates only 160 seats to the EDs, while in Parliamentary Elections, 196 seats are allocated (of which 160 are allocated proportionally and 36 based on province, somewhat disproportionally).

### Population vs Registered Voters

EMMA allocates seats proportional to population, while in Parliamentary Elections, the 160 seats allocated proportionally are allocated in proportion to the number of registered voters.

EMMA uses population (from the 2012 census) because it needs population data at the Grama Niladhari Division (GND) level. As of now, we don't have access to registered voters at this level. Hence, EMMA cannot use registered voters for proportional allocation.

Compared to the Parliamentary Elections allocation, EMMA's allocation is likely to favour populations a smaller proportion of registered voters — i.e. those with younger populations.

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

#### Article 342 · October 20, 2021

What proportion of your net worth is Bitcoin?

#### Article 343 · October 30, 2021

# 3 Metaphors for Social Media

### Coping Strategies

## Two Housemates

You have two housemates.

One gives you not a moment's peace. "Talk to me! Talk to me! Talk to me!" it mumbles at all hours. When you are working, sleeping, and at all times in between, you have no respite.

The other housemate is different: A polite friend who would only talk to you at the right time, would not bother you with trivialities, and would only interrupt you in an emergency.

Which housemate would you rather have? Assuming you had the choice? And you do have the choice, don't you?

## Small Town Notice Board

You live in a small town, with a large square. In the middle of this square sits a notice board where anyone can pin messages to anyone else.

How often do you walk into the square and read the notice board? Would once a day would sound reasonable? Would once a week would sound unreasonable?

Alternatively, what if you spend your entire day and much of your night standing next to the notice board? Rain or shine? What if you read and read-read every single thing anyone posted? And what if you analysed and over-analysed every morsel of triviality and gossip?

Which of these people are you? Sane and free, or mad and in chains?

## A New Shirt

Imagine you were out shopping, and you saw a nice T-Shirt. On the one hand, it is quite reasonably priced and is "your type". On the other hand, you don't really need it, because you have so many like it.

Would it harm your life if you didn't buy that T-Shirt? Would you feel such a void in your soul? Would it undermine your contentment and happiness?

What would you do? Must you not walk away?

![Image](https://cdn-images-1.medium.com/max/800/1*aEp7d_6TANqbXtCLysZoRw.jpeg)

#### Article 344 · November 1, 2021

# 2 Types of Internet

### Philosophizing on technology

"What is the internet?" I ask you.

"A collection of devices connected by wires", you reply.

"And what does it do?"

"The devices can communicate information with each other", you continue. "For example, your phone and my phone are part of this network. I type in a message on WhatsApp. Moments later, it reaches your phone. My phone communicates with your phone."

"And has the internet always been like this?"

"More or less."

"Then what has changed?"

"Well", you consider, "More devices are part of the network, more types of devices, and the network itself has got faster, broader, and more reliable."

"And how will it change in the future?"

"It will get faster, broader and more reliable. And more and more devices will join the internet."

I'm silent.

#### Article 345 · November 1, 2021

# The 2 Most Important Questions about Blockchain

### Or how to avoid getting hit by brown-stuff

Some claim that blockchain-based solutions will solve all the world's problems. From poverty to malnutrition, to war, to climate change. A panacea, elixir, and magic potion all rolled into one. These claims might even be true. Or they might not be.

But regardless, we can say one true thing about blockchain. A blockchain system (which typically consists of blockchains managed by peer-to-peer systems forming a distributed ledger) is a database. Or even more simply, a thing that stores data. And any magical powers derive solely from the fact that it is somewhat different from other things that store data.

#### Article 346 · November 3, 2021

# 3 ways in which Decentralized Systems are not Decentralized Systems

### How labels deceive

Decentralization is touted as a key advantage of most decentralized systems.

For example, a crypto-currency built upon a blockchain-based distributed ledger is "decentralized". In contrast, the national monetary system controlled by a central bank is "centralized". The decentralization in the former might be considered an advantage over the latter because members are protected from arbitrary monetary policy (e.g. controlling money supply) by a central authority (e.g. a central bank).

One problem with arguments like this is that the term "decentralization" is vague. What does decentralization mean? Is "decentralization" a binary yes/no, a more nuanced property? How Decentralized are Decentralized systems?

#### Article 347 · November 6, 2021

# On Wisdom

### The "Sour Grapes" Variety and the True Variety

Reality is the state of the universe; it is what is. Desire is our wish to change reality. Hell is a situation where reality and desires don't match; and heaven is when they do.

Note, both hell and heaven exist in degrees. A hell where "I want to each chocolate, but none is available" is very different to a hell where "I want to live comfortably, but this terrorist, dentist or violinist is torturing me."

#### Article 348 · November 7, 2021

# The Great Game

### On Coins, Red Tiles and Beautiful Friends

I toss a coin and try to guess the outcome. It is a game of my own invention: with no other players and no reward, except for the possible pain of losing or the pleasure of winning.

I call "heads" and toss the coin. The coin does, indeed, land "heads".

I feel a small gush of pleasure. Satisfaction. A feeling that I am in some name or form, "better". Conversely, if luck didn't favour me, and the coin landed "tails", I would feel some small, be it ever-so-small, pain. Dissatisfaction. The feeling that I am worse-off.

#### Article 349 · November 26, 2021

# How to invest better

### By playing dice

What do all investments have in common? They all provide you with the opportunity to net some money. How much money? Various investments differ. Some have the potential to net you more money; others less.

Why do opportunities that net you less exist? After all, isn't it rational to invest in whatever opportunity that would net you the most amount of money?

Not quite — because you need to factor in uncertainty — also known as risk. With almost all investments, there is no guarantee of a certain net gain. And opportunities that have a higher average return also tend to have a higher risk.

## Two Imaginary Games

For example, consider the following two dice games: Game A and Game B.

>>> You need to pay Rs. 1000 to play either game.

>>> In-Game A, you win Rs. 12,000 if you throw six and nothing if you don't.

>>> In-Game B, you win Rs. 3000 if you throw 4, 5 or 6, and nothing if you don't.

Which game would you play? That depends.

On the one hand, Game A has an average net return of Rs. 1000 per game (+100%). Game B has an average net return of Rs. 500 per game (+50%).

On the other hand, there is a 5/6 chance that you lose your money from Game A. With Game B, this probability is only 1/2. Hence, while Game A has a higher average return, it is also riskier.

While these are imaginary games, real-world investments have similar properties and implications.

In the next section, I describe some examples. The numbers are approximate and are meant more as qualitative and directional.

## Real Games

### Game 0: Cash

Let's start with a trivial game. "Investing" in Cash is like a trivial dice game where,

>>> You pay Rs. 1000 to play, and you get Rs. 1000 back, whatever the outcome of the dice.

Your average net return is 0%. But your risk is also zero.

### Game 1: Fixed Deposits and "Safe" Fixed Income Investments (E.g. Government Bonds)

>>> You pay Rs. 1000 to play, and you get Rs. 1050 back, whatever the outcome of the dice.

Average net return is +5%. Risk: zero (almost — see next section).

### Game 2: Less "Safe" Fixed Income Investments

Strictly speaking, if you invest your money in a fixed deposit with a reputable bank or government bond, there is a small probability that you will lose your money — e.g. if the bank goes bust or the financial system of the country crashes. This "small probability" is usually much lower than 1/6 [the smallest probability we can represent in our dice game].

However, (say) with a less safe finance company, the probability of a default can be much higher (even 1/6 or more). Usually, such companies give higher interest rates on deposits.

In other words, like a game where,

>>> You pay Rs. 1000 to play, and you get Rs. 1320 back if you throw 2, 3, 4, 5 or 6, and lose your money if you throw 1.

Average net return if the company doesn't go bust: +32% (this is what is usually advertised). Actual average net return +10% (this is what you should consider). 1/6 chance of losing your money.

### Game 3: Stocks (Investing for one year in the Colombo Stock Exchange)

>>> You pay Rs. 1000 to play.

>>> If you throw 1, you get back Rs. 7002: Rs. 9003:Rs. 1,0004: Rs. 1,1005: Rs. 1,3006: Rs. 1,600

Average net return: +10%. Odds of losing all your money: zero. Odds of losing some money: 1/3.

These numbers are based on your earnings in 1 year, had you invested Rs. 1000 in a stock index fund that tracked the Colombo Stock Exchange's ASPI (All Share Price Index) at some random point in time between 1993 and 2021.

### Game 3a: Stocks (Investing for five years)

>>> You pay Rs. 1000 to play.

>>> If you throw 1, you get back Rs. 9002: Rs. 1,0003: Rs. 1,1004: Rs. 1,2005: Rs. 1,3006: Rs. 1,300

Average net return: +13%. Odds of losing all your money: zero. Odds of losing some money: 1/6.

Like Game 3, these numbers are based on ASPI statistics, but considering gains for a 5-year window, annualised.

Note the average return is roughly the same (i.e. the difference is not statistically significant), but the risk of losing some money is considerably smaller (statistically significant).

### Side Topic: Playing many games

Game 3a is equivalent to playing Game 3 five times. In general, if your average return is positive, you can lower your risk by playing the game several times, investing over a longer time window.

However, if you don't have time for a long window (e.g. if you are elderly), then it is best to invest in safer investments.

### Game 4: Entrepreneurship and investing in startups

>>> You pay Rs. 1000 to play.

>>> If you throw a six, you get Rs. 60,000, and nothing if not

Average net return: +999%. Chance of losing money 5/6.

As with the stock market, playing many games is the only way to make money from startups. On the downside, since the risk is much higher, you need to play many more games, compared to the stock market. On the upside, the return is also much, much higher.

### Game 5: Gambling in a Casino

[Not really "investing", but I thought the comparison interesting]

>>> You play Rs. 1000 to play.

>>> If you throw a six, you get Rs. 5,833, and nothing if not.

Average net return: -3%. Chance of losing money 5/6.

These numbers are based on the 35/36 odds that most casinos are supposed to have. For every Rs. 36 gambled, the house gets Rs. 1, and the remainder is returned to the players.

Hence, unlike proper investments, gambling has a negative average net return. Playing many games will not help. The more you play, the more you lose.

### Game 6: Insurance

While you probably don't consider "Insurance" an investment, it tends to behave like it is. Consider this toy example:

Suppose you have a car worth Rs. 5,000, and suppose the odds of crashing it are 1/6. If you don't have insurance, there is a 5/6 that you don't lose anything and a 1/6 chance of losing Rs. 5,000.

Now, suppose you get car insurance, which costs Rs. 1,000. There is a 5/6 chance that you don't crash your car, and you lose your insurance money, and a 1/6 chance that you crash your car, and the insurance company reimburses you.

The "net effect" of insurance is the difference between the two. In other words, there is a 5/6 chance of losing the Rs. 5,000 insurance fee, and 1/6 chance of netting the difference between the insured amount and the fee.

It is like a dice game where,

>>> You play Rs. 1,000 to play.

>>> If you throw six, you get Rs. 5,000, and nothing if not.

Average net return: -17%. Chance of losing money 5/6.

Note, obviously, the numbers above are unrealistic. Even the worst driver will have better than 1/6 odds, and no car has cost Rs. 5,000 since World War II (or I?). But as I said earlier, I meant the numbers to be directional and qualitative. Or in other words, to highlight the purpose of insurance: losing a little money instead of losing a lot.

In a sense, life is like gambling in a casino. And directionally, the odds are similar. However, unlike gambling in a casino, we have no choice, but to play the game. Insurance makes the odds (and life) a bit more bearable.

## Concluding Disclaimers

The goal of this article was less to provide concrete financial advice and more to provide some intuitions about investment options.

I'm no financial adviser, so please consult a proper professional for sounder financial advice.

![Image](https://cdn-images-1.medium.com/max/800/1*IAcbCwU3waPOxISiQjmDQQ.jpeg)

#### Article 350 · December 6, 2021

# Antifragile Algorithms

### Or Beyond Robust Programming

Most algorithms a Fragile. A few are Robust. This article is how we can do even better than Robust: How we can write Antifragile algorithms.

## Fragile, Robust, and Antifragile

In his classic book, Antifragile: Things That Gain from Disorder, Nassim Taleb differentiates between three types of things: the Fragile, the Robust, and the Antifragile.

Fragile things suffer from even small amounts of stress or noise. For example, you are likely to label a crate of crystal glasses as "Fragile" or "Handle with care" because even a small amount of mishandling (i.e. stress or noise) will break the glasses.

In contrast, if you were shipping packets of salt or bars of gold, you would not label their containers "Fragile". You're unlikely to label anything because mishandling or not, they are likely to remain unchanged and undamaged. We refer to this quality of remaining undamaged with stresses and noise as "Robustness".

You might say "Robustness" is the opposite of "Fragile". But this is like saying the opposite of "negative" is "zero", or the opposite of losing money is "not losing money".

The opposite of "negative" is "positive", and the opposite of "losing money" is gaining money. Similarly, the opposite of becoming damaged in the face of small stresses is improving in the face of small stresses. If you were transporting some good (I don't know what), which was Antifragile, you would mark the crate "Please handle carelessly".

Now, what if Algorithms could be Antifragile?

## Fragile Algorithms

Suppose you wanted to scrape a news article from the newspaper's website. Suppose you built a very simple scrape that identified the title of the article and the body of the article.

Suppose an h1 HTML tag always contained the title, a p HTML tag contained the body, and there was no other content with these tags.

```
<h1>Another Gas Explosion in Fartington City</h1><p>Our Fartington correspondent reports that yet another...</p>
```

To find the title and body, you need to find the h1 and p tags. If you used BeautifulSoup for parsing HTML, your code would look something like this:

```
soup = BeautifulSoup(html, ‘html.parser')article_title = soup.find(‘h1')article_body = soup.find(‘p')
```

This parser is simple, which is good. But it is also Fragile; a very small stress or noise will break or deteriorate it.

What is a small stress or noise in the Algorithms world? A small change that will break the algorithm. For example, what if the designer of the news site replaces the h1 tag of the title with a different tag?

```
<div class="div-article-heading">   Another Gas Explosion in Fartington City</div>
```

You might also confront this stress if you use the same algorithm to crawl a different news site.

## Robust Algorithms

A simple way of making your crawling algorithm more robust would be to look for different patterns of potential headings. For example, you could do something like,

```
title = soup.find(‘h1')if not title:    title = soup.find(‘div', class_='div-article-heading'):
```

You can make your algorithm even more robust by detecting the title in some more generic way. For example, you could detect the font size and weight of the various text types and determine that the "title" was the biggest and boldest.

As I hinted, this algorithm is more robust. The algorithm doesn't break or deteriorate with noise and stress (i.e. changes to the article format).

## Antifragile Algorithms

But what if we could do even better? What if our algorithm improved with noise and stress? What if there existed a news article parsing algorithm that got better as it parsed more and more various and different news sites?

Some might suggest a Supervised Learning Algorithm, where you input many examples of news websites, along with their titles and bodies. The algorithm would learn to parse the title and body and get better with more and more examples. In this sense, this Supervised Learning Algorithm is Antifragile.

However, Supervised Learning is, in a sense, cheating because you are "helping" it with training data, a benefit that our other algorithms didn't have. On the other hand, an Unsupervised Learning Algorithm could be both Antifragile and work without help.

Here's a very broad outline of what it might look like:

```
for many articles:    find various types of text found in that articlefor these various types of text:    exclude common text like links and other generic items    find "title-like" text    find "body-like" text
```

![Image](https://cdn-images-1.medium.com/max/800/1*ywt285wmOf3wPPJYvzp_pw.png)

## Concluding Generalizations

In many situations, designing Antifragile products or systems is difficult and counter-intuitive. However, in some situations (like News Article Crawling), we often write Fragile algorithms because it is easy, and because we don't think "Antifragile first". In general, we (programmers) should look for the Antifragile option first.