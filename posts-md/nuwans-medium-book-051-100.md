# Book 2

#### Articles 51 to 100

#### Article 51 · August 9, 2019

# On Software Engineers

### And recruiting them

>>> "How do we hire really good Software Engineers?"

A common question I get these days.

In this article, I've attempted to answer this question, mostly based on my experience recruiting Software Engineers (SWEs) and Engineering Managers at Facebook (2009–2017). While I focus on the SWE role, many of the ideas presented can be applied to other roles.

## C-grade Candidates

Every profession has some core professional skills. For example, a Software Engineer should be able to write code; a Data Scientists should be able to analyse data; a Designer should be able to design Web Sites. The most basic employment candidate is one who has these basic skills for the role. This is what I mean by a C-grade Candidate.

As I mentioned, a SWE should be able to code. The way you test a potential SWE candidate for C-level abilities, is through a "coding interview". At Facebook, these were known as "Ninja" interviews, consisting of Data Structures and Algorithms questions.

>>> What types of questions? Should we test particular programming languages? What about frameworks?

Whenever a candidate describes themselves as "an expert in Java" or "an expert in Angular JS", I hear alarm bells ringing. This is because in a world where technology is changing so fast, being rigidly married to a single technology is a sign of inability to adapt, and learn.

Hence, coding interviews should focus on fundamentals and creativity, not programming languages and frameworks that a creative candidate with the fundamentals can learn in a few weeks anyway.

In addition to these "Ninja" coding interviews, Facebook also had a separate interview which tested high level system and architectural design ability, known as a "Pirate" interview. Like the "Ninja" the pirates tested creativity, the ability to think "outside-the-box" and not being married to fixed concepts and technology.

## B-grade Candidates

Organizations are complex organisms, with many people playing different roles. These roles coexist and collaborate, contributing to a common whole. For example, product teams at Facebook were a partnership between Software Engineers and Engineering Managers, Product Managers, Designers, Researches, and Data Scientists. It was impossible for a Engineer to do their job properly, without understanding and collaborting with, say, a Designer.

Hence, working in a complex organisation requires a set of social, behavioural and cultural skills that enable one to work well with others. B-grade candidates have all the core professional skills that C-grade candidates have, plus these social, behavioural and cultural skills.

At Facebook, these B-level skills were tested in an interview known as the "Jedi". Questions focussed on a wide range of behavioural situations, from resolving conflicts, to working in teams, to understanding the purpose and importance of other roles.

### On "Minders"

Many organisations underestimate the added value of B-level skills, and are happy to hire just C-grade candidates. This is usually not too serious for junior candidates (e.g. SWEs newly graduated from universities), but fast becomes a big problem as the candidate gets older, and acquires more responsibilities.

While it is possible for a junior SWEs interactions with the "outside world" (i.e. other roles) to be minimal, senior SWEs have to actively collaborate externally. C-grade candidates struggle at this, because they possess few social, behavioural and cultural skills. Often they cause conflicts, which tend to escalate into even larger conflicts.

Most organisations solve this problem by creating a "communications layer" between socially in-ept C-grade candidates, and the outside world — usually, in the form of a project manager. The additional overhead caused by these "minders" not only slow down the development process, but create unhealthy organisational tensions. For example, SWEs are constantly aware that their "minders" don't contribute ideas or intellectual property, but usually take the credit for their accomplishments.

## A-grade Candidates

The best candidates have, in addition to professional skills (C) and social, behavioural and cultural skills (B), the right mindset and motivation to work well in an organization. The best candidates believe in what the company does and want to contribute to that mission, irrespective of compensation and prestige (If a candidates too many questions about salary, and titles, that indicates that their motivations might not be completely aligned with the companies).

The best candidates are constantly trying to improve, and want to grow all the time. This "growth mindset" is what I mean by the right mindset. A-grade candidates tended to have strong philosophies about their own personal growth, and what they expected of organizations.

There was no dedicated interview for detecting A-level skills at Facebook. Instead, throughout the other interviewers ("Ninja", "Pirate", "Jedi") the interviews were constantly on the look out for evidence of A-level skills.

## Concluding thought: A-grade organisations

There is one clear advantage in hiring C-grade SWEs overs Bs or As; they are much cheaper. In Sri Lanka, a A-grade SWEs, straight out of university could have a starting salary of 180,000 LKR per month or more. On the other hand, there are C-grade SWEs with 10 years of experience earning less than a third of that.

Hence, many organisations that care more about shorter-term profits, will be happy to hire C-grade SWEs or less. These organisations, usually, don't produce new intellectual property, or product design, merely translate requirements specs (usually developed abroad) into code. While this model is still common, and has been historically dominant in Sri Lanka, it is quickly going away — especially with rising living standards locally, and developments such as AI globally.

To me, the future is one of A-grade SWEs and A-grade organisations (i.e. organisations that want to hire A-grade SWEs). Hence, I hope this primer will be useful!

