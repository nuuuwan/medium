#### Article 100 · September 15, 2019

# On SWE Interviews

### Why an interview loop is a collection of ANDs

Recently, I interviewed two very different candidates for the same Software Engineer (SWE) role.

The first (let's call him "Ajith") had excelled in academics, achived a top-20 rank at the A. Level exam, and graduated near the top of his class at university. The second (let's call her "Buddhi"), had good (but not great) performance in her A. Level and at university (incidentally, the same program as Ajith).

Ajith, however, failed his onsite interview badly. Not only was he unable to complete several easy coding questions, he had trouble communicating, and seemed to have little interest in the company. Buddhi, in contrast, aced her coding interview, which included some very difficult questions, seemed very enthusiastic about the company and had behavioural skills to match.

>>> Now, who should we have hired? Ajith or Buddhi?

This decision might not be as clear-cut as it seems when you consider the following:

* Ajith might have failed the onsite interview, but he has clearly better academic results than Buddhi.These tests, unlike the onsite interview, are based on mostly objective, standardized tests taken by 100,000s of candidates each year. Hence, Ajith's accomplishments might be considered far more fair and unbiased.

* On the other hand, these standardized test (though objective), measure a very narrow set of skills. For example, why would A-grades for mathematics, physics and chemsitry make a good SWE? While scores for mathematics or physics might correlate with aptitude in some Computer Science subjects, they hardly cover all the skills that a good SWE should have.

* While Buddhi might have had a weaker academic record, she is clearly better than Ajith on the dimensions that the role requires (see On Software Engineer).

* On the other hand, the methods used to test these dimensions (onsite interviews) are highly subjective. For example, my opinion as an interviewer could be biased.

* On yet another hand, the types of things a good SWE should have are complex and subtle. And a standardized test cannot capture these types of nuances. Hence, the only solution is a subjective interview.

So what do we do?

## Three types of skills

Our scenario involves three types of skills:

* Skills necessary to get good scores at A. Levels and University

* Skills necessary to be a good SWE

* Skills necessary to pass a SWE Interview

From my experience, most good SWEs also have good scores at A. Levels and University. However, not all candidates with good scores at A. Levels and University have the potential to be good SWEs. There are also a few SWEs who have poor scores at A. Levels or University.

![Image](https://cdn-images-1.medium.com/max/800/1*TLq0wiMonxSA0khVNXAgRA.png)

Hence, a company wishing to hire SWEs would usually use "scores at A. Levels and University" as a filtering factor. Since most good SWEs also have good scores, we reject those who have poor scores. We would have a few potential good SWEs that we reject ("false negatives"), but this is considered preferable to hiring candidates who end up being poor SWEs ("false positives"). This last point is important.

Both Ajith and Buddhi would have passed this initial filter.

Once this filtering process is complete, we need to identify and select those candidates who, in addition to having good scores at A. Levels and University, also have the potential to be good SWEs. Onsite interviews generally focus on this differentiation.

![Image](https://cdn-images-1.medium.com/max/800/1*zhdPzEJZ9LTfiJW_SOQZAg.png)

As before, we consider "false negatives" preferable to "false positives". Hence, there tend to be relatively more potentially good SWE candidates we rejects, compared to bad SWE candidates we hire.

![Image](https://cdn-images-1.medium.com/max/800/1*OMqT6UAdvcZ-gp9uprsPNw.png)

## Ajith and Buddhi

Given that both the filtering process and the onsite interviews favour "false negatives" over "false positives", very few bad candidates pass both stages. Hence, it is highly likely that Buddhi would end-up being a good SWE candidate.

![Image](https://cdn-images-1.medium.com/max/800/1*Vp3Q3HUKXzR8Lvg4HapTlw.png)

Unfortunately, by the same policy ("false negatives" over "false positives") it is also highly likely that Ajith could be a good SWE candidate, but didn't pass our interview bar. But this is by design.

## My Point

The key principle is: "It is much less painful not to hire a good candidate, than to hire a bad one and bear the consequences."

Hence we structure the interview loop as an "AND" of several factors, including objective standardised tests, and subjective onsite interviews. Ajith passed one, but failed the other. Buddhi passed both ("test scores" AND "onsite"), even though she was not as good as Ajith on one ("test scores").

A good candidate might not pass all of these ANDed tests, but a bad candidate would almost certainly fail at least one of them.

[Note: For simplicity, I've described the ANDing of two factors. In practice, there could be more.]

...

## Caveat Emptor

In theory, while these recommendations might be optimal, there are some practical situations where it might not be so. Let's look at some of these scenarios next.

### Bad Interviews

There are at least two types of bad interviews.

The worst type of interview is where the interviewers are so weak, that they are unable to provide any signal beyond parotting obvious things (like A. Level and university scores), on which they tend to be more conservative than necessary. These interviews invariably result in "false positives" (like Buddhi getting rejected), but also "false negatives" (like a potentially poor SWE "Chamal" getting hired).

![Image](https://cdn-images-1.medium.com/max/800/1*hLAfRckGqqc6ss5yXikJIQ.png)

A slightly less dangerous interview is one which is completely irrelevant, that no one ever gets hired. Note, this is less dangerous, because almost always, a bad hire is worse than a no hire.

![Image](https://cdn-images-1.medium.com/max/800/1*Q-CbBkgjXjQkFGfagtMfCg.png)

### Poor Filtering

A company might have a good interview loop, but poor filtering. In addition to "false negatives" (like Ajith), this might also lead to some "false positives" (like candidate "Dumbo", who has poor SWE potential, but passes both the filtering and interview stages).

![Image](https://cdn-images-1.medium.com/max/800/1*wueIYIXbqvdP_oq0i_DYfw.png)

### The C-grade Company

In On Software Engineers I said,

>>> "Many organisations that care more about shorter-term profits, will be happy to hire C-grade SWEs or less. These [C-grade] organisations, usually, don't produce new intellectual property, or product design, merely translate requirements specs (usually developed abroad) into code"

Now, if you're a C-grade organization, none of what I said matters. Any human would probably make a good enough SWE. Hence, you could do away with filtering and interviews, and hire anyone looking to join you.

![Image](https://cdn-images-1.medium.com/max/800/1*91TCm35fQ4i9BYEg_xltnw.png)