#### Article 52 · August 10, 2019

# On Coding Interviews

### And its many faces

Recently, I had the following (paraphrased) conversation with a Engineering VP of a well-known tech-company in Colombo:

>>> CTO: So many of our SWEs can't write proper code. 😔

>>> Me: Didn't they have a coding interview?

>>> CTO: No.

>>> Me: But why did you hire them? 😮

>>> CTO: Their resumes looked great. Top ranks in A.Levels, and Top GPAs from university. Several of them came recommended from several professors known to me.

>>> Me: 🙈

All SWEs (Software Engineers) should be able to code (among many other things [1]). And, if you're looking to hire one, you should check if they cancode. Unfortunately, too many people assume candidates who look good can also code good. This is seldom the case, because, for a start, while these factors might correlate with coding ability, they are necessarily not causal. What makes a high scoring student doesn't necessarily make a good coder.

Another problem as bad as not interviewing, is an interview process that has insufficient signal on coding ability. This is usually due to two reason:

* Organisations assume that interviews are too expensive (both time and money).

* Organisations don't know how to interpret the results of interviews.

A sophisticated interview process is expensive in an absolute sense. But SWEs (in particular) are "high margin employees". The profits most tech companies earn per SWE, is often several times the cost of hiring, remunerating and maintaining a SWE. For example, a SWE costing 300,000 LKR per month (salary + benefits + taxes +other overheads), usually leads to incremental profits of anything from 600,000 to 3,000,000 LKR per month. Hence, while a sophisticated interview process might be expensive in an absolute sense, it is actually cheap relative to the benefits of hiring good people.

In the rest of this article, I describe a sophisticated coding interview process, which is both economical, and has high signal.

## Face 1: The Offline Puzzle

When you want to hire a SWE, you design some job description and share it on your network, on job sites, and on social media. Many potential SWE candidates might see your advertisement, and some of them will be interested in the job.

At this point, you could ask the candidates to send in their resumes and other details. In addition to this, you also want to assess if they are actually interested.

A simple technique that assesses interest is to ask the candidates to solve a coding puzzle. This puzzle can be sent over email, or using a website like hackerrank.com(which has all sorts of useful tools). This is the simplest "face" of the coding interview.

A good puzzle should not be too difficult, and take about 10–30 minutes to solve. Less than 10 minutes and the problem might be trivial. More than 30 minutes, and the candidate might give-up interest.

At the end of this step, candidates who are not interested drop out.

[Note, it is possible that the candidate cheats and copies the answer off the internet, or asks a friend to solve it. This is ok. There will be plenty of opportunities to catch cheats later in the process.]

## Face 2: The Phone Screen

Candidates who complete the Offline Puzzle will qualify for the phone screen.

### Properties of interviews

Each of the "faces" of the coding interview, have several contrasting properties:

* Signal: The type of signal you're looking to get

* Cost: The cost of the interview

* Conversion Rate: How many people pass the interview.

* Volume: How many candidates you should interview

In the Offline Puzzle, the signal was interest, the cost was cheap, the conversion rate is probably low (because many people who say they are interested, actually are not), and as a result you need to interview more people (high volume).

In the Phone Screen, the signal is "actual coding ability". While seeing and hearing someone coding live, you should be able to get some sense of how they think, how creative they are, what attention they pay to writing clean code, testing, debugging etc, and other good practices. The cost is much higher because you need a reasonably experience interviewer to spend a non-trivial amount of time on the interview. We will discuss conversion rates and volumes in the conclusion in more detail.

## Face 3: The Onsite Interview Session

Candidates who pass the Phone Screen can (probably) code. So why have an onsite interview?

Given how fundamental coding is to what a SWE does, it is usually valuable to get more signal on coding ability, in-person, ideally by several different interviewers. The onsite coding interviews are a more detailed version of the phone screen where 2–6 difficult coding questions are asked by 1–3 interviewers. In addition to these coding questions (which usually focus on Data Structures and Algorithms), candidates should also be tested on higher level system design and architecture skills.

An onsite interview is also vital for assessing non-technical abilities like social, behavioural, and cultural skills, motivation and mindset. For more details, see [1].

The onsite interview is also a good opportunity to "market" the organization to the candidate, and "show them around".

## The Full Interview "Process"

From my experience*, about 20% of those who pass the Phone Screen, will pass the Onsite Interview. Assuming similar conversion rates for Advertising to Offline Puzzle and Offline Puzzle to Phone Screen, and also assuming that candidates always accept your offers, to hire one SWE, you'll need to do 5 Onsite Interviews, 25 Phone Screens, and 125 Offline Puzzles.

[*Disclaimer: These numbers should vary depending on organisation, role and other factors. You should replace my guesstimates with your ow, better statistics].

Now, this might seem like a lot of coding interviews (5 + 25 + 125 = 155 in total) for one hire. But most of these are Offline Puzzles, which have little incremental cost per interview.

The conversion rates also give you some sense of how much time and money you should spend on each interview. Since any candidate going through a Onsite Interview Session is 5x more likely to get hired than one going through a Phone Screen, you should look to spend 5x time and money on these. The main cost of each of these interviews is the time spent by the interviewer, the Onsite Interview Session should be about 5x the length of a Phone Screen. For example, if the Phone Screen is 30 minutes, the OnSite Interview Session should be 2 hours and 30 minutes.

![Image](https://cdn-images-1.medium.com/max/800/1*I3Qn60xMLSRH6fmXnwe5RQ.png)

## Concluding Take Aways

The humble coding interview is quite sophisticated and has many faces, with contrasting properties. Understanding these will help you hire good candidates efficiently and economically

### References

[1] https://medium.com/on-technology/on-software-engineers-f16bdafef43d