![Image](https://cdn-images-1.medium.com/max/800/1*xMsJwPaRQ-qGkmThSrz76w.png)

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

#### Article 53 · August 11, 2019

# On Goals, Skills and Aspirations

### And their implications

![Image](https://cdn-images-1.medium.com/max/800/1*pGoDmUMZxMSBYEVPst19yA.png)

An organization must align its employees behind its goals. Everyone should be doing "What they should do".

On the other hand, employees work at the organization to satisfy their needs. For example, they are paid a salary which satisfies their physical and safety needs. They interact within the organization, which might satisfy some of their needs for friendship and esteem. The best organizations might also allow their employees the opportunity to self actualize and grow. In other words, employees work in organizations because they can do (to various extents) "What they want to do".

But finally, all of these must be realistic. On one hand, these align with the skills possessed by the employees, and other the hand, the environment and resources provided by the organization. At the end of the day, people can only do "what they can do".

## What does this mean for organizations?

* Have the right "should do" (Mission, Vision, Strategy, Tactics)

* Hire people who "want to do" (Motivation)

* Hire people who "can do" (Skill)

* Create an environment and provide resources enabling "can do"

## What does this mean for employees?

* Join organizations where you "should do" what you "can do" and what you "want to do"

#### Article 54 · August 12, 2019

# How not to pick a President

### On Cognitive Biases

>>> Who will be the next president of Sri Lanka?

Gotabhaya Rajapaksa recently announced his candidature from the SLPP [1], and there is some parallel speculation on who will contest from the UNP.

And while political high-ups make their decisions, there is also a lot of talk and gossip amongst "ordinary voters" on who should be the president, and how they should vote.

>>> But, how does one decide?

## How we should decide

Picking a president is a complex decision. The rational thing to do would be something like the following:

* Collect as much information about the candidate's record and those of their affiliates

* Project it into the future

* Consider its implications for the country.

It is convenient to "visualize" this information among two dimensions:

* Good Outcomes vs Bad Outcomes

* Voluntary vs Involuntary

We want a president whose actions will result in "Good Outcomes" as opposed to "Bad Outcomes". At the same time, we'd prefer these "Good Outcomes" to arise from voluntary good deeds and policies, as opposed to luck. Hence, for each candidate, we find as much information about the four quadrants of the two-dimensional picture. Then, we base our decision off that.

![Image](https://cdn-images-1.medium.com/max/800/1*QNIF-E2oDkLPPvcFha9AMg.png)

## How we actually decide

But let me confess: I don't know anyone in Sri Lanka (or any other country, for that matter) who has picked a president (or head-of-state) using this "algorithm".

In reality, our "algorithm" is far simpler, and sadly stupider. Here are some ways in which we actually decide.

### Extreme Event Bias

While a candidate might have done and caused many things, many people vote (or don't vote) for them based on one extreme event.

For example, many people voted for Mahinda Rajapakse purely on the basis that he "won the war". Similarly, many people voted against George W. Bush because he (somehow) "caused 9/11".

This bias towards extremes and forgetting the middle (as most biases), derives from our instinct to be risk-averse, which itself stems from our need to survive.

### Anchor Bias

"Anchoring" consists of choosing a candidate based on some factor that has little to do with the candidate.

For example, in Sri Lanka, much the electorate picks a candidate based, not on policy or record, but party ("කැපුවත් කොළ" or "කැපුවත් නිල්" or "කැපුවත් රතු" types). Another standard anchor is "who my family votes for".

In a stranger case of anchoring, a cousin of mine voted for one party, because her husband voted for the other party. Her logic was not actually antipathy towards her spouse, but a sort of "vote hedging". This sort of "negative-anchoring" is as irrational as the "positive" variety.

### Familiarity Bias

Posters, placards and paper handouts are frequent during election season and even off-season. Candidates also clamour for prime-time TV minutes, and our increasingly spending more money on social media advertising.

These tactics play straight into a common voter bias. Voters are more likely to vote for a "familiar" candidate, regardless of who they are or what they will do.

### Sunk Cost Bias

Suppose you voted for some candidate. Then, suppose that the candidate performed abysmally in their term in office. What will you do in the next election?

The rational thing to do would be to vote for someone else. But that would make your first decision a "stupid decision". It would make you look "stupid".

So you post-rationalize some vague justification that the candidate's term was actually "not too bad". And you vote for them again.

## Conclusion

These are just a few examples of many cognitive biases. You can learn about more in [2].

All voters are guilty of these cognitive biases, to some extent, and politicians know and exploit them. The antidote to prejudice is awareness; to be mindful of our propensity to err, and correct ourselves when we do.

So if there is one thing you'll take away from this article, ask yourself this:

>>> "Why have I picked this candidate? Is this a rational decision, or do cognitive biases overly influence me?"

## References

[1] http://www.dailymirror.lk/caption_story/MR--SLPP-Leader---Gota--presidential-candidate/110-172687

[2] The Art of Thinking Clearly, Rolf Dobelli

#### Article 55 · August 13, 2019

# August 13, 2019

### Follow-ups/ideas from meetings, reading

### On Naming Things [1]

Can we talk about anything without that thing existing in our mind? For example, when we say "George Washington liked apples" doesn't some abstraction of George Washington live in our heads?

### On Democracy [1]

What is the ultimate justification for Democracy?

### On Universals [1]

What is the point of universals? And primitives?

### On Sparta [1]

Were the Spartan's actually successful? Were they better or worse than the other Greek states? How is one state better or worse than another?

### On Dynamic Pricing

What is it and how does it work?

### On Dividing Equity

How should the founders of startups choose to divide equity?

### On Test Driven Development

How can Development and Testing merged? More generally, how can human coders be restricted to only doing creative and interesting things, and machines be assigned all the boring non-creative tasks?

### On Randomness

Is a (fair) coin toss random? As you toss it multiple times, the number of heads converges to the number of tails. This is predictable. Hence, is it random?

### On Creately [2]

Should use it more often. How does one start expressing an idea in the form of a picture or diagram? What sort of things will encourage that "first step"?

### On Writing

Why should one write? What are the benefits of writing? What can I write about writing?

### BR on Writing [1]

First emerse yourself in the content. When the content will write itself. Should I write some Algorithm for writing?

### On Humans vs. Machines

Drawing a clear line. Creativity. The future of jobs. AI.

### On Design, and testing designs

The Noob test. The Drawing test. What other test might there? I should have something which I can pass on to a designer and get some feedback.

### —

[1] A History of Western Philosophy, Bertrand Russell

[2] https://app.creately.com/manage/recent

#### Article 56 · August 13, 2019

# On Freewill

### Speculations of an Agnostic

![Image](https://cdn-images-1.medium.com/max/800/1*bxuYPpmd284j1zIYxgiMtQ.png)

There is a cup of coffee on the small table in front of me. It is white, with bands of black. There is a stream of white steam drifting from about it. Should I pick it up and take a sip? Or let it cool?

Either way, the choice seems to be mine. I can choose to pick-up or not to pick-up. I have the freedom to will. Freewill.

Or so I might believe.

Most materialistic scientist say otherwise. They suggest that the choice to pick-up was not mine, but pre-determined by various external factors, like the weather or chemicals and electrical signals in my brain.

There are two factors that compound this free-will vs no free-will debate.

* Materialism. Science deals with material observations, or things we can materially observe. Like the weather, or the chemical and electrical signals in my brain. Materialists don't care about what I'm thinking, or what I'm "conscious" of.

* Observation. While Observation is core to science, it cares little about the observer. It assumes that what is consistently observed by many observers (in a relative sense), must be valid.

Is there some middle ground which merges the two conflicting sides of the free-will vs no free-will debate?

Here's one speculation:

>>> Suppose there is no free will, and nothing can control or influence the universe. Hence, the universe consists of random states, which are uncertain, unpredictable, and unknowable.

>>> Now suppose when we observe the universe, we can observe not all these states, but a subset of these states, and we can "choose" what subsets we observe. Hence, I can choose to see the states where I "choose to pick-up the cup". Similarly, I can also choose to see those states where I didn't pick up the cup. Any "external observer" also has these choices.

>>> In such a scheme, both the "illusion of free will" (for both "self" and "external observer") and the "lack of free-will" are both preserved.

What do you think?

#### Article 57 · August 14, 2019

# August 14, 2019

Poya. Mostly at home.

### On Human Competence

Need to expand on this topic. Education in particular. From first principles.

### The Oval Office and the Press Office

On thinking in general, but also the interplay between the two "offices".

### On Negative Feedback

The story of the colleague who was afraid of me.

#### Article 58 · August 14, 2019

It's an interesting question.

Physics seems to agree with the infinite probability space idea also. But (as in other cases) says nothing about the process of observation. That is probably key to answering this question: i.e. defining what "to observe" means.

#### Article 59 · August 14, 2019

# On Artificial Intelligence

### And why we need to study Human Competence

## A Brief History of AI

### Definition 1: Machines that solve problems the way humans solve problems

The first attempts at Artificial Intelligence (AI) in the mid 20th century, attempted to mimic the human brain. Early Computer Scientists were fascinated at how simple artificial neural networks, which had a general resemblance to the neurones and synaptic connections of the brain, could solve simple problems. Many hailed a new age, and a new type of computer which could end-up solving all problems humans could solve, and attain and surpass human intelligence.

This euphoria was short-lived and died down. Firstly, due to hardware constraints, early AI systems could not scale beyond toy problems. Secondly, there was more and more debate and controversy on how exactly human intelligence worked, and how humans solve problems. Humans had little consensus on what "Human Intelligence" meant, let alone the "Artificial" variety. Finally, there were systems which bore no resemblance to the brain what-so-ever but could still solve interesting and "intelligent" problems.

### Definition 2: Machines that solve problems that humans used to solve better than machines, better than humans

Hence, the focus moved away from "how" machines solved problems to "what" problems machines solved. Computer Scientists have focussed on getting machines to solve intelligent problems while leaving the definition and study of intelligence to philosophers and psychologists.

However, "intelligence" was still poorly defined. What made a problem an intelligent problem?

Computer Scientists adopted the somewhat problematic definition of defining an "Intelligent Problem" as problems that "humans can solve better than machines". Playing complex games like Chess, or recognizing hand-writing, or writing "creatively", were all considered examples of "intelligent problems", because at the time, humans could solve them better than machines.

This definition was problematic because the moment a machine could solve an intelligent problem better than a human, the problem ceased to be an "intelligent problem" (by definition). Hence, as computers got better an better at playing Chess, eventually beating grand-masters, playing Chess was considered less AI and more mechanical machine task.

### Definition 3: Machines that solve problems, that humans can't solve

The last decade has seen an explosion in data collection and hardware capable of processing this data. In parallel, new software algorithms capable of exploiting these data and hardware trends have developed (e.g. Deep Learning algorithms).

Processing tera-bytes of data is beyond any human. Hence, the latest incarnation of AI attempts to solve problems that humans can't solve. While we still use anthropomorphic words like "Intelligence", AI is increasingly diverging from human intelligence.

Hence, the future of AI has no bounds. Any problem is fair game. Many of these problems are currently solved by humans, and these humans are at risk of loosing their jobs.

## On Competence

While I've used the word "Intelligence" several times in this article, I don't really know what that word actually means. Nor do other computer scientists, philosophers, or psychologists. There is a lot of interesting discussion and debate, but no consistent and widely recognized definition.

But for all practical purposes, when we say "Artificial Intelligence" we mean "Artificial Competence" or "a machines ability to solve problems".

While we might know what a specific machine is capable of, we have no sense of what machines can do "in general". Or the "set of all problems that machines can solve". The converse question is also interesting: "the set of all problems that machines cannot solve", and its subset "the set of all problems that machines cannot solve, but humans can".

## On Human Competence

Throughout most of the last 200 years, our notion of "Human Competence" or "the set of all problems humans can solve" has changed little. Many human institutions like education root themselves on this two-centuries-old philosophy.

However, in the last couple of years, we have been rudely awakened by trends in AI (or should I say AC), globalization and rising inequality. Many types of "Human Competence" that we took for granted have been replaced by "Artificial Competence". This trend is accelerating.

Any problem that both humans and machines can perform will be taken over by machines. Hence, going forward, I'm going to use the term "Human Competence" to refer to (not "the set of all problems that humans can solve", but) "the set of all problems that machines cannot solve, but humans can".

![Image](https://cdn-images-1.medium.com/max/800/1*4VGmr43Gj_wnfCFDVSWcFQ.png)

## On the Future

Many describe a future where most humans will be out of work, a minority that owns all capital will rule the world. It is unclear how we avoid this dystopia, without first, correctly understanding "Human Competence" and its characteristics.

This understanding consists of studying and finding answers to the following questions:

* What are the properties of Human Competence? (See https://medium.com/on-technology/on-human-competence-e5e2976427de [Update 8/15])

* In what specific situations can humans solve problems better than machines?

* How might we adapt our education systems, and other institutions and processes, to focus on nurturing Human Competence?

* How can we use technology to foster Human Competence? Or in other words, how might Artificial Competence support Human Competence?

(I hope to address these questions in a following set of articles).

#### Article 60 · August 15, 2019

# On Human Competence

### What humans can do, but machines can't

In [1], I defined Human Competence as:

>>> "the set of all problems that machines cannot solve, but humans can"

I concluded this article by asking:

>>> "What are the properties of Human Competence?"

The goal of this article is to answer this question.

## How humans think

Humans think in two ways: "Thinking" and "Contemplating".

Thinking is a very conscious act. It involves solving some specific problem, that is well defined. For example, "What route should I take to the office this morning?". Thinking consists of following a set of deductions, or inductions that lead to the solution. It is easy to measure progress on solving the problem, on how optimal the answer is, and the extent of the error. While thinking involves facts, opinions and memories, the process of thinking reduces these to something simple. You might know all the roads in Colombo, but finding your route to the office involves narrowing this down to a much smaller subset.

Contemplation, on the other hand, is a mostly sub-conscious process, in that we aren't aware of what's going on. Contemplation also solves problems that are not defined, or that we are not consciously trying to solve. Contemplation often leads to creative composition. For example, poets often describe the process of writing the poem as "the poem writing the poem", while the poet is an external observer. There are few parameters or constraints that defined "rightness", and Optimality and error are ambigous.

## How machines think (and why machines can't contemplate)

Computers have two fundamental abilities:

* The ability to input, store, and output data.

* The ability to process stored data, according to a set of instructions, which are usually also encoded in stored data

While the results of instructions might be complex and emergent, they are still deterministic and human-defined. Hence, computers "solve problems" in a similar way to how people, "think". They follow a path until they get to a solution, or near enough to it.

There are two reasons why machines cannot contemplate:

* Humans don't precisely know what contemplation is. We know that it is probably some complex interactions within our brains, and that interaction involves the complex storage system that is the brain. But our knowledge of this is weak, and we have little sense of how to replicate this within computers.

* Within our brains we perform this complex form of reflection, which we call "consciousness". Consciousness leads to other concepts like "needs", "meaning", "value" and "good". These values drive how humans behave, ultimately control the world, and determine how we contemplate. How the consciousness of individual humans impacts the world is asymmetric; powerful humans have more influence than weaker ones. Hence, in a world where computers don't have social, economic, or political power, they cannot influence values, and thus, contemplation.

In summary, there is a possibility that machines will be able to mimic and surpass the human brains storage mechanisms and the ability to contemplate. But as long as machines don't influence values, they have no direction for contemplation.

## How humans act

Humans don't only think; we also act. And there are various problems that humans solve by "acting" which machines cannot solve.

I'm going to gloss-over this class of problems because they seem more obvious. For me, acts that require "human contact" or the "human touch" (from nursing to personal training)

## What next

Hence, "the set of all problems that machines cannot solve, but humans can" or Human Competence, consists of:

* Contemplative thought

* Acts requiring the human touch

![Image](https://cdn-images-1.medium.com/max/800/1*b1-kVezYXO2fD-DVtbG0cg.png)

In future articles, I hope to address,

* In what specific situations can humans solve problems better than machines?"

* How might we adapt our education systems, and other institutions and processes, to focus on nurturing Human Competence?

* How can we use technology to foster Human Competence? Or in other words, how might Artificial Competence support Human Competence?

## References

[1] On Artificial Intelligence, And why we need to study Human Competence, Author (https://medium.com/on-technology/on-artificial-intelligence-124cffaf512d)

#### Article 61 · August 19, 2019

# On Auto-Complete

### Moving away from automating to informating

There was a meme going around Twitter, where you were supposed to type "I...", and then construct an interesting sentence using the words suggested by auto-complete (AC).

Unfortunately, I found it practically impossible to create anything close to an exciting sentence. The suggestions were too mundane and utilitarian.

>>> "setting up a meeting at work", "picking up the children", "going out for dinner".

The tips were based on a minimal vocabulary and seemed to circle back to suggest the same thing again and again.

>>> "I will have dinner, then pick up the children, and then have dinner".

## How AC works

AC is trying to predict what the human wants to type next. It makes this prediction using an elaborate model consisting of millions of examples of previous conversations, and various rules about grammar, spelling and vocabulary. The output of this process is a small number of suggestions (e.g. three). If the human selects one of the suggestions, then AC has succeeded. If the human types something else, or worse, if the human types nothing, AC has failed.

Hence, AC ends-up finding words that "the human is likely to choose". It is also biased towards the most common scenarios. The result is that AC's suggestions tend to be mundane and utilitarian.

## The Problem: The vicious automation cycle

Automation is a process where machines replace human productivity. In information technology systems, automation replaces a human's interaction with data and takes over the resultant decision making. For example, in the case of AC, the machine decides what words to type next, by analyzing data related to conversations. In an automation free world, the human would rely on their experience and education.

We can represent this diagrammatically as follows:

![Image](https://cdn-images-1.medium.com/max/800/1*3PEbuPig_x1JF0E3vKVdZg.png)

For example, "data" is made up of the "millions of examples of previous conversations". The "machine" is the AC system. The "human" is the human using AC. The resulting data is the choice that the human user ends-up making.

Automation is a "reductionist" process that creates no new information. Machines, unlike humans, cannot create. They can do an excellent job of "mimicking" the human creative process. For example, a sophisticated machine could produce a piece of music that sounds like Chopin, or re-render a photograph in the style of Picasso. However, they cannot create a "new work of art in the style of a new artist". Hence, automation innately results in "reducing" data. In our AC system, the set of words used gradually converges to a small set of the most common, and utilitarian words.

In this "Automation Cycle," the machine effectively controls what the human types. The human adapts to the machine, and types increasingly dumber and dumber text. The data which ingests this new "dumbed-down" data, makes predictions which are themselves dumber and dumber. A vicious cycle ensues, wherein each round information is lost.

## The Solution: The informate-tion cycle

How might we break this vicious cycle?

There are two problems with the "Automation Cycle":

* The machine prevents the human from interacting with data

* Instead, the machine controls the human's actions, thus stifling the human's creativity

How might these problems be solved?

One problem with a phone with its small keyboard is that it is difficult for the human to type. AC is a reasonable solution to this problem. However, rather than inspire the human to interact with a vocabulary of hundreds of thousands of words, AC restricts the human to three. Solving this problem involves building a more vibrant interface. One option might be to support richer forms of input, like speech or writing. VR and AR imply other solutions, where the human is not constrained by a small keyboard. Even with a small number of options, the machine might align itself with human creativity by optimizing beyond just "getting the human to type something". For example, it could try and maximize the human's vocabulary, by suggesting a word which it has never suggested before.

My "solutions" are incomplete and premature. But my goal was to describe a principle, not its final instantiation.

![Image](https://cdn-images-1.medium.com/max/800/1*7dcOawf2DmbTZ_rHuzXhCg.png)

In this new design, the machine that controls the human is replaced by a machine that pre-processes data so that the human might consume it more easily. The new data created by the human is them post-processed before storage. Unlike machines, humans are creative and are capable of producing novel information. Hence, in this new cycle, there is a further increase in data, information and knowledge.

Shoshana Zuboff [1] coined the term "informate" to describe this alternative to automation, where machines augment human productivity, without replacing it. Thus, we replace a reductionist automation cycle, with an expansionist informate-tion cycle.

## Next Steps

This article was meant, at best, to be an introduction to the automation/informate-tion duality. In future articles, I hope to address:

* Where else might informate-tion replace automation?

* How can we maximize incentives for building informate friendly systems?

* How can technology enhance human competence?

### References

[1] https://en.wikipedia.org/wiki/Shoshana_Zuboff

#### Article 62 · August 19, 2019

# On Justice

### And yearning for it.

![Image](https://cdn-images-1.medium.com/max/800/1*duWhvSknH5OELQP6qxBwKA.jpeg)

What is justice?

The OED defines "just" as "Based on or behaving according to what is morally right and fair". Its essence is "right". We all have some notion of "what is right", and justice is about "right being done".

From where does our "sense of justice" or "sense of right" come?

Some believe that the universe is innately just, possibly facilitated by a "just God". And that our sense of justice and right comes from this divine fount. However, even many who don't hold this theological view, do have a strong sense of "justice" or "right".

So, from where does this come?

The existence of "right" implies that there is also "wrong". A belief in either implies a belief that there is a "right way for things to happen" and a "wrong way for things to happen", and that the "right way" is the "right" way.

Splitting the "way things happen" into "right" and "wrong" implies an opinion (on what is right and wrong), which conditions our view of the world.

Hence, a "yearning" or "clinging" for justice, implies a yearning for this opinion to be true, again and again. Or in other words, to make this opinion permanent.

But, what if you also believe that nothing is permanent or constant?

Then, is there any point in believing in , or yearning for justice?

When we feel "wronged" by an injustice, what is actually "wrong"? The "wrongness" of the wrong? Or our "belief" in the wrongness of the wrong? For, if we didn't believe it wrong, it wouldn't be wrong and an injustice, would it?

Conversely, if we don't believe in "wrong", then can we ever suffer injustice?

#### Article 63 · August 20, 2019

# The Creativity Conjecture

### On Hard-Boiled Eggs and Piano Miniatures

All Machines, including computers, even the most sophisticated super-computers, follow instructions; instructions designed and written by humans. Sometimes the connection between these instructions, and the machine's final behaviour or output might not be obvious, but a precise and deterministic relationship exists, nonetheless. Hence, in summary, machines follow instructions and end-up doing productive things.

Humans are also productive, sometimes as a result of following instructions. For example, this morning, I "produced" two hard-boiled eggs by following the precise instructions of "boiling two eggs for 7 minutes". Obviously, humans are also capable of following more elaborate instructions and being more productive.

Whenever a human is productive by following instructions, it is almost always possible to design a machine that does the same thing, often faster, and more cheaply. I'm sure a hard-boiled egg making machine exists, though I don't own one.

But now for something completely different.

Last evening, I wrote a short piece of music for the piano. I didn't follow any instructions to write it. I happened to be doodling on the keys, and a piece of music, just "came to me". I could record the piece and share it on iTunes. Alternatively, I could transcribe it into sheet music, and possibly sell it. Either way, in this example also, I (a human) have been productive. But, this time, I didn't follow instructions.

As with boiling eggs, humans are also capable of being productive, without following instructions, and in ways where it is impossible to provide instructions. While I could, in theory, design a machine that boils eggs, I could not design one that would produce genuinely creative music.

Now you might say,

>>> "But wait. There are machines that compose music. You once designed one [1]"

Yes — that's true. And many of these machines pass "intelligence" tests like the Turing Test [2]. So, what exactly do I mean by "I could not design one [a machine] that would produce genuinely creative music."?

I am less interested in the result (what) and more interested in the process (how). Hence, I actually mean, "I could not design one [a machine] that would produce genuinely creative music, the way humans do".

You might retort:

>>> "But who cares how the machine does it, as long as what it produces is useful and possibly better than what humans produce?"

The key phrase here is "possibly better".

I conjecture that there is a class of human activity (let's call it the class of "creative activity") with the following properties:

* It is not known how to reduce the activity into a set of instructions

* The result of this activity is superior to those produced by machines

This conjecture is what I mean by the "Creativity Conjecture".

Hard-boiled egg anyone?

![Image](https://cdn-images-1.medium.com/max/800/1*-S69v7p2I5dzbkW7W8GFGw.png)

### References

[1] https://www-cs.stanford.edu/people/nuwans/docs/AMCTIES.pdf

[2] https://en.wikipedia.org/wiki/Turing_test

#### Article 64 · August 21, 2019

# On Traffic Shortcuts

### And why they should be abolished

Colombo Traffic is bad at the best of times. It is worse during the morning and evening office rush-hour. It is, perhaps, worst at the entrances and exits to the city centre.

Increasingly, many of the drivers in Colombo use Google Maps and other forms of navigation, a trend accented by Uber, PickMe and other taxi services. GPS powered navigation tends to provide some ingenious driving tips. A common suggestion is the "shortcut" that bypasses a main road.

But do shortcuts actually work?

### Freeways are good

Something good about a main road that is not crisscrossed by shortcuts is that it is effectively a"freeway". By "freeway", I mean that its two flows of traffic in opposite directions, don't interfere with each other.

![Image](https://cdn-images-1.medium.com/max/800/1*WGqiLlNVjoR4OvNJodPuCw.png)

### Collision Points are bad

On the other hand, the moment there is a shortcut bypassing a segment of a main road, "collision points" occur. By "collision points" I mean a point of the road where there are two or more flows of traffic coming in, from different directions. Unless some flows of traffic stop for the others, there can be collisions. We solve this collision problem by posting traffic lights, traffic police officers or roundabouts to control the traffic flow. However, these collision prevention tactics incur some overhead and slow down the traffic overall.

![Image](https://cdn-images-1.medium.com/max/800/1*mk1kYYs-PxshIZpNfHqpmw.png)

During rush-hour, most of the traffic is in either one or the other direction; Into the city in the morning, and out of the city in the evening. Hence, in many places, shortcut roads have been made "oneway".

![Image](https://cdn-images-1.medium.com/max/800/1*hl4BeruzDBRS2eTHtnm1SQ.png)

Unfortunately, this doesn't solve the problem of collision points either, as you see from the diagram. The number of collision points is reduced from 5 to 3, but they still exist. More importantly, the collision points also become bottlenecks.

### Bottlenecks are worse

Suppose during evening rush hour, M vehicles were trying to get out of the city every minute, and N were trying to get in. Also suppose Mp vehicles used the shortcut, while M(1 — p) remained on the main road. At two of the collision points, we have Mp + N vehicles trying to get passed per minute, when without the shortcut we only had N. Hence, the shortcut actually slows down the traffic.

## What next?

At the best of times, traffic shortcuts have no benefit, and at the worst times significantly slow down traffic. Hence, we should abolish shortcuts. But how?

On some shortcut roads, one entrance is blocked disabling its ability to bypass the main road. However, this is highly disruptive, particularly to the residents on the road, and is usually restricted to short, private roads.

An alternative might be for navigation apps to be smarter, and factor in the well-being of the traffic ecosystem as a whole, instead of narrowly optimizing for their clients' benefit. In a world with increasing automated navigation, these problems converge anyway.

#### Article 65 · August 22, 2019

# On Sinhala Pronunciation

### And how I've been mispronouncing my name all my life

### English sucks, Sinhala is beautiful

The English alphabet is a mess. The letters seem to be in no particular order, there are no patterns, and the only way to learn it is to memorize it (all 26 letters) from A to Z.

English pronunciation is even worse. While most languages have some deterministic relationship between letters and sounds of words, in English "bough", "cough", and "dough" have completely different endings. Hence, again, the only way to learn spelling is to memorize.

The Sinhala Alphabet is phonetic and far better organized. It first lists all the vowels, followed by the consonants, both of which are in order of pronunciation.

Consonants are ordered based on the location of sound production, starting with the soft palette on the roof of the mouth (e.g. ක, "ka" as in "kill"), through the hard palate (ච, "ca" as in "chill"), the alveolar ridge (ට, "ṭa" as in "till"), the teeth (ත, "ta" as in "thick"), before finally ending with the lips (ප, "pa" as in "pill")

![Image](https://cdn-images-1.medium.com/max/800/1*-217e_SMIjnKPPT65YOjdQ.png)

### To Err is to mispronounce

Given that Sinhala is phonetic, you might think that spelling is easy. But there are a few exceptions that arise from speakers (like myself) not knowing how to pronounce certain characters correctly.

The "na" (as in noon) sound is a good example. There are two "na" sounds in Sinhala:

* ණ — sounded from the alveolar ridge, like ට ("till")

* න — sounded from the teeth, like ත ("thick")

Many people (like myself) use the ණ (alveolar ridge, like "till") pronunciation for the "na" sound, even when spelling intends න (teeth, like "thick").

Another standard error is to mix the two "la" sounds: ල and ළ.

### A name by any other pronunciation would mean as meaningful?

My name spelt "Nuwan" in English, corresponds to two different words, with different spelling, meanings and pronunciation in Sinhala: "නුවන්" and "නුවණ්". The former (which is my name) means "eyes"; the latter means "wisdom".

Throughout my life, I have been pronouncing my name as "ණුවණ්", which is neither of the above, has no meaning in Sinhala, and never occurs within the many petabytes that make up the internet.

![Image](https://cdn-images-1.medium.com/max/800/1*5WC9msHpOv1UMjCNJLTR3g.png)

Time for a change?

### Reference

* https://www.trilingualdictionary.lk

* https://en.wikipedia.org/wiki/Place_of_articulation

* https://en.wikipedia.org/wiki/Sinhala_script

#### Article 66 · August 23, 2019

# Beyond Thinking

### Contemplations overlooking the sea

>>> Me: What is the opposite of "Thinking"?

>>> You: "Not Thinking"?

>>> Me: That's like saying, "the opposite of doing a good deed is doing no deed at all" or "the opposite of growing tall is staying the same size" or "the opposite of multiplying a number by 2, is not multiplying the number by 2".

>>> You: Ok. What about "Thinking illogically, irrationally, or negative thoughts"?

>>> Me: That's still not quite what I was looking for.

>>> You: Why?

>>> Me: "Thinking bad thoughts" is still thinking; like saying, "the opposite of doing a good deed is doing a bad deed" or "the opposite of growing tall is growing short" or "the opposite of multiplying a number by 2, is dividing the number by 2".

>>> You: Ok. If the opposite of multiplying is neither not multiplying nor dividing, what particular opposite are you looking for?

## A sea that is oddly still

To answer your question, we would need to first define "Thinking". What exactly happens when we are thinking?

To find out, we could try the following experiment: a) Let's watch out for the next thought that comes to our mind; b) Let's try and describe, not the thought, but the process of thinking. In my case this is what happened.

For a moment, I happened to look up from my laptop, out of the window, and I see the sea. I think,

>>> For a rainy day, the sea is oddly still, isn't it?

Several things happened. First, I saw the sea. Second, I also had some notion of "the day". Then, I labelled the sea as "oddly still"after already naming "the day" as "rainy". "Still" and "rainy" are words that I already know, and I can easily associate with other examples of "rainy" and "still".

Let's watch out for another example. I happen to notice the time on the clock. Just passed 5pm. I think,

>>> I should make tea.

And that's what I end-up doing.

## Thoughts over a cuppa

Within both these instances of "thinking", I've associated "things that I know" with "other things that I know". For example,

* "Sea" and "still"

* "Day" and "rainy"

* "Tea" and "5pm"

By "associating" I've effectively reduced "something that I can't explain" to something that I can.

For example, a moment after I saw the sea in the evening light, it was something unexplained and unexplainable. But the moment I labelled it as "still", I reduced it to something I know and can explain. And more importantly, something about which I don't need to think any more.

The sea is still. That's all there is to it.

## Tiny ripples and strange shadows

But this "explanation" of the sea is oddly unsatisfying. For a start, I can stare at the sea, fascinated, almost endlessly, even when it is "still". Surely, there is more to it than "still"? And of course, there is.

I look out of the window again. This time, I'm determined not to think. I manage a couple of minutes, completely void of thought. And then I reflect on what happened.

>>> I see many things. The sea is not quite still. There are tiny ripples. And there are silver lines between these ripples. The clouds place strange shadows on the sea. I not only see the sea, but can hear the sea, and feel the sea's breeze on my face. And if I concentrate, even though the sea is several miles away, I can, faintly, smell the sea.

I could go on and on, but if I've proved one thing, it is this: There's a lot more to the sea than "being still". So what was I thinking?

## The sea that is chosen to see

But I'm less interested in what I was thinking. This "contemplation" of the sea led to far more interesting thoughts about the sea, despite, perhaps because, of the fact that I was not thinking. I was taking in all the unexplainable signals about the concrete sea, without seeking abstract explanations. Hence, there was no "reduction" from a concrete unexplainable to an abstract explainable.

But would it be possible to take this process even further?

Consider what happened when I "saw" the sea. Various particles reflected off the surface of the water, and my eye detected some of these. Note, the particles detected by my eye satisfied two conditions:

* They were reflected off the sea, and hence a function of the sea; and

* They were detected by my eye, and thus, a function of my eye

Assuming the sea is "real" and "absolute", what if my eye was doing what my "thinking" was doing? Suppose it "chose" what to see, to simplify and explain the sea?

## A conclusion of a thousand words

But now I'm straying into rambling speculation.

>>> (Exasperated) You: If the opposite of multiplying is neither not multiplying nor dividing, what is?

>>> Me (Vague): It's subtracting the number from itself.

Let me end with a picture.

![Image](https://cdn-images-1.medium.com/max/800/1*ZYcFXRncl5v19QoNGZ6M1Q.png)

You can perhaps think about this picture, or even better contemplate, or even better "realize" (whatever that means).

Perhaps by the sea, sipping a cup of tea.

#### Article 67 · August 23, 2019

# On why we sense

### Coincidence, Correlation, and Causation

## On Breaking Glasses

There is a glass of water on the table in front of me.

Scenario 1: Suppose I knock it over. It would then fall to the floor, and smash to pieces. I would have "caused" the glass to break. This is "causation".

Scenario 2: Now, suppose, whenever you walk into a room and find me in that room, you also happen to find a broken glass on the ground. You might get suspicious. It might look like I cause glasses to break. But you don't really know that I caused the glass to break. It's just that "Nuwan is in the room" and "There is a broken glass on the floor" are "correlated".

Actually, there might be no "statistically significant evidence" for a correlation even. In which case, it would merely be a "coincidence".

Scenario 3: Now, suppose that I am a janitor. And whenever a glass breaks, it is my job to do the cleaning. And so, you turn up in a room, there is a broken glass, and I also have turned-up to clean up the mess. This is also "causation" — but in this case, the "broken glass" caused "me" (to be in the room).

## Conditions for causation

When could we say that A caused B? Several, conditions would need to hold.

* Condition 1: Both A and B must have happened. For example, "Nuwan happens to be in the room", and "The breaking of the glass has happened".

* Condition 2: A must have happened before B. For example, "Nuwan happened to be in the room, before the glass broke"

* Condition 3: There must be some process by which A caused B. For example, "Nuwan caused the glass to break by knocking it over, and making it fall to the floor".

If any of these conditions don't hold, then there is no "causation". For example, in Scenario 1, all the conditions are true; in Scenario 2 and Scenario 3, only Condition 1 is true.

## Sensing the universe

By "sensing the universe", I mean our body's ability to see, hear, feel, smell and taste.

Why do we see? What do we have eyes?

An evolutionary biologist would say the "cause" for our eyes was a "need to see". Humans have very complex eyesight. Some animals, like eagles, have even better eyesight. Trees have basic "sight", being able to distinguish light from darkness — but little else. Many microbial organisms are utterly insensitive to light, and hence, have no eyesight.

Hence, over millions of years, various organisms acquired varying degrees of sight depending on need and the random iterations of evolutions. In our "Conditions for causation" scheme,

* Condition 1: Bodies need to see, and there are examples of organisms with bodies with eyes that see (like humans)

* Condition 2: There was a "need to see by bodies" before "eyes evolved".

* Condition 3: Evolution was the process by which eyes evolved, where, through many generations, organisms with bodies with better eyes survived and reproduced, while others died out.

In summary, we have senses, because "Our senses helped our bodies survive".

## A look in the mirror

But what about the opposite. While it is true that "our senses helped our bodies survive", it is also true that "Our bodies helped our senses survive".

For example, there won't be "Homo Sapiens eyes" today, if Homo Sapiens died out thousands of years ago, and there were no Homo Sapiens bodies. The same applies for all types of "eyes", even the rudimentary "eyes" that trees have.

But then, who is the master and who is the slave? Do our senses serve our bodies, or do our bodies serve our senses? As opposed to saying "The need for seeing, caused our bodies to evolve eyes", should we instead say, "The need for seeing, caused our eyes to evolve bodies"?

What does that even mean? If the latter statement is true, our "Conditions for Causality" would look like:

* Condition 1: Eyes need to see, and there are examples of eyes with bodies with organisms that see (like my eyes, and your eyes)

* Condition 2: There was a "need to see by eyes" before "bodies evolved".

* Condition 3: X was the process by which bodies evolved, where, through many iterations, eyes with better bodies with better organisms persisted, while others didn't.

I can't prove any of these conditions. Nor can I explain what "an eye without a body" is, or what the mysterious "X" is.

But, more interestingly, nor can I disprove the "Conditions of Causality".

Did I break any glass? Perhaps the mirror?

![Image](https://cdn-images-1.medium.com/max/800/1*TOa7YFUlJgnvsnXUnH89MA.png)

#### Article 68 · August 25, 2019

# Number Sequences

### On Uncertainty, Prediction Error, and Lost Reputation

## Prediction Error and Loss of Reputation

Consider the following sequence:

1, 2, 3,...

Can you predict the next number in the sequence?

The correct answer is "6".

If you, like most people, predicted "4", you might be disappointed. You suffered a "prediction error". You might have thought you had a "reputation for solving mathematical problems", and that reputation just suffered a setback.

The next ten numbers in the sequence are: 6, 5, 5, 1, 6, 4, 2, 4, 1, 6, ...

## Uncertainty

If you think you can try and "solve" this sequence, don't bother. Each number was generated randomly by picking a number between 1 and 6. It was purely chance (a one-in-216 chance, to be precise) that I got 1, 2, 3 at the beginning.

Before you get mad at me for challenging you to bogus puzzles, please consider the next game. You can reclaim your reputation.

## Reputation reclaimed

Now, suppose we play the same game (where you try and guess the next number in the sequence). Suppose we continue to use the same "number generation strategy", where I pick a number at random from 1, 2, 3, 4, 5, 6.

But suppose we add a new rule: You can choose to ignore specific numbers that you have chosen beforehand.

For example, if you choose to ignore 4, 5, and 6, our original sequence becomes:

1, 2, 3, 1, 2, 1

If you choose to ignore, 1, 4 , 5 and 6, it becomes:

2, 3, 2

You can choose to ignore all 6 numbers or none at all or anything in between.

Now, what is the optimal strategy to play this game? What set of numbers do you choose to ignore? What number do you guess?

## Solution

Of course, the solution to this puzzle is simple and trivial. Your "ignore set" consists of any five numbers, say "1, 2, 3, 4 and 5" and you predict the remaining number, say "6".

For example, our sequence is

6, 6, 6

And of course, you get 3 out of 3 predictions correct.

## Philosophical Conclusion

Do you see the world for what it is? Or do you choose to see the world such that your reputation (for winning puzzles and life in general) is maximized?

If so, what is your ignore set, and what is your prediction?

![Image](https://cdn-images-1.medium.com/max/800/1*MLFZ8JW_mKkSoHJWK0BZxQ.jpeg)

#### Article 69 · August 27, 2019

# Chained Melody

On the anatomy of tunes and ideas

## George Wilfred's famous melody

Think of any melody — say, the melody of the Sri Lankan National Anthem:

![Image](https://cdn-images-1.medium.com/max/800/1*OvxzakVVrnoouYTDjDOvMw.gif)

Suppose you sing, play or hum it from that starting G. At what point does it become recognizable as a particular melody?

A single G means little. Add a second note (another G), and still we have two isolated Gs. Add a third, an it is still G-G-F —i.e. not much. It is probably with the D-F-E♭phrase ending that Egodahage George Wilfred Alwis Samarakoon (a.k.a. Ananda Samarakoon)'s famous melody becomes finally recognisable.

## No note is an island

Hence, a single note is not a melody. Collections of notes become motivs which then gradually emerge into melodies. Melodies emerge into subjects, and subjects emerge into whole movements of music. Movements emerge into "pieces" of music.

With each step, music becomes more complex, and endures longer in time.

All of this requires time and memory. If one forgets how a melody began, then it ceases to be a melody. For example, "Sri Lanka Matha" would not be recognizable if we forgot the G-G-F by the time we got to the D-F-E♭.

This "need for memory" also applies in the opposite direction.

Consider the G at the beginning of "Sri Lanka Matha". In concert pitch, this G has a frequency of about 392Hz. Depending how exactly the sound is produced, it will take some wave form.

For example, this is what the wave would look like if produced by a tuning fork (Sine wave), a violin and a piano:

![Image](https://cdn-images-1.medium.com/max/800/1*wXqt6K-KUpU5G7eyJlYYsA.png)

At a given moment in time, "sound" is just the position of particles of air. A particular sound only emerges when these particles move in the shape of a wave. This wave causes our ear-drums to move in concert, which is then sensed by our brains. Hence, just as no melody exists with an isolated note, no sound exists at an isolated point in time.

Hence by nature, all melodies are "chained melodies". They only acquire meaning from their context. Without this context they are meaningless. There is no such thing as an "absolute melody". All melodies are "relative" to all that is around it.

## The Cosmic Dance

But wouldn't this apply to any piece of information?

Just as a melody is made up of notes, a painting is made up of color. And just as a sound has no meaning at moment in time, nor does colour, which is also a vibrating electro-magmetic wave of a particular frequency.

And what about more complex pieces of information? Like ideas, values, and ethics? Are they any more absolute than the isolated G at the beginning of our national anthem?

#### Article 70 · August 28, 2019

# On Democracy

### From first principles

Sri Lanka is bracing itself for yet another presidential election. Party faithfuls are getting behind one or the other party. Others are contemplating backing a third, perhaps even fourth horse. As usual, "democracy", "the survival of democracy', and "the threats to the survival of democracy" are hot topics, at least amongst the (self proclaimed) englightened classes.

Hence, I thought it a good time to reflect on democracy in general, and Sri Lankan democracy in particular.

## Equal Power

Democracy is (for me) a system of government where political power is shared equally amongst the citizen. Or a system of government where all citizens have equal power.

To better understand anything, it is usually useful to compare it with its alternatives. So what are some alternatives to democracy

* Autocracy, (power in the hands of) one person

* Meritocracy, people with merit, skill, or academic ability (very similar to Technocracy)

* Monarchy, a monarch

* Oligarchy, a small number of people, usually rich

* Plutocracy, the wealthy

* Theocracy, religious leaders

* Representative Democracy, a few representatives chosen by the people

All these alternatives have two things in common:

* All concentrate power in the hands of a few

* They all have some justifiable rationale for this "concentration process" (at least to their supporters). For example, supporters of Meritocracy might say that PhDs in Engineering, Bio-Chemistry, or Economics make better leaders. Supporters of representative democracy often claim that most people don't know how to govern a country, and hence must leave it to the experts. Supporters of Monarchy claim that the monarch has a divine right to govern (whatever that means).

The problem will all of these alternatives is that these "justifiable rationales" rarely hold up. For example, meritocrats who might be very smart at somethings end up being very stupid at most other things; "Representatives" often end up being incompetent, corrupt or worse. Hence, there is no effective way to concentrate power in the hands of a few.

The only alternative to these alternatives is democracy in its purest form: Equal power to all citizens. We solve the "concentration" problem by picking a system that has no concentration.

Hence, democracy has one and only one justification: it is better than all other forms of government.

## How to promote democracy in Sri Lanka

There is a very easy way to measure if Democracy is declining: if there is more inequality of power, then there is less democracy (by definition).

Conversely, the way to make a country more democratic, is to increase equity of power. This can be done in a combination of ways:

* Equity. Political power goes hand in hand with economic power. Many "democracies" like Sri Lanka are, to a large extent, controlled by small elites of wealthy, influential people. Law and Order, and Institutions are, to a large extent, subservient to these elites. The most effective way to create an equitable society is to make institutions, and law and order, strong, and this elite weak.

* Enlightenment. Democracy works best when the population is intelecually rich. Sri Lanka, for example, is still somewhat backward in terms of intellectual freedom. Philosophy and thought are still very much grounded in religious texts and feudal or colonial identities. Technology and the internet have mostly made things worse. We need to find ways of turning this around, including finding more enlightening uses of technology.

* Identity. A lone man on an island has no use for a system of government, or democracy. Conversely, democracy only makes sense, if the people of a country decide that there is some value in prospering as a country. Sri Lanka has no national identity. We have various racial, religious, caste, and class identities, but these always trump the national identity. Hence, everyone is more Sinhala, Buddhist, Govigama, "English-Speaking", "Royalist" or "Colombo Educated" than they are Sri Lankan. Our country needs a strong identity and, perhaps, some unifying story.

* Development. Economic, social and political development which promotes Equity, Enlightenment and Identity is a sort of "blanket" strategy that will help many of the components of democracy. While Sri Lanka has achieved significant development in the last couple of decades, the job is by no means complete. We should focus on continued development, particularly in terms of technology, product development and intellectual property.

Hence, for me, this is how we can promote democracy: ultimately by promoting power equity.

## Concluding Thoughts

Voting in presidential elections is a very small part of democracy. If we vote in such away that our (the peoples) political power is given away and futher concentrated in the hands of a few, then that is not democracy. On the other hand, if some short-term concentration will result in long-term equity, then that is still progress to some extent. And yes, this is a paradox. But complex topics are full of paradoxes.

Perhaps that is the most important takeaway: a system of government is complex, and so is the business of elections, and democracy in general.

If you think it is simple, then you've probably got it wrong.

![Image](https://cdn-images-1.medium.com/max/800/1*5dzZ4mW_AxenjgKcqjcpYw.png)

#### Article 71 · August 28, 2019

# On Time Travel

### More adventures with coins

## Time

The relationship between time and information is interesting. As time "increases" so does information. In other words, there is more information in the present, than there was in the past.

For example, suppose we toss a coin. After the coin lands heads or tails, there is one additional bit of information (namely whether the coin landed heads or tails) in the universe. Before the coin toss, this information didn't exist.

To be clear, a coin toss results in a lot more information than a single bit. For example, if the coin landed on the ground, there is its precise location. There is the collective memory of the people who saw the coin toss. There might be some additional record of the coin toss; someone might have written down the outcome, or recorded it on video. In practice, the coin toss probably resulted in exa-bytes of data.

But let's ignore these details for now. My point is: information increases with time, or alternatively, time increases with information.

## Stopping Time

Now suppose that the coin was indeed tossed, but there was no record of it. Suppose, no one remembered the outcome of the toss, nor was it recorded on video, and nor did anyone write down the outcome.

Now, if there is no record of the outcome of the coin toss, can we say that information has been added to the universe?

And if information was not added to the universe, did time pass? Given that the present has the same information as the past?

## Reversing Time

Now suppose that the coin was tossed, and its outcome (say, heads) was recorded on multiple media: paper, video, and the collective memories of several bystanders.

However, suppose that soon after that the following happened: the paper with the outcome was burned; the video was dismiised as a fake, probably doctored by the Russians, Hillary Clinton, or Wile E. Coyote; and all the bystanders got amnesia, probably as a result of attending a 5 Seconds of Summer concert.

Now, the past (soon after the coin toss) clearly contained that bit of information about the outcome of the coin-toss. But the present (post paper burning, Russian fakes, and 5 Seconds of Summer), does not contain the said bit. Hence, the present has less information than the past. Hence, did we travel back in time?

## Concluding Perspective

We say that after tossing the coin there was more information in the universe. But is this actually true?

I don't know how much information exists in all that is the universe: probably exa-exa-exa-bytes, give or take. Was it that the coin-toss increased this information, or that we decided to arbitrarily label some set of information as new information?

Was it that we decided that some set of information represents "no outcome", and a different set (with the same amount of information) represents "some outcome"?

And would this apply to all information? Everything that we know? Mere labels of things we choose to know and choose not to know?

![Image](https://cdn-images-1.medium.com/max/800/1*YbRT1Hh1CLbgrHEBebRo-g.jpeg)

#### Article 72 · August 29, 2019

# D-E-S-I-G-N Tests

### 6 UI Design Tests from a Non-Designer

I'm a computer scientist, not a UI Designer. I have no qualifications, or proper experience in UI Design. However, in the last couple of months, I've had to do quite a lot of "UI Design" out of necessity; partly because good UI Designers are hard to find and hire, and partly because I was part of "early-stage developments" that could not afford the said experts.

In this article, I list some insights I've learnt by "trying to be a designer". It is structured as "6 tests" that could be used to verify if a UI Design is a good (enough) design.

Disclaimer: The professional designers among you (some my friends and former colleagues), might laugh or cry at the rest of this article, as it is not really grounded in formal or academic design principles. Hence, if this article is not useful as a pattern to follow, it will, at least, be useful as an anti-pattern not to follow.

### Drawing Test

Good Designs are almost always simple, and memorable.

When I test the design of a new screen for the first time with a new customer, I ask them if they can take a blank piece of paper and draw what they saw from memory. They might not remember 100% of all the details, but if they get 60–80% right, then I know that the design is simple enough, and more importantly memorable.

### Engagement Test

While some UI components are intended to be "read", for a product to be meaningful, we need users to "do things" or "act". Hence, the best designs motivate the user to do something. Crude "engagement tactics" coerce users to click buttons or do other mechanical things. True engagement, on the other hand, inspires, and motivates users to get the best value out of the product.

When a user interacts with my product for the first time, I see how long it takes for them to "do something" meaningful, ideally without me having to tell them anything.

### Science Test

Most skills, including design, are a mix of art and science.

The art of design is about producing something novel and creative. The "science" of design is all the data we have about how people use a product, how we want a user to use a product, and the wealth of theoretical knowledge about colour, space, and form. Art and Science must compliment. For example, if the "science" says that the most productive action that can happen on a page is X, then the majority of the design real-estate should focus on enabling and encouraging this action.

The "test" consists of verifying if the science and the art are in sync.

### IKEA Test

A test that IKEA uses to test its furniture products is to ask volunteers to try and assemble furniture without the instruction manual. Similarly, how to use a web product should be intuitive enough so as not to need help or other explicit instructions.

When a test user sees a product for the first time, I ask them to try and do X without giving them any help on how. And if they can do this quickly, without asking questions, my design has "passed the IKEA test".

### Good-Looking Test

A good design "looks good". One problem with "looking good" is that often we know when something looks good, but don't know why; rather like a painting or a piece of music. Hence, the problem with this test is that it might not be clear what to do if the test "fails".

Either way, we must continue to iterate, until more and more users agree that the design "looks good".

### Noob Test

Finally, the Noob test is a sort of meta-test for all other tests.

All of the tests should pass if the "test user" is a total novice, inexpert, and completely new to the product.

A good design should work just as well with a novice, compared to an expert.

## So, in summary...

* Drawing

* Engagement

* Science

* IKEA

* Good-looking

* Noob

Go forth and D-E-S-I-G-N!

#### Article 73 · August 31, 2019

Fixed. Thanks!

#### Article 74 · September 2, 2019

# Breath on a Knife edge

### On minding, commenting and doing

## Blood, Bile and Sweat

Can you feel the beat of your heart as it pumps blood into all corners of your body?

If not, move your index finger to the side of your neck. You should feel a pulse.

Now, ask yourself, "What is the rate of my pulse?"

Is it 70 beats per minute? 80? 60? Does it feel too fast, or too slow? Now, suppose you imagine that it is too fast. Can you slow it down? Or conversely, can you speed it up?

We can be aware of our heart beat. This is what I mean by minding. We can also make various mental comments about it (like "My heart is beating fast"). This is what I mean by commenting.

On the other hand, it is difficult to do anything to directly control our heart rate. We could run up several flights of stairs, thus, indirectly, increase it. Or do some deep meditation, thus, indirectly, decrease it. But we can't set it at (say) exactly 57 beats per second — the way we could say the number "57".

Can you feel your liver expelling bile into your gall-bladder?

It happens all the time, but have you very felt it? Probably not. Our bodies perform thousands of actions, like pumping bile, which we are not, and often cannot be, aware of. Many things happen, without us minding.

Can you touch the tip of your nose with your thumb?

You probably can. But this is different from feeling your heart beat, because in addition to minding (that your thumb and nose touched), and possibly commenting (say, "the tip of my nose is sweaty"), you are also doing. You appear to be willing your thumb to touch the tip of your nose.

## To do or not to do

What about breathing?

When a doctor presses a stethoscope to our chest and commands us to "breathe", we breathe. We breathe deep; we breathe in, and we breathe out. Hence, like touching the end of our nose with our thumb, we can do breathing. We can also comment about our breathing, like "my breathing is painful. I might have a chest infection".

On the other hand, we can also breathe without doing. Just as our heart beats involuntarily, most of our breathing is also involuntary. We don't have to will ourselves to breathe. If we had to, we would suffocate in our sleep, or when we were absent-mindedly thinking of something else.

Hence, we can both do breathing, but also not do breathing.

## The Knife Edge

Now, is it possible to mind our breathing, while we are not doing it? Just like we mind our heart beat?

What about commenting? Can we mind our breathing without commenting about it? How?

![Image](https://cdn-images-1.medium.com/max/800/1*wbuSK2Z4wOzZr4MZyqvQ0A.png)

#### Article 75 · September 2, 2019

# On Self Genesis

### And the twelve days of creation

### The first day

In the beginning, there was nothing, and nothing was there, and there was nothing.

And God said, "Let there be change", and there was change, and all that was there changed. But since there was nothing, nothing changed. Yet all things changed.

But then I said, "I will forsake change, for I'm tired of change — I will stretch out my hand and destroy change".

But I could not destroy change.

And, so, I said, "I will ignore change".

### The second day

All things changed, but I ignored change. But I could not ignore all change.

So, while all things changed, some things did not change, and some things changed.

### The third day

I looked at what did not change, and what did change, and saw that it was good. And I said that it was good.

And I waited for the next time that it was good. And there was time. And with time the next time.

And I said that time was good, that it was a good time.

### The fourth day

I looked at what was good, and saw it had shape, but no name. So I named this shape "name". And, hence, there was name.

And I said that it was a good name.

And I named all that was good, and had shape, with names.

### The fifth day

And all the had shape and name, needed to be seen.

But there was no sight, and all was darkness.

So I said, "Let there be light". And there was light and sight. And all that was good, with shape and name, was seen in the light.

### The sixth day

But light was light, and sight was sight, and a great mountain of compassion spanned between.

So I said, let light touch sight, and sight touch light.

And light touched sight, and sight touched light.

I touched touch and said it was good.

### The seventh day

And when I touched touch, I felt the touch. And it felt good.

And so, on the seventh day, there was feeling.

And it was a good feeling.

And so feeling good, I rested on the seventh day from all my work that I had done.

### The eighth day

But as the day changed, the feeling left me. Light touched no sight. And sight touched no light.

There was no light. And only darkness. And I craved the light and the feeling.

And so, on the day after the sabbath, I craved.

### The ninth day

But there was evening and there was morning, and the day changed again, but light was not in sight, and sight was not in light.

But I craved and said, "I am this craving, and this craving is me. I am, and therefore I am I"

And so on the ninth day, I clung to my craving.

### The tenth day

On the tenth day, I rose.

And as I rose, I said, "I am I, and the only I, and the only I that is I".

And I looked at all there was, and said "I am. The I thy I. Thou shalt not have any strange Is before Me."

### The eleventh day

But on the eleveth day, that which was I, changed. And there was no I. And I died.

I said (in bad Greek), "I am dead. God has killed me".

And as I died, that which was not I, became I. And I saw I.

### The twelfth day

And I saw that I was I. And yet, I was not I.

I was I, and not I.

I had changed. And it was not good.

I looked at all the changed, and said (this time in bad German) "All this is quite unsatisfactory".

And then I said, "I will forsake change, for I'm tired of change — I will stretch out my hand and destroy change".

### Epilogue

But I could not destroy change.

And, so, I said, "I will ignore change"...

#### Article 76 · September 2, 2019

# What makes great great?

### On the essence of greatness

## A culinary example

What makes a cuisine a great cuisine?

All great cuisines have the following three characteristics.

* A great cuisine is old. It has spanned a long period of time. Countries and regions with great cuisines have long histories.

* Within that period of time, it has changed, evolved and mutated. Countries with long, but simple histories, tend to have uninteresting cuisines. On the other hand countries with long, turbulent and complicated histories, have great cuisines. This is because history has forced the cuisine to change, evolve and mutate.

* This evolution has been influenced by many factors that constantly judged, and shaped it. Truly great cuisines have been constantly questioned and measured. Often historical personalities have question the nature of food, and forced it to progress.

If you can see a parallel with biological evolution, you see correctly: Time, Mutation and Fitness.

![Image](https://cdn-images-1.medium.com/max/800/1*-rR4h46fLd2fRqC8JIoVPQ.jpeg)

## But what is great?

But you might say that great is subjective. You might argue that to a boiled potato, a boiled potato is great cuisine. But of course you're right: Before we proceed, we need to agree on what great actually means.

In all aspects of life, art and science, there is only one enduring defintion of great: Whatever that endures is great.

Now, you might protest that this definition is a tautology. Of course, it is a tautology — as true is true.

But then again, there is something enduring about enduring. A song which is still popular after 200 years, is clearly a greater song than one that has topped the chart for just 2 weeks. A book that is read for 2000 years, is clearly greater than one that has been read for just 20. This is because time tests all things, and has the habit of culling the insignificant, the meaningless and the non-great.

Hence, the essence of greatness is endurance. The greatest man is the last man laughing. The greatest joke is the last joke standing.

## Concluding resolutions

* On Books. Re-read the old books one has already read and enjoyed. The same applies to movies, songs and dishes. Read new books (movies, songs and dishes) only by accident; but be open to making accidents.

* On Bucket Lists. Replace your bucket list with a bucket cycle. A cycle of things you do over and over again.

* On Theories. Time passes slowly when events are far between. A second is a long time in physics; a decade a short time in economics. Hence, you can trust a second-old theory in physcis more than a decade-old theory in economics.

* On Houses. An old house will probably last longer than a new house. An old city, longer than a new city. An old country, longer than a new country.

* On Journalism. Judge a journalist by what they wrote last year. Judge an economist by what they wrote last decade. Judge an astrologer by what they wrote before the big bang.

* On Tourism. Before visiting a country, check if it existed a 1000 years ago. If you enjoy being disappointed, visit some place that that didn't exist 10 years ago.

* On Cuisine. If you want to try some truly good French cuisine, try a dish invented before the French Revolution (You won't find these in most Michelin starred restaurants). If you want to try some truly bad American cuisine, try a dish invented after the American Revolution, or even worse, the American Civil War.

[This article has been significantly influenced by the books and thoughts of Nassim Nicholas Taleb].

#### Article 77 · September 3, 2019

# How bad is our traffic?

### The Colombo Traffic Index

## TomTom Traffic Index (TTTI)

The Dutch navigation technology company TomTom recently published its Traffic Index, a measurement of congestion levels in 403 cities across 56 countries. TomTom describes its methodology as follows:

>>> The congestion level percentages represent the measured amount of extra travel time experienced by drivers across the entire year. We start by establishing a baseline of travel times during uncongested, free flow conditions across each road segment in each city. We then analyze travel times across the entire year (24/7) for each city — and compare this information against free flow periods to derive extra travel time.

>>> An overall congestion level of 36% means that the extra travel time is 36% more than an average trip would take during uncongested conditions. Average times are of actual taken trips, across every vehicle in the entire network, 24/7. Travel times in free-flow (uncongested) conditions are not based on speed limits but on actual trips made.

While the index included several South Asian cities, neither Colombo nor any other Sri Lankan city was on the list.

![Image](https://cdn-images-1.medium.com/max/800/1*Qr3xhCYd5SCZYNobeB6PTA.png)

So I decided to do my own version of the "Traffic Index" for Colombo.

## Colombo Traffic Index (CTI) Methodology

TomTom owns a vast amount of traffic data, which I don't have access to. Hence, rather than try and mimic the TTTI exactly, I used a simpler methodology, which makes computation simpler, but still preserves the spirit of the TTTI.

The spirit of TTTI is (for me) the definition of the index, which, in principle is the ratio of Actual Travel Time / Zero Congestion Travel Time. While preserving this definition, I made the following simplifications:

* I used Best Case Travel Time (i.e. travel time at the time of the day when travel time is least) as an approximation for Zero Congestion Travel Time

* Rather than looking at all the roads in the city, I looked at travel between a set of "important locations" on the periphery of the city to the City Centre (which I assumed to be the World Trade Center, Colombo 1). The "important locations" were Wattala, Kelaniya, Battaramulla, Nugegoda and Dehiwala, all about 30 to 60min of travel from the City Centre on average.

* Rather than looking at a whole year's worth of data, I looked at one day: An ordinary working week-day, when schools were open.

My data source was the Google Maps API. Estimates were for "driving" (not public transit or walking) and used "pessimistic" estimates.

## Case Study: Travelling from Dehiwala

For each of the important locations, I looked at travel time to and from the city centre. For example, travel time to and from Dehiwala was

![Image](https://cdn-images-1.medium.com/max/800/1*ku_hedTPqGclGkvb0fA6Zw.png)

The blue line represents travel time from Dehiwala to the City Centre, while the orange line is vice-versa. As expected, both lines have peaks 1) during the morning office rush hour, 2) when schools close in the afternoon, and 3) during the evening office rush hour.

Note: I didn't look into why the travel out of the city takes longer than travel into the city — it might be due to the assymetries in Galle Road, Duplication Road, and Marine Drive.

The Best Case Travel Time in both directions is early in the morning (~4am), and we can use this to compute the Actual Travel Time /Base Case Travel Time ratio (i.e. my Traffic Index) at various times of the day:

![Image](https://cdn-images-1.medium.com/max/800/1*WtrGHV7aH8ez5gCYGArcfw.png)

At the best case travel time (~4am) the index is zero (by definition), and is low until around 6am. By the 8am morning office traffic peak, the Traffic Index into Colombo is 153%. This means that travel time is 153% or 2.53x times more at this time. At 4am you should be able to travel from Dehiwala to Colombo Centre in about 18min. By 8am, the estimate is 44min (or 18min + 153%).

At the close of schools, and the evening office rush hour, travel out of Colombo becomes (comparatively) more congested, with the Traffic Index at 1pm 182% and 5.30pm 221%. At 4am you should be able to travel from Colombo Centre to Dehiwala in about 23min. At 1pm it would take an estimated 64min (23min + 182%); at 5.30pm an estimated 74min (23min + 221%, or 3.21x more time).

## Computing the CTI

We can aggregate the Traffic Index across the day into a single overall Traffic Index. The average travel time from and to Dehiwala were 31min and 43min respectively. The best case travel time from and to were 18min and 23 min. Hence, the average Traffic Indices are 75% and 87% respectively. We can average these two to give 81%.

We can extend this to all the "important locations", and average the TIs to give our final aggregated, global average Traffic Index, or our Colombo Traffic Index (CTI): 80%.

![Image](https://cdn-images-1.medium.com/max/800/1*XpkmYJ-7neQLM_ZAfanGug.png)

## What the CTI tells us

Important Disclaimer: Before comparing the CTI to the TTTI for other cities, note that my methodology is different, simpler, and less accurate. Hence, absolute interpretations and direct comparisons are not recommended.

On the other hand, the CTI does tells us a few things:

* The bad news: Colombo Traffic is pretty bad (though, you don't need an index to know that). In numerical terms, traffic is 80% or 1.8x slower than what it can be, on average. The worse cases are much worse.

* The good news: The "other side of the coin" of a bad traffic index is that there is huge opportunity for improvement. More road capacity (particularly at bottlenecks), and more mass transport (buses, trains, metro) can improve speed up traffic times by nearly double on average, and much more during rush hour.

* The meh news: In the meantime, the information behind the CTI can be useful for planning your travel. For example, optimizing your travel by even a few minutes can result in significant time savings.

## Appendix: Travel times from Important Locations

![Image](https://cdn-images-1.medium.com/max/800/1*dgrWaMGDRs0OC7WgsC09eg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*kQetBBIr3bNs_4xyXC1ALQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*yrOHTnEogDtAoubPK_gbDg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*mYvMx9RSyU9ck5bOvbYHRQ.png)

## Bonus Appendix: Travel time data between Colombo and other cities

Most important takeaway: While travel from Colombo to other cities is comparatively efficient, traffic on some routes (e.g. Colombo to Kandy) is almost as bad as city traffic. Just as we need improved intra-city transport, we also need improved inter-city transport.

![Image](https://cdn-images-1.medium.com/max/800/1*8Nd7BAf7eseuIve1mEikeQ.png)

#### Article 78 · September 5, 2019

# The Price is Right?

### On Shirts, Shakespeare, Da Vinci, Victor Hartmann, and Homo Economicus

I recently bought a shirt for Rs. 2,000 (~$11). Now, what does that tell you?

A few things, at least: I had Rs. 2,000 to spare. I needed the shirt. The shirt was more valuable to me than the Rs. 2,000, and anything else that I needed, and was available for Rs. 2000 or less.

It also tells you: The shirt-seller had the shirt in stock. They needed Rs. 2,000. The Rs. 2,000 was more valuable to them than the shirt.

But now for something completely stupid.

## Parenthesis: Homo Economicus

Economics "is the social science that studies the production, distribution, and consumption of goods and services" [Wikipedia]. Almost all of Classical Economics is stupid because it studies, not Homo Sapiens (as all social sciences must), but Homo Economicus.

Homo Economicus is a mythical being which is rational, innately self-interested, and makes optimal decisions, given the information it has. Homo Sapiens (like you and I), on the other hand, is irrational, not always self-interested, and often makes sub-optimal decisions.

Back to the real world.

## "A horse! A horse! My kingdom for a horse!"

The act of buying involves two acts: an act of buying and an act of selling.

"Obviously!", you might say. "You are buying a shirt, and the shirt-seller is selling it".

Yes and No. I am, indeed, buying the shirt. But I am also selling Rs. 2,000. The difference of this exchange is profit. A rational being would not exchange anything without a positive profit. In our example, I exchanged Rs. 2,000 for a shirt because the shirt was more valuable to me, relative to the money. Conversely, the Rs. 2,000 was more valuable, relative to the shirt, to the shirt seller.

Hence, profit depends on value, and what "more valuable" means.

But what does "more valuable" mean?

## "Everything connects to everything else"

In theory, one could take a microscopic view, and assign absolute value to everything — where everything has an absolute value, independent of everything else.

However, in practice, no one knowns how valuable anything is. The reason I bought the shirt was because it was relatively more valuable (to me) than the Rs. 2,000. And if I considered a pair of trousers, or a few days worth of groceries, or a book more valuable, I would not have bought the shirt. Hence, the value of the shirt was relative; not just to the Rs. 2,000, but countless other things that I might have needed.

The concept of need is also complex. Like value, it involves multiple factors and entities. It might also involve price. For example, the price of something might influence our need for it. Paradoxically, often the more expensive a good is, the more we feel we need them (either from wanting to spend on luxury, to believing a more expensive good is a better good).

Hence, when you consider the broader picture (the shirt-seller, other people that sell things to me, and the vast supply chains surrounding them), the value of my shirt is connected to the value of an almost infinity of things.

The value of anything in the the mind of anyone, is connected to the value of everything in the minds of everyone.

![Image](https://cdn-images-1.medium.com/max/800/1*VhSYXfHaNgMxUAUm5r2LVg.gif)

## A stupid idea — Revisited

Given the nature of value and its connectedness to everything, it is impossible to act like Homo Economicus, and make optimal buying and selling decisions, because we don't really know what the value of anything is.

The guardians of Homo Economicus (i.e. Classical Economists) usually give two rebuttals to this argument:

* While, in theory, the value of a thing is connected to the value of everything, in practice a small set of these everything, have a disproportionately big influence on value. While, in theory, this is true, in practice, Economists are, at best, vague, and at worst, horribly wrong, on how big the small set of things is. Almost every economic disaster has been a result of Economists "mis-underestimating" the bigness of the small set.

* The other argument is that, there are, indeed, things with "absolute" value: like money or gold. An Economist would tell you, "Rs. 1 has a value of exactly Rs. 1". Again, true, in theory, but false in practice. We know that inflation, and devaluation affect the value of all money. But even if we discount effects like inflation, we know from experience that Rs. 1,000 that we worked hard for, or was a gift from a close relative, has a lot more value to us than Rs. 1,000 we won in a lottery, or randomly picked-up on a street. Hence, even money has no absolute value.

## Samuel Goldenberg and Schmuÿle

There are two types of person to whom this article is irrelevant.

* The first type is the Rich Person. And by rich person, I don't mean Dhammika Perera or Victor Hartmann's Samuel Goldenberg, or even Bill Gates. I mean someone so rich that they could buy out Bill Gates, the entire United States of America (People, Resources, Finances and all), and the entire Peoples' Republic of China, with their spare change. For this person, nothing has price. There is no difference between a $1 bill and a $100 bill.

* The second type is the hermit, who has renounced worldly things and comforts. Just as for the Rich Person nothing has price, for the hermit, nothing has value.

We all (including you, me, Perera and Gates) sit on a vast spectrum between the Rich Person and the hermit. And there is some consolation that if we are pressured in one direction, we can always go in the other. If we are short of money, then we can be a little more like a hermit. And if our lives are too hermit-like, we can splurge a little like a Rich Person.

![Image](https://cdn-images-1.medium.com/max/800/1*LO5FD1P89vTfbres87z0JA.jpeg)

## Bonus Consolation

But there is an assumption behind the value of different things. That different things have different values. But what happens when this assumption is broken? What happens if, to us, everything has the same value?

Shirts, Trousers, gold, money, or the view of a sunset over a valley?

Might we be both Rich Person and a hermit at the same time?

![Image](https://cdn-images-1.medium.com/max/800/1*fyXMJYD2JeLywdufyQL2hw.png)

#### Article 79 · September 5, 2019

# The Strange Case of the Lipton Circus Farter

### A short story

There is no justice for traffic lights. Day and night, they go about their business silently, without complaining. And, all we do is complain about them. Have you met anyone who has had a happy traffic light story?

One August afternoon, it was my turn to complain. The sun was directly above the red light, and the more I willed the light to change, the more my eyes burned in the sunlight.

While I stood arguing silently, I heard a sudden:

>>> "Why, man, you there standing and farts sending?"

To my left was an old gentleman in a maroon shirt, dark trousers, and well-polished shoes. He was staring at the red light and didn't see me.

Then he turned his head, and his face changed from an irritated red to sheepish green.

Almost immediately, a second old man, this time a little flatter in dress, but evidently the first man's side-kick, joined us.

The first man's gaze moved from me to the second man, and he redirected his previously misdirected admonitions to his friend:

>>> "Why, man, you farts sending?"

The second man looked at both of us, once bewildered, twice embarrassed, and thrice indignant.

>>> "I farts sending not!"

As this important discussion took place, I remembered seeing both men crossing the road with me, as I crossed Alexandra place from ODEL towards Davatagaha Mosque. I remember pondering which crossing to take.

You see, Lipton Circus is a complicated intersection of six roads at two interconnected traffic roundabouts. It takes a bit of time to decide which crossing to take. To get from ODEL to Union Chemists, you need to cross two roads; from the General Hospital Outpatient Department, three. And if you make the wrong turn, four, even, five.

By this time a gaggle of students from Buddhist Ladies College had joined us and started giggling at so many mentions of "fart". To make things worse, the second old man continued to protest with childlike dudgeon.

>>> "I farts sending not! Sending not!"

Finally, the traffic light, the root of all our sorrows, changed. We, farts and all, crossed the road.

The two old men walked in the opposite direction, towards Paradise Road, evidently, taking their fart talk with them. I made my monthly visit to Union Chemists, handed my prescription to the attendant at the counter and waited. She returned momentarily with two plastic bottles, sniffing the air.

Several customers at ODEL had complained to my supervisor, and the nice lady doctor at the General Hospital Outpatient Department recommended doubling my dose.

I walked out, and "Damn!", I said to myself. Another red light!

...

[This is a work of fiction. Names, characters, businesses, places, events and incidents are either the products of the author's imagination or used in a fictitious manner. Any resemblance to actual persons, living or dead, or actual events is purely coincidental.]

#### Article 80 · September 5, 2019

# What's done is perfect

### Confessions of a three handed house-sweeper

Sweeping a house is a bitter-sweet experience.

On one hand, the good thing about giving your house a jolly-good sweep with a broom is that you end-up with a cleaner house.

On the other hand, there are a couple of things I find frustrating:

* During sweeping, the back and forth movement of the broom causes a mini "wind-surge" that disturbs the already swept heap of dirt.

* After sweeping, the process of transferring the dirt from the floor, to the dust-pan and finally to the dust-bin is never perfect. There's always a bit left on the floor.

But on the third hand, these frustrations do have a silver lining. Whenever the wind-serge distrubs the heap, usually only a small amount of dirt is disturbed. So you still have more dirt in the heap than pre-sweeping. Similarly, with each episode of the dust-pan, there is less dirt on the floor.

This reminds me of Achilles and the Tortoise, and the geomatric series. Consider:

>>> 1 + ½ + ¼ + ⅛ + ...

This series never sums to 2 exactly. But with each addition, it gets closer and closer to two. After 2 steps, it is equal to 1.5. After 4 steps, 1.875. After 10 steps, ~1.999.... After 20 steps, ~1.99999...

Sweeping is like this geometric series. After each sweep of the broom, the floor is a little cleaner, and a little closer to the perfect floor. As is the case after each scoop of the dust-pan. A theorotical perfection is never reached, but each step is more and more perfect. A sort of absolute (if not relative) perfection.

In fact, 1.5, 1.875, 1.999... and 1.999999... all have their own perfection. They might not be exactly 2, but they are computed and done. And what's done is perfect.

But I'll stop writing now. What's done is perfect.

![Image](https://cdn-images-1.medium.com/max/800/1*HS7ReTgrD6fx4G8IZwUJzw.jpeg)

#### Article 81 · September 6, 2019

# On Cutting the Cake

### Splitting Startup Stock and the Principle of Proportionality

## Alice meets Bob

A startup founder (let us call her Alice) approached an investor (let us call him Bob).

Alice had built a small but stable business with annual revenues of Rs. 2M, from about 40 loyal customers. Her yearly costs, taxes, and other expenses were about Rs. 1M, and she paid herself the remaining Rs.1M as a salary.

Alice asked Bob for an investment of Rs. 2M, for a 20% share of the company (at a Rs. 10M valuation).

Alice claimed that the company had the potential to 2x revenues annually for the next five years, while costs would be proportional to revenues.

Bob did some quick calculations. The company currently made an annual profit of Rs. 1M. That would double at the end of the first year to Rs. 2M. Similarly, the profits at the end of the 2nd, 3rd, 4th and 5th year would be 4M, 8M, 16M and 32M respectively. Hence, (ignoring inflation), the total profits in the next five years would be Rs. 62M.

And assuming the lifetime of the business was five years, the valuation of the company would be a similar figure. Hence, an investment at an Rs. 10M would be a steal.

But of course, this is not the case. Bob's calculation does not factor in risk. And startups are all about risk.

## Distribution of Valuations

In her meeting with Bob, Alice gave, actually, two valuations.

* A best-case valuation, while describing the companies "potential", where the company would be worth at least Rs. 62M

* A "conservative" case valuation while making an offer to Bob, where the company was worth Rs. 10M.

It is a good bargaining tactic first to describe an optimistic potential and then describe a more "conservative" offer.There is also a worst-case valuation that Alice (and most founders) failed to mention. Rs. 0, or even negative, where the company fails and goes bankrupt.

Hence, in reality, valuations follow a distribution.

A founder's "conservative" valuation is rarely conservative. An investor is more likely to get an 80% best-case valuation when they are, perhaps, expecting a 50% best-case (median) valuation.

![Image](https://cdn-images-1.medium.com/max/800/1*3mYkEgA4-XJXZyE3pqFPig.png)

## What should Bob do?

There are some obvious things that Bob should do; due-diligence to make sure that everything makes sense.

* How reputable is Alice?

* How happy are the customers?

* How genuine are the numbers?

But there is another sobering reality: Everything is uncertain with startups. Everything we said about the future, from the best case to the worst-case valuation, is highly unpredictable and debatable.

So, what should Bob do, after doing the obvious things?

## The Principle of Proportionality

Alice and Bob don't know the future: whether it would be the Rs. 62M Best Case, the Rs. 10M not-so-"conservative" case, or the Rs. Zero-or-worse worst case. But we know there would be some case.

Whatever the case is, Alice and Bob should try and enforce the following principles of proportionality:

* Any dividend or profit or gain should be proportional to investment share

* Any loss should also be proportional to investment share

These principles are another way of saying, everyone should be treated fairly.

What does this mean in practice?

## Alice and Bob — Revisited

Let us consider the worst-case first, where the company, in actuality, has no value. During the first year, Bob loses his Rs. 2M and Alice loses Rs. 1M (assuming she paid herself a fair salary).

Now, we see that "Any loss should also be proportional to investment share" is broken. Bob suffers 67% of the loss, after investing 20%. Alice, on the other hand, only suffers 33% of the loss, after owning 80% of the company.

Hence, in the worst-case, the share split is not fair. How can we fix this?

Now, Bob's 20% share is based on a Rs. 10M valuation. In other words, Alice agrees that the company is worth Rs. 10M. But at the end of the first year, she has committed on Rs. 1M to the company. Hence she should own only 10% of the company. Not 80%!

### Instalments to the rescue

We can fix this problem by giving Alice stock, not all at the beginning, but in instalments. In the beginning, she has zero shares, but by the end of the first year, she is awarded a total of 10%, possibly in monthly instalments.

This assumes that Alice takes all her compensation in the form of shares. Alternatively, she might opt for Rs. 500K in cash, and 5% of the company share.

### Conditional cliffs

But this was the worst case. What if the company does well? What if, as projected in the best-case scenario, at the end of the first year, the company makes Rs. 2M in profit. Now, this will entitle Alice to a further Rs. 2M of shares, or another 20% (a "cliff"). Hence, in this best-case scenario, at the end of the first year, Bob will have 20% of the shares, and Alice 30%. Similarly, at the end of the 2nd year (Rs. 4M in profit + Rs. 1M in salary), Alice will have an 80% share in total.

Now, what happens if the 3rd year also completes accordingly to the best case projection? All shares have been divvied up, and Alice can't have more stocks. This might sound unfair, but this is a function of Alice and Bob deciding on a 10M valuation. Alice could buy some of Bob's shares, but given the performance of the company, Bob will undoubtedly want a higher valuation than Rs. 10M.

Alternatively, if Alice could have predicted this future, she could have pushed for a higher valuation at the beginning. For example, if Bob agreed to a Rs. 20M valuation, at the end of the first year, Bob would have owned 10% of the company, and Alice 15%. And at the end of 3 Years, Bob would have remained at 10%, while Alice owned 90%.

## Conclusion

To conclude, whatever the case is, founders and investors should try and enforce the principle of proportionality. Fairness is the key to all successful partnerships.

### Update: Follow-up

* https://medium.com/on-economics/on-cutting-the-cake-part-2-a67126043196

#### Article 82 · September 7, 2019

But Alice is guaranteed of stock in installment, plus a cliff conditional on the company performing well. Is this insufficient? Under what circumstances would Alice get a bad deal?

#### Article 83 · September 7, 2019

Re: End of the day, startup investing is a high-risk and high-reward class of asset that is strongly correlated to time. Comparing it to other investment classes for proportionality is generally misleading IMO.

Agree on the point about comparison. But do you think I'm making a comparison?

#### Article 84 · September 7, 2019

Re: Founders should be paid in cash+stock where the total value is a multiplier (<2 series A, changes as you go up) on the general market value in my opinion as what the founders bring to the table cannot be matched with what a professional of the same class can bring the company if she was replaced in the same business in her role.

This is true if the founders are, as you imply, high quality and even exceptional. In practice, not all founders might meet this bar. Even among the exceptional, there is a spectrum.

#### Article 85 · September 7, 2019

Re: However, the founder in this situation approaches the investor with a business that does have value from the start.

This is not true. The business does have some value. What made you assume otherwise?

#### Article 86 · September 7, 2019

Re: The different way to look at this would be the founders have created value and the investor is buying a portion of that value.

Completely agree. This is also the principle behind the principle of proportionality.

#### Article 87 · September 8, 2019

# How happy are Sri Lankans?

### Reflections on the World Happiness Report 2019

## Suspicious and Suspiciouser

On March 30th, the United Nations Sustainable Development Solutions Network published their World Happiness Report for 2019. Sri Lanka was ranked 130th out of 156 countries. I found this a little surprising. Are we that unhappy?

Digging a little deeper, things looked even more suspicious. Reputable hell-holes like Congo and Iraq were ranked above Sri Lanka. Were people actually happier in Congo or Iraq?

![Image](https://cdn-images-1.medium.com/max/800/1*Dy4IivYa6b4t6CvPP_zyLQ.png)

This didn't feel right. So I thought of investigating a little deeper.

## Measuring World Happiness

According to Wikipedia, the World Happiness Report's Happiness Score is computed as follows:

>>> "The rankings of national happiness are based on a Cantril ladder survey. Nationally representative samples of respondents are asked to think of a ladder, with the best possible life for them being a 10, and the worst possible life being a 0. They are then asked to rate their own current lives on that 0 to 10 scale.The report correlates the results with various life factors."

For example, when a representative sample of Sri Lankans were asked to current lives on a 0 to 10 ladder, the average answer was 4.366.

The authors then tried to explain the score, by correlating it to several life factors that were expected to influence happiness. These factors were:

* GDP per capita

* Social support

* Healthy life expectancy

* Freedom to make life choices

* Generosity

* Perceptions of corruption

The result of correlating the Happiness Score with the life factors was an equation like this:

Estimated "Happiness Score" = "Score Explained by GDP per capita" + "Score Explained by Social support" + "Score Explained by Healthy life expectancy" + "Score Explained by Freedom to make life choices" + "Score Explained by Generosity" + "Score Explained by Perceptions of corruption" + 1.88

Now, according to this linear function, the Estimated "Happiness Score" for Sri Lanka is something like:

Estimated "Happiness Score" = 0.559 + 0.949 + 1.26 + 0.831 + 0.470 + 0.244 + 0.047 + 1.88 = 5.687

What this means is, given Sri Lanka's life factors, Sri Lanka's Estimated "Happiness Score" should be 5.687. But this is more than Sri Lanka's actual Happiness Score 4.366. In other words, the Sri Lankan's interviewed "say" that their happiness was 4.366, but given "how things actually are" in Sri Lanka, it should be 5.687.

The United Nations Sustainable Development Solutions Network Pandits call this difference the Dystopia Factor. Sri Lanka has a particular negative Dystopia Factor of 1.321, implying that Sri Lankas say that they are much less happier with their current life situation than they should be given their real circumstances.

## How things really are

I recomputed the Happiness Scores by removing the bizarre Dystopia Factor. "Say they are" are the "Happiness Scores" reported in the World Happiness Report. "Really are" is this score minus the Dystopia Factor.

![Image](https://cdn-images-1.medium.com/max/800/1*--BicngL8C5W0YAskhbiLQ.png)

While the macro pattern doesn't change much (the top ranks are dominated by the "west" and the bottom ones by Africa), the countries that significantly changed ranks are interesting.

### The countries with the 10 highest dystopia factors (where people "say" things are much worse than they "actually are") are:

![Image](https://cdn-images-1.medium.com/max/800/1*2iXO_l3uSLBqtHnXWLpl8g.png)

Sri Lanka has the fourth highest Dystopia Factor. Under the "new scoring system", Singapore moves from 34th place to 1st place. There is no obvious pattern in the other countries. Three of them are reasonably well performing African countries (Botswana, Rwanda, and Tanzania), three are South Asian neighbours with similar culture (Sri Lanka, India and Myanmar), and two small countries which are economically developed (Hong Kong and Singapore).

### The countries with the 10 lowest dystopia factors (where things "actually are" much worse than people "say" they are) are:

![Image](https://cdn-images-1.medium.com/max/800/1*Mtv1rMV6QgSni9_TIvrM9w.png)

As before, this list also has a mix of very different countries, including the "happiest country" Finland, according to the original World Happiness Report. It has four Central American Countries (Costa Rica, Mexico, El Salvador), and three African countries (Benin, Niger, and Ivory Cast).

## A Philosophical Difference

The "Really are" and "Say they are" Happiness Scores have a subtle difference. In the latter, we assume that happiness is "what people say what happiness is". In the former, we first find factors that seem to influence happiness, and then see how the people are doing on these factors.

The difference between these scores is, as I said, subtle. The former, though seems statistically more robust, and corrects for cultural nuances like modesty, and emotional humility.

## Conclusion

There is some evidence that Sri Lankans tend to be more negative about their life situation and happiness. If we correct for this "Dystopia Factor" Sri Lanka's happiness score improves from 130th to 63rd.

While the World Happiness Report is sensitive to life factors that influence happiness, they should probably do some further research into factors that influence the measurement of happiness.

#### Article 88 · September 8, 2019

# How not to pick a President (Part 2)

### Some self criticisms

In my article, How not to pick a President, I discussed some cognitive biases that tend to influence how people vote. I discussed,

* Extreme Event Bias, including how so many people voted for Mahinda Rajapakse, just because he "won the war".

* Anchor Bias, including how so many people vote "always for the UNP" or whatever party or family affiliation

* Familiarity Bias, including how people are deeply influenced by shallow tactics like posters

Related in Who do you side with?, I discussed how two party, binary politics dominate so many countries, and how the "lesser of two evils" binary thinking stifles rational democracy.

The attitude I showed was that people with cognitive biases, and can't think beyond binary politics are stupid (and implicitly) less smarter than me. In other words, I seemed to imply the following:

* People who voted for Mahinda Rajapakse just be cause he "won the war" are dumb

* People who always vote Green or always vote Blue are dumb

* People who are influenced by posters and prime-time TV are dumb

* People who can only vote for one of the two dominant parties are dumb

But when I reflect on these points, particularly in the context of Sri Lanka's presidential election in 2019, I am also struck by the following:

* No third party (except criticize the main parties) has proposed a credible plan on how to govern the country. I haven't even hear a plan for a plan as yet. Have you?

* There has been no plan for educating the public on politics and civcs. So can we criticize posters and TV shows by moron presenters, without proposing something better?

* We "won the war" is a memorable phrase. Is there any inspiring alternative which can rally the people? And has it been ever said by someone who the people know and trust?

* Finally, can we even have national politics without national identity? Is there any point in optimizing national politics (and related optimizations like reducing corruption), without building national identity?

At least for me, food for thought. Bon Appétit!

![Image](https://cdn-images-1.medium.com/max/800/1*GlMd7SE4cDUnA18IXDsUqg.gif)

#### Article 89 · September 8, 2019

# On Maps

### From Concrete to Abstract to Inspiration

I've been fascinated by maps from a small age. As a child, I would spend hours trying to draw the road map of Colombo. My grandfather subscribed to an annual report titled The Natural Resources of Sri Lanka, which contained all manner of maps about rivers, mountains, gem stones, crops and people, and I would trace the various depictions of the country onto pieces of paper.

And this fascination has continued into adulthood. While living in London, Harry Becks iconic Tube Map, was a constant preoccupation. While traveling on the underground, I would gaze at the maps on the opposite wall, memorising stations, and analysing interchangers.

But what makes a map a great map? Why are maps fascinating?

![Image](https://cdn-images-1.medium.com/max/800/1*yKj8hmfquaQVPY-P7z5wzw.png)

Maps represent the real world, which (by definition) is real, and concrete. But in representing the real world, maps simplify it; maps minimise the information of the concrete into an abstraction; maps reduce.

In this sense, maps are an incomplete, inaccurate, and imperfect representation of the real world. For example, the Tube Map does not capture the distance between tube stations. Bayswater and Lancaster Gate are a short walk from each other, but appear several stops apart.

But at the same time, and paradoxically, this reduction process also inspires. A human looking at the map is stimulated to think about the concrete behind the abstraction in new and creative ways. For example, when one looks at a Tube Map, you see all the intersections, junctions, and changes. A simple form of creativity is how easy it is to "create" trip. Hence, the reduction promotes expansion.

![Image](https://cdn-images-1.medium.com/max/800/1*bSr896R0uwCZfS1cvdZ2Kg.png)

And of course, this pattern can be extended to all abstractions, from mathematics to art.

#### Article 90 · September 9, 2019

# Anatomy of a Tennis Match

### Dissecting the 2019 US Open Men's Final

![Image](https://cdn-images-1.medium.com/max/800/1*6nEKEpDgd4fJd6bbMm95kQ.jpeg)

## Point

>>> You: So, who won? Nadal or Medvedev?

>>> Me: Medvedev won the 1st point.

>>> You: No. I asked who won the match

But points are interesting. A point is the smallest unit of score (or "play") in tennis. One player serves, and the other tries to return. Whenever someone misses, or hits the ball out, or is obstructed by the net, the other scores a point. Points are vital!

![Image](https://cdn-images-1.medium.com/max/800/1*T_ohvJvgi9FlKirm5GIj6g.png)

## Game

>>> You: I'm not necessarily (or should that be sufficiently) interested in points.

>>> Me: Ok, ok. Nadal won 5 of the first 8 points, to Medvedev's 3, and won the game.

>>> You: Ok. So Nadal won the match?

No. Nadal won the game; The first game. Whenever a player wins at least 4 points, and has won at least 2 points more than the other player, they win the game. And after that a new game is played. Nadal won the 1st game.

![Image](https://cdn-images-1.medium.com/max/800/1*SOAIGdBUwMOeDcAjRRLiBQ.png)

## Set

>>> You: I'm not interested in playing games. Who won the match?

>>> Me: Nadal won the set.

>>> You: He won all the matches?

No, no. Nadal won 7 games to Medvedev's 5. Whenever a player wins at least 6 games, and has won at least 2 games more than the other player, they win the set (Tie-breakers are an exception, but I won't go into that). And after that a new set is played. Nadal won the 1st set.

![Image](https://cdn-images-1.medium.com/max/800/1*DViqmD798Jox11YXW0reZg.png)

Also, at the end of the 1st set, Nadal had won a total of 45 points to Medvedev's 36.

## Match

>>> You: I'm not interested in set theory. For the last time, who won the match?

>>> Me: Nadal won 3 sets to Medvedev's 2. So he won the best-of -5-sets match, 3–2.

>>> You: Thank you! That's all I wanted to know.

![Image](https://cdn-images-1.medium.com/max/800/1*AObDU14MTrE-ehMjtdNb9g.png)

>>> Me: But you might want to know other things.

>>> You: Such as?

Nadal won a total of 28 sets to Medvedev's 25. Nadal also won a total of 177 games to Medvedev's 164!

>>> Me: And I might want to know that because?

If tennis had a simple scoring mechanism like Basketball, the final score would have been 177–164. Nadal would have won, but the game would have been completely different! Imagine sitting through 341 points??? Everyone would have left by the 3rd set, if not before.

>>> You: So what's your point?

>>> Me: Ha, ha. "Point". That was funny!

## My actual "point"

Games (in the general sense, not the tennis "game") can be classified along two dimensions. "Plays" and "Scoring".

Tennis has simple plays (ending in a point), and complex scoring.

Football has complex plays (which usually last several, or tens of minutes), and simple scoring. Rugby Football (I find) is (even) more interesting, because it has equally (or even more) complex plays, and a less simple scoring system.

Basketball has both simple plays and simple scoring — which is why it is tedious and best suited for people with IQs of a rugby (or even football) score. You might as well start at 100-all, and just play the last 5 minutes. Tennis would descend to the same depths if not for its beautifully complex scoring system. The fact that the basket in basketball didn't have a hole for the first several decades of the game, is proof of this low-IQ-ness of the basketball fraternity.

Cricket has apparently simple plays (a ball bowled by a bowler to a batsman), which is made complex by a wide range of possible outcomes: Nothing happening, several ways of a wicket falling, a theoretically infinite diversity of runs, and in many situations — rain! The combinations of runs and wickets makes the scoring of Test Cricket complex. For example, one team might have far less runs than the other team, but won't lose if they don't lose all their wickets. 50-Over, and T20 cricket, unfortunately, tries to emulate the "simplicity" of Basketball. The complexity of plays redeems it, but the simplicity of scoring undermines the game's beauty, and also its "glorious uncertainties".

![Image](https://cdn-images-1.medium.com/max/800/1*7ui4FJxA9XwIBPfe28KbFw.png)

#### Article 91 · September 9, 2019

# On Cutting the Cake (Part 2)

### Day Zero Value

In On Cutting the Cake, I discussed the topic of splitting startup stock in general, and the principle of proportionality in particular:

>>> Any dividend or profit or gain should be proportional to investment share

>>> Any loss should also be proportional to investment share

Several of you expressed some concerns, that my recommendations would be unfair to founders, as opposed to investors. Several of you referred to my toy example:

>>> "We can fix this problem by giving Alice stock, not all at the beginning, but in instalments. In the beginning, she has zero shares, but by the end of the first year, she is awarded a total of 10%, possibly in monthly instalments."

In this follow-up to On Cutting the Cake, I want to address two of your concerns. Namely that,

* The scheme ignores value already built by the founder

* The founder has no shares at the beginning, and might loose control of the company

## "The scheme ignores value already built by the founder"

In my toy example, the founder Alice had already built a business with some value:

>>> Alice had built a small but stable business with annual revenues of Rs. 2M, from about 40 loyal customers. Her yearly costs, taxes, and other expenses were about Rs. 1M, and she paid herself the remaining Rs.1M as a salary.

So why did I recommend that Alice should have 0% ownership of the company at the beginning? Especially given that Alice had proved value?

My next point might be controversial, but is at the basis of my recommendation:

When we say "Alice had proved value", what we actually mean is that we are "predicting future value based on past value". And as with any prediction, this prediction is uncertain.

Now, what is the uncertainty (or variance, or "error-bars") of this prediction? To understand uncertainty, we would need to consider similar startups — or, to be precise, a statistically significant number of similar startups. Now, for any startup you might want to invest in, how many similar startups do you know? And know well? This is the problem. Each startup is unique, and, hence, it is almost impossible to make accurate predictions about the future.

Now, neither can we say that the value of this startup is zero. All we can say is that we can't say anything. Hence, we get around the problem of prediction by postpoing our decisions that need that prediction, until we have credible information.

Hence, as Alice adds value to the company by working (and providing credible information that Alice is indeed prepared to work, as opposed to running away with the investment), she earns stocks:

>>> In the beginning, she has zero shares, but by the end of the first year, she is awarded a total of 10%

Similarly, if the company proves value (more credible information), again, Alice earns more stock:

>>> What if, as projected in the best-case scenario, at the end of the first year, the company makes Rs. 2M in profit. Now, this will entitle Alice to a further Rs. 2M of shares, or another 20% (a "cliff"). Hence, in this best-case scenario, at the end of the first year, Bob will have 20% of the shares, and Alice 30%. Similarly, at the end of the 2nd year (Rs. 4M in profit + Rs. 1M in salary), Alice will have an 80% share in total.

Hence, I don't ignore value. I merely postpone decisions that need an accurate estimation of value, until I have this information.

## "The founder has no shares at the beginning, and might loose control of the company"

The founder is contractually entitled to receive instalments of stock on both 1) a time basis, and 2) on the company performing well (see above examples).

In our toy example, by the end of the first year, founder Alice has a majority of the shares:

>>> ...at the end of the first year, Bob will have 20% of the shares, and Alice 30%.

This majority increases with time:

>>> Similarly, at the end of the 2nd year (Rs. 4M in profit + Rs. 1M in salary), Alice will have an 80% share in total.

## Concluding thoughts

One (possibly contrarian) principle which most founders and many investors don't accept is that it is not possible to value startups on day zero of an investment. Many who do accept this point, still try to pretend that valuation is possible, because they don't see an alternative.

There is an alternative, and that is to postpone part of the stock split decision until more information is available. Contrarian perhaps, but quite simple.

![Image](https://cdn-images-1.medium.com/max/800/1*eoT9yBOU02V7JYqso1Fp8A.png)

#### Article 92 · September 9, 2019

# On Cutting the Cake (Part 3)

### Stock for Employees and the Motivation Principle

In On Cutting the Cake, I discussed the topic of splitting startup stock in general, and the principle of proportionality in particular:

>>> Any dividend or profit or gain should be proportional to investment share

>>> Any loss should also be proportional to investment share

In this follow-up, I discuss a corollary of the Proportionality Principle, which I will call the Motivation Principle, and in particular, discuss its effect on employees.

## A personal note: Silicon Valley vs. Silicon Isle

When I first interviewed for software engineer jobs in Silicon Valley, I had the following new experience: In addition to a cash salary, my compensation offers also included stock. In some cases, the stock component even exceeded the cash component. Startups almost always offered stock, and so did many "big" companies — especially to high quality candidates.

In fact, for high quality candidates, in addition to higher cash compensation, companies also offered a higher proportion of stock compensation. This implied that companies assumed that higher quality candidates valued stock more than cash.

While I had some work experience in Sri Lanka before I moved to California, I had never encountered, or even heard of a Sri Lankan tech company offering stock (note this was back in 2007).

## The Motivation Principle

When both profit and loss is proportional to investment (Proportionality Principle) investors want to do their best to maximise the former and minimise the latter, motivating everything from working harder, to working smarter. Hence, the Proportionality Principle motivates investors to re-invest in all sorts of beneficial ways.

Or in other words:

>>> Proportional investment, motivates further investment.

This is what I call the Motivation Principle.

An obvious corollary of the Motivation Principle is if you want an employee to work hard and smart, give them stock. Better still, make sure that stock is proportional to performance.

Note, disproportionalities would result in asymmetric motivation, or even demotivation. For example, if a company is doing well, employees without stock would feel less part of this success, particularly since they don't get to completely share in it. On the other hand, if the company is doing badly, such employees would care less.

## Conclusion

The conclusion is simple. Give 'em stock.

![Image](https://cdn-images-1.medium.com/max/800/0*UQjg1QpnA3g_inN_.png)

#### Article 93 · September 9, 2019

# The Big Three

### On the dominance of Federer, Nadal, and Djokovic 2003–2019

![Image](https://cdn-images-1.medium.com/max/800/1*yYMRYnGFG3LbHDbaou9C7A.jpeg)

## 55 out of 68

With Rafael Nadal's win in the final grand slam for 2019, Federer, Nadal, and Djokovic (the "Big Three") have, between them, won an astonishing 55 out of the 68 finals (81%) since 2003.

I wanted to visualise this history in a picture:

![Image](https://cdn-images-1.medium.com/max/800/1*C-cMMBDZbf6_q9nDAWjfrQ.png)

While each of the Big Three have won at least one of the grand slams, they have clearly won some more than others. Nadal is the most "asymmetric"; 12/19 or 63% grand slams have been the French Open. Federer clearly favours grass (8/20 or 40%), and Djokovic has dominated the Australian open (7/16 or 44%).

Federer has the most "symmetric" record, which backs up the Jimmy Connors quote:

>>> "In an era of specialists, you're either a clay court specialist, a grass court specialist, or a hard court specialist...or you're Roger Federer".

## Almost winning

One important factor that the previous visual ignores is that each of the Big Three often competed with each other in a grand slam final. So, although Federer and Djokovic have only won one French Open each, they have each been in 4 and 3 finals respectively, which they lost to Nadal on 6 occasions between them.

![Image](https://cdn-images-1.medium.com/max/800/1*WJvyWk7hIHel_DM2BhLwkA.png)

In an era without Nadal, Federer and Djokovic would have won many more French Opens, and in an era without the Big Three, so would the likes of Thiem, Andy Murray (formerly part of the "Big Four"), and Warwinka.

Counting both all grand slam final appearances (wins and losses), the visual looks like:

![Image](https://cdn-images-1.medium.com/max/800/1*4kh9hR7autCWRAGAkN97Tw.png)

From this view, Nadal and Federer look more like Clay (French Open) and Grass (Wimbledon) specialists respectively, and Djokovic looks like the generalist. So should the quote be,

>>> "In an era of specialists, you're either a clay court specialist, a grass court specialist, or a hard court specialist...or you're Novac Djokovic" ?

## Honourable Mentions

![Image](https://cdn-images-1.medium.com/max/800/1*dgrIvkz0eASx5vTAbJoXBA.png)

At one time, Andy Murray was coupled with the "Big Three" to form a "Big Four". However, this name has been dropped since then, given the gap between his performance, and the other three.

However, if were were to coin a Big Four, Murray would be a top contender, together with Stan Warwinka, both of whom have won 3 grand slams (2003–2019) each.

And if we further rewind history, we see that 5 other players (Sampras, Emerson, Laver, Borg, and Tilden) have won at least 10 grand slams.

![Image](https://cdn-images-1.medium.com/max/800/1*6-Zf6CUgPvxxYBQ5DBI15A.png)

## The Big One

There is no Big Three in women's tennis. Not even a Big Two. But there is an obvious Big One. If we look at the same period (2003–2019), Serena Williams has won 19 of 68 grand slams (not counting the four she won before 2003).

No other player comes close, with Justine Henin and Maria Sharapova a distant second and third with 7 and 5 grand slams respectively.

![Image](https://cdn-images-1.medium.com/max/800/1*xMPwRZDeex6aYzeC6TzyWw.png)

Williams' wins are also more symmetric than the men's. So the quote should be,

>>> "In an era of specialists, you're either a clay court specialist, a grass court specialist, or a hard court specialist...or you're Serena Williams"

Game, Set and Match!

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

#### Article 95 · September 10, 2019

# On Discipline

### In nomine Patris et Filii et Spiritus Sancti

Sri Lankans are supposed to be undisciplined. On the road, where we drive like maniacs. In the workplace, where we are lazy and erratic. Even in parliament, where we are (I'm told) incompetent and corrupt.

Many Sri Lankans also hate undisciplined people, and for this reason, many Sri Lankans hate many other Sri Lankans. The former also pontificate a lot on how to make the latter more disciplined.

In this article, I intend to go one step further. And pontificate on the pontificators.

![Image](https://cdn-images-1.medium.com/max/800/1*oTuP2cb5r0JdfuG-9HWvwA.jpeg)

## The Son

How do you make a manic driver mend their ways? How do you stop them from jumping lanes, running red lights, and horning at every second opportunity?

"You cannot", says the son.

"They have to mend their ways. They have to have consideration, compassion and empathy for their fellow drivers. And until all drivers are like this, our roads will be manic."

"And why should they cultivate consideration, compassion and empathy?", we ask.

"Out of loyalty and gratitude to society", continues the son. "Just as I am loyal and grateful to my father".

The same applies to the workplace and parliament. Workers, out of loyalty and gratitude to their employers, customers and shareholders, should work hard and smart. Politicians, out of loyalty and gratitude to the people, should be honest and competent.

At least, so says the son.

## The Father

But the father disagrees.

"That manic driver will never mend their ways. Unless you give them a bit of stick, like a father disciplines a son", continues the father.

"Drivers have to have fines, and licences taken away at the smallest sign of naughtiness."

And the same applies to workers and politicians. Employees need to be strict. Rules have to be enforced, and laggards fired. Politicians need oversight and must be subjected to a state of law.

"And why does the father discipline the son?", we ask.

"Because that's the only way a system can work. If rules are enforced, like a father disciplining a son", the father concludes.

## The Holy Spirit

Both the father and son have something in common. The son seems to obey arbitrary rules to please the father, and the father enforces arbitrary rules to nurture the son. How "arbitrary," you think these, depend on your personality. If you are a cynic, everything is too arbitrary. If you are an idealist, nothing is.

We are all neither total cynics nor total idealists: We are to varying degrees realists. We all have a sense of son and a touch of father.

And the reality is that we need to think like both father and son at the same time. Without the son, society feels repressed. Without the father, society breaks into anarchy.

Whether road, workplace or parliament, we need to ask two questions: 1) Is the son present to a sufficient degree, and 2) Is the father also present to a sufficient degree? There is no point in expecting discipline if one of there other is missing.

We cannot force employees into working harder or drivers into driving better. Nor can we expect politicians to be honest, if there are no rules to govern them.

We need a spirit of both son and father: a sort middle path — a holy spirit.

#### Article 96 · September 11, 2019

# On Libertarianism

### A Critique

![Image](https://cdn-images-1.medium.com/max/800/1*0jtH0EE9CcvV-02H3CGuzQ.png)

Libertarianism is a political philosophy that expounds that, the highest moral good is "an individual's right to satisfy their interests". The optimal way to secure this good is through "individuals making individual rational decisions".

Hence, Libertarianism relies on the trueness of the following propositions:

>>> A. The highest moral good is "an individual's right to satisfy their interests".

>>> B. The optimal way to secure this good is through "individuals making individual rational decisions".

>>> C. Individuals can make individual rational decisions.

Let's look at each of these, one by one, in reverse order.

## C. Rationality

Unfortunately, according to the latest findings of medicine, psychology and behavioural economics, humans rarely make rational decisions. Humans are more "rationalizing" than rational. We do something (without any rational basis), and then post-rationalize some excuse after the fact.

Hence, C can't be true.

## B. Decisions

But suppose for argument's sake we assume that C is true, that humans can, at least in the interests of satisfying their interests, make rational decisions. Would B hold as well?

Why would an isolated individual decision be more optimal to one made as a collection of individuals? Wouldn't a collective of individuals be more creative than a single individual, and have access to more information than one?

Also, what about the manifold instances where individuals defer decisions to others? As in the case of doctors? And generals? Why not even politicians?

Hence, B also breaks down.

## A. Interests

But suppose we ignore everything above and assume B and C to be true. Why should A also be true?

Don't many people see moral good in interests beyond the individual? Don't many people see moral good in pursuing and satisfying the interests of others (altruism)? And don't many people combine the interests of self and others, and seek the good of the collective?

Hence, A breaks down too.

## The Religion of Libertarianism

With A, B, and C all breaking down, the only way anyone can be a Libertarian, is if they accept A, B, and C as a matter of "faith", i.e. "based on spiritual conviction rather than proof".

This faith seems to be abundant in most Libertarians I've met. Libertarians sound a lot like Religious fanatics, often nitpicking facts, and trying to make points through the force of force, misinformation, emotion, and irrationality, as opposed to the force of rational argument.

Hence, the paradox of Libertarianism is, that for a philosophy that claims to worship rationality, it relies almost entirely on irrationality.

Libertarianism has another parallel with many religious scams like mega-churches and tele-evangelism, where a few people get rich, while making many poor. If you happen to be a scammer, monopolistic plutocrat, or robber-baron yourself, it would probably be in your interests to convince as many people that no one should interfere with your "right to satisfy your interests". Why not make a donation to the Libertarian party? High ROI (return-on-investment), methinks.

![Image](https://cdn-images-1.medium.com/max/800/1*_5mqMbthO8WT5uRpBxEkSA.jpeg)

#### Article 97 · September 12, 2019

# On Working from Home (WFH)

### Should Tech Companies support WFH?

My definition of "working from home" is:

>>> Working from your private residence, when your employee owns an office (an official central place of work) within commuting distance, from where most of your co-workers work.

![Image](https://cdn-images-1.medium.com/max/800/1*DAvBm5T2Z6LjA_NA2UdSdg.jpeg)

Working from home is somewhat controversial. Back in 2015, CEO Marrisa Mayer famously banned working from home at Yahoo. Other companies and CEOs supported or refuted "WFH" to various degrees. At Facebook, we had "No Meetings Wednesday" de jure, which, to many employees became "WFH Wednesday" de facto.

The question I want to answer in this article is,

>>> If you have a (say) Tech Company with a reasonable number of employees (say 20+), what should you policy on WFH be?

Let us start by first considering two factors that made WFH possible in the first place.

## Factors that make WFH possible

### 1. The "Home Office" and remote communication

My first work laptop weighed over 3.5kg. And while I was also provided with a "Dell branded" laptop bag to transport said laptop around, I never took it anywhere, not to meetings let alone home. Not that I could have done much if I took the overweight machine home. I had dial-up internet, which was barely sufficient for email. 13 years later, my current laptop weighs a little over 1kg. I have an optical fiber internet connection, which, in addition to lightening fast email, also enables high quality Video Conferences with several parts of the world concurrently. My kitchen also contains several of the healthy snacks and beverages, no self-respecting tech company could afford not to provide.

Hence, from a productivity, point-of-view, my home is as high-tech as an office, and without the phenomenon of this "home office", WFH would not have been possible.

For many of us, work is about meetings: sometimes small meetings with one person, sometimes big meetings with several dozen. Pre-high-speed-internet, meetings could happen only in person, at the office. However, post-high-speed-internet, and with the advent of a wide range of companies that provided internet conferencing and meetings products, one could "call in" to a meeting while WFH.

Coupled with atrocious traffic, and high fuel prices, this factor has pushed many people to work partly or completely from home.

### 2. Performance Management

In the old days, managers evaluated an employee's work by how long they worked. Hence, the 8 hour work day, and the 40 hour work week. Some workers worked for longer, for which sometimes they got paid "over-time". There were elaborate systems for employees to "clock-in", and foremen and other tyrants would go around to check if employees were indeed "working".

Things are very different in the modern tech company. During one of my first meetings at Facebook, my manager told me:

>>> "If you finish what you planned to do today in 2 hours, then you're free to leave, and spend the rest of the day doing whatever. [He mentioned playing tennis]".

However, this was only possible because in a tech-company it was (relatively) easy to evaluate what people did (in my case, at the time, the types of things a junior Software Engineer did).

In the old days, a worker would be never allowed to WFH, because their manager would have no mechanism to measure "time" (the, then, currency of performance evaluation). However, nowadays, a remote software engineer could be asked to fix these bugs, or ship this code, and it would be easy to verify whether the bug was fixed, or the code shipped correctly.

Hence, the shift of performance management to be "outcome/impact based" from being "time based" further enabled WFH.

## Automata, Uber, and the Future of WFH (v1)

An automaton is a machine that takes in some input and deterministically produces some output. Optionally, it might have a internal "state", which might change on the input, and influence the output.

Our "Factors that make WFH possible" have several commonalities with automata:

* The internal "state" in the home and the office is almost identical, given advances in laptops, the internet and kitchens.

* A manager asking a software engineer to write some code, and the engineer writing and publishing that code, is like input and output. With sufficiently well written "requirement specs" the output can be as deterministic of that of an automata.

* In general, improvements in the "home office", performance management and remote communication all reflect in improvements in input, and output, and enable a more precise and deterministic connection between the two.

Uber Drivers also follow this pattern: Inputs are simple ("pick up this rider"); outputs are simple and deterministic ("the driver drove the rider to this location, on this schedule and route"); all drivers and cars have consistent states ("A 45 year old in a Toyota Prius, can do tomorrow, what they did today").

The problem with this Automata/Uber analogy is that it has an obvious dystopian consequence. Uber's plan is to replace its human drivers with self-driving machines. One reason Uber is doing this is because it can; because anything that is an automata can be automated.

Most Software Engineers who WFH might face the same fate as Uber Drivers, and Luddites. This "Future of WFH" (let's call it v1) looks bleak.

## Future of WFH (v2)

But unlike Uber drivers there is an alternative for Software Engineers (or some at least): A world where high-quality Software Engineers can retain their jobs, and WFH.

The key (and obvious) point is not all Software Engineers are automata. In fact, high quality software engineering is a highly creative process, and belongs to the type of work that I described in On Human Competence as "the set of all problems that machines cannot solve, but humans can". But not all Software Engineers operate in this high quality mode. In fact, all but the class of engineer that I describe in On Software Engineers as "A-grade" will risk loosing their jobs to automation, with or without WFH.

However, the "Human Competence" practiced by "A-grade" software engineers consist of complex interactions between people, machines and problems, and hence a future that supports them WFH would need some significant advances.

### Advance 1: Even more sophisticated communication, and "home offices"

Some of the most productive meetings I have, take the following form: 3–4 employees spend about an hour in a room with a white board and brainstorm ideas. We go in with few expectations, and we come out with some inspired, creative ideas. Replace the white board with a black board, and this meeting has mediaeval technological sophistication.

But on the other hand, it is incredibly difficult to recreate this experience in a remote, online world. I am yet to see a compelling product that supports this time of "brainstorming" remotely. However, VR and AR are likely to change this.

In general, supporting "creative" working from home would require several step-changes of advancement in conferencing and meetings technology.

### Advance 2: Sophisticated Performance Management

At Facebook, we had Performance Reviews every 6 months. One problem with this system was there was no clear way of evaluating performance that spanned several cycles. While it was easy to reward a project that shipped in 4 months, within a 6 month cycle, it was almost impossible to clearly reward a project that was 1 year old, and had another year to go. In this latter case, "reward for impact" was often differed. As a result, many engineers were incentivised and chose to work on shorter term projects.

The more "Human Competence" focussed software engineering projects become, the more long term, and more difficult performance measurement becomes. While it is easy to evaluate an automata, it is much harder to evaluate a creative human.

This advance is necessary for both a WFH world, and a "Work from Office" world of the future. There is no way a manager would allow an employee to WFH if he can't even measure the employees performance while at the office.

## Back to the present

"Future of WFH (v2)" is some years away, at least. At the same time, automation is making "Future of WFH (v1)" more and more real every day. For example, in Sri Lanka many BPO Software Engineering jobs, which were comparatively WFH-friendly, are going away fast.

Given this state-of-affairs, I predict some decline in WFH in the short term. "A-grade" companies, with "A-grade" software engineers will find it difficult to support WFH without the Future of WFH (v2)-advances I mentioned above. In parallel, the B and C grade software engineers will find automation erode their WFH-friendly jobs.

Hence, what should a tech company's WFH policy be?

>>> Tech companies should aspire to be "A-grade" companies, with "A-grade" software engineers.

>>> At present, it is difficult to employee "A-grade" software engineers on a WFH basis. So in the short-term, tech companies should move away from the WFH (v1) model.

>>> However, in the medium to long term, WFH (v2) will be back, and might be revisited.

#### Article 98 · September 13, 2019

# On Statistical Significance

### When is significant not significant?

>>> "Almost anything can be attacked as a loss of amenity, and almost anything can be defended as not a significant loss of amenity, which seems to signify that one should appreciate the significance of significant." — Sir Humphrey Appleby (Yes Minister)

## Heads or Tails ?

Let's suppose we have a coin. An ordinary coin with a heads side and a tails side. Now, suppose we toss it 10 times, and get the following results:

H H H H t H H H t H

8 heads, and 2 tails. Is the coin a fair coin? How might we answer this question?

## A Tale of Two Tests

One one hand, there are more heads than tails (8 > 2). On the other hand, a fair coin could have resulted in 8 heads (or even 9 or 10 heads, for that matter). So the vital question is: are there too many heads?

### Test A

Now, the probability of getting 7 or fewer heads by tossing a fair coin 10 times is ~94.6% (Alternatively, the probability of getting more than 7 heads with a fair coin is ~5.4%). Hence, our outcome of 8 heads is only found with a (relatively) small set of fair coins. A statistician could have said,

>>> "there is evidence to conclude that the coin is not fair at a 5.4% significance level (or 94.6% confidence level), because all but 5.4% of fair coins are expected to pass the 7 or fewer heads test".

### Test B

But similarly, the probability of getting 8 or fewer heads by tossing a fair coin 10 times is ~98.9% (Alternatively, the probability of getting more than 8 heads with a fair coin, is ~1.1%). Hence, if we got 9 or 10 heads, then we could say that it was very unlikely that the coin was fair. But since we got 8 heads, a statistician might have said,

>>> "there is no evidence to conclude that the coin is not fair at a 1.1% significance level (or 98.9% confidence level), since, like all but 1.1% of fair coins, this coin passes the 8 or fewer heads test".

What do we pick? Test A or Test B?

## True Nature

To know for certain if a coin is fair, we would need to analyse its physical nature. For example, if the coin is a perfect cylinder made of a uniform material, it will likely be fair. Since the specific dimensions of a perfect cylinder can vary, theorotically, there is an infinite variety of fair coins. Unfair coins, similarly, have some physical property that make them unfair. For example, they might be made of two different metals, of different densities.

Hence, if we knew the exact physical nature of the coin, we could have pronounced them fair — without experiment. However, if we don't have the ability to understand this nature, we might need to resort to experiments (like tossing the coin). The observations of these experiments, while functions of the underlying physical nature, don't completely reveal this nature.

Starting from this "True Nature" we could try and answer our "Is the coin fair" question from "first principles".

## First Principles and Roadblocks

We can break our problem, into several questions:

* What are all the possible physical natures the coin could take? Let's denote the various physical natures as N₁,N₂,N₃,...

* Is a coin with a particular physical form fair? Let's define function F such that F(Nᵢ) = 1 if a coin with physical nature Nᵢ is fair, 0 if it isn't.

* For each of these physical natures, what is the probability that we are observing such a coin? Let's denote the probability of observing a coin with physical nature Nᵢ with P(Nᵢ). We need to calculate, P(N₁),P(N₂),P(N₃),...

* For each of these physical natures, what is the probability of observing "H H H H t H H H t H" given that the coin tossed had that physical nature? Let's denote our observation ("H H H H t H H H t H") with O, and the probability of observing O given the coin tossed has physical nature Nᵢ with P(O|Nᵢ). We need to calculate, P(O|N₁), P(O|N₂), P(O|N₃)...

Now, using Bayes' Theorem the probability that a coin has a particular physical form Nᵢ given our observation O:

P(Nᵢ|O) = P(O|Nᵢ) . P(Nᵢ) / P(O).

The probability that a coin is a fair coin given our observation O is:

∑ F(Nᵢ). P(O|Nᵢ) . P(Nᵢ) / P(O).

Similarly, the probability that a coin is not a fair coin given our observation O is:

∑ (1-F(Nᵢ)). P(O|Nᵢ) . P(Nᵢ) / P(O).

Now, the coin is more likely to be fair if and only if,

∑ F(Nᵢ). P(O|Nᵢ) . P(Nᵢ) / P(O) > ∑ (1-F(Nᵢ)). P(O|Nᵢ) . P(Nᵢ) / P(O)

Or

∑ F(Nᵢ). P(O|Nᵢ) . P(Nᵢ) > ∑ (1-F(Nᵢ)). P(O|Nᵢ) . P(Nᵢ)

Unfortunately, the problem with this first principles approach is that we don't have an answer to two of the questions.

* Question 1: We don't have an exhaustive knowledge of all possible coins. Hence, we can't possibly enumerate N₁,N₂,N₃,... etc. exhaustively.

* Question 3: We don't know the probability P(Nᵢ) of a particular coin occurring

(On the other hand, Question 2 and Question 4 can be answered, through analysis and observation. Hence, F(Nᵢ) and P(O|Nᵢ) can be known, usually)

Hence, we meet a road block. Either we need to try and answer Question 1 and Question 3, or we need to make some assumptions.

## Back to the Real World

Let's revisit our two statistical conclusions:

>>> Test A: "there is evidence to conclude that the coin is not fair at a 5.4% significance level (or 94.6% confidence level), because all but 5.4% of fair coins are expected to pass the 7 or fewer heads test".

>>> Test B: "there is no evidence to conclude that the coin is not fair at a 1.1% significance level (or 98.9% confidence level), since, like all but 1.1% of fair coins, this coin passes the 8 or fewer heads test".

Both claims have something in common: we subject the coin to a test, which a fair coin is highly likely to pass, or highly unlikely to fail.

If a coin fails the test, and we pronounce it "not fair", there is a 5.4% chance that we are wrong in Test A, and a 1.1% chance that we are wrong in Test B. Hence, the only difference between the two "tests" is how wrong we are prepared to be if the coin fails the test.

If we denote "fair" as negative, and "unfair" as positive, we say (in statistical jargon) that Test A has a false positive rate (where the coin is actually negative, but we say it is positive) or a Type I error of 5.4%. Test B has a Type I error of 1.1%.

## Assymetrical Hypotheses

Similarly, if the the coin is actually positive ("unfair"), but we say it is negative ("fair"), we say there is a Type II error, or a false negative.

So what are the Type II errors of the tests? Or in other words, if we conclude that the coin is indeed fair, what is the chance that it might be unfair? But when will we actually say that the "coin is indeed fair"?

Now, if the coin failed the test, we had reasonable confidence that the coin was not fair, because most fair coins pass the test. But can we say the opposite? That, if a coin passed the test, we have reasonable confidence that the coin is fair, because most unfair coins fail the test? We can't say this because we don't know if most unfair coins pass the test. In fact, we know nothing about unfair coins. To know, we would need exhaustive answers to Question 1 and Question 3.

Instead, we deal with the problem of unknown Type II errors by making an assumption, and a very strong one at that: We assume that most coins are fair.

This leads to the following reasoning:

* Most coins are fair.

* Hence, it is unlikely that we will encounter unfair coins.

* Hence, it is even more unlikely that we will encounter unfair coins, and they will pass the test.

* Hence, Type II errors are unlikely.

* Hence, we don't care about Type II errors.

* Let's get back to doing real statistics, without wasting time philosophising...

## So is our coin fair or unfair?

I don't know. I can only say two things:

* Most fair coins pass Test A. Our coin failed Test A.Therefore, our coin is probably unfair. But there's a 5.4% chance that I'm wrong.

* Most fair coins pass Test B. Our coin passed Test B. Our coin is probably fair, because most coins are fair. But there's a chance that I'm wrong, because I know nothing about unfair coins, and if they pass Test B.

Maybe our coin is fair in some worlds, and unfair in other parallel worlds. I don't know. Perhaps, we will never know.

![Image](https://cdn-images-1.medium.com/max/800/1*JUqbxEphlNsDEum9YBYgnw.jpeg)

#### Article 99 · September 14, 2019

# Free from Freedom

### Freedom, Unfreedom and Beyond

The OED defined freedom as:

>>> "The power or right to act, speak, or think as one wants."

What one wants means differs from person to person and situation to situation and might be contradictory. For example, if you were an ISIS terrorist, what you want might be the freedom to set fire to Jordanian airforce pilots. But if one were a Jordanian airforce pilot, then what you what might be the freedom not be set upon the fire. Hence, freedom is always relative to the subject (e.g. ISIS terrorist, or Jordanian airforce pilot).

Just as individuals have individual notions of freedom, collections of individuals (e.g. countries) share (or claim to share) collective ideas of freedom. Sometimes these notions are codified into law. For example, the First Amendment to the United States Constitution codifies the concepts of freedom relating to religion, speech, press, assembly and petitioning:

>>> "Congress shall make no law respecting an establishment of religion, or prohibiting the free exercise thereof; or abridging the freedom of speech, or of the press; or the right of the people peaceably to assemble, and to petition the Government for a redress of grievances."

## From Freedom to Unfreedom

Suppose you believe in the freedom to practice a religion of your choice. How would you apply this freedom to a religion X that requires that people should not have the freedom to follow other religions? And that the followers of X should have the freedom to persecute adherents of other religions?

There is a paradox here. On the one hand, if you don't allow people to follow X, you betray your belief in freedom of religion. On the other hand, if you allow people to follow X, then you implicitly support the suppression of religions and thus again betray your belief.

How might we get around this paradox?

We could add a "Do not treat others in ways that you would not like to be treated" (a form of Golden Rule) clause to all religions, and those religions (like X) that don't conform, are not afforded the protection of the law.

This solution is a form of regulation: we subject all religions to a rule "Do not suppress other religions" so that freedom of religion can be maintained. But regulation in particular, and rules, in general, are a form of unfreedom. They take away the power and right to act, speak and think.

Hence,

>>> No set of freedoms is viable, without a corresponding set of unfreedoms.

## Beyond Freedom and Unfreedom

Is unfreedom the opposite of freedom?

Consider our ISIS terrorist and the Jordanian pilot. The former's freedom was the latter's unfreedom. And the former's unfreedom was the latter's freedom. Hence, in many ways, the difference between freedom and unfreedom is subjective and individual. Was the Jordanian airforce pilot being set on fire any different from a set of ISIS terrorists burning alive after an airstrike with the complements of the Jordanian airforce? Would the pain felt by one human burning at very high temperature, be significantly different from that felt by another facing a similar predicament?

Hence, the opposite of freedom cannot be unfreedom because freedom is unfreedom. And unfreedom is freedom.

But then what is the opposite of freedom and unfreedom?

Let's consider the definition of freedom more closely. What one wants is a hope for the future. The ISIS terrorist hopes for a future where the Jordanian pilot is burnt alive. The pilot, on the other hand, hopes for a future where he is alive and unburnt.

Hence, the opposite of freedom is not having hopes for the future. Note, this is not despair, which is the belief (or even hope) that the future will be bad and negative. Nor having hopes for the future is purely a matter of accepting that the future is uncertain, unpredictable, and unknowable, and there is no point in having specific hopes for the future.

Hence,

>>> True freedom is being free of the need for freedoms.

## Concluding question?

Zooming back from abstract philosophising to the concrete real world, where does this get us? Are their any needs for freedom we can give up?

>>> What freedoms might we give up so that our lives might be lighter and happier?

I'll leave these questions as an exercise to the reader.

![Image](https://cdn-images-1.medium.com/max/800/1*ypiUfVtQljw65iEE9yfwGQ.jpeg)

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