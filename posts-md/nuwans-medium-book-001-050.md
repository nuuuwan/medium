# Book 1

#### Articles 1 to 50

#### Article 1 · January 1, 2018

# Reinventing the Wheel

![Image](https://cdn-images-1.medium.com/max/800/1*uelROBkMlKDIomBaa1kK9w.jpeg)

I write code. And so often when I write code, I'm compelled almost instinctively to re-write code that already exists. Suppose I need to extract some text from a PDF. There is a wide range of software which can do this well. But my first instinct is to try and rewrite this software from scratch.

While some of my fellow computer scientists, software engineers and coders are surprised, sometimes even critical of this behavior, others have confessed to being tempted to do the same thing.

## Problem

I've been reflecting on why I do this, and there are a couple of explanations.

1. Understanding. Rather than understand how the 3rd party code works, I'm tended to write my own code so that (at least in theory), I'm guaranteed to understand the code. The cost of writing an application from scratch is almost always greater than the cost of reading through the 3rd Party code and understanding it — but irrationally, this doesn't seem to factor in.

2. Security. This is a special case of understanding, where I'm worried about the question, "will this code behave in some strange way?"

3. Code Quality. I'd like to write code and maintain its quality in a certain way. This is as much about format and style, as it is about quality. Any new code will just pollute my code base. Hence, rather than take pains to merge something new into my code, I re-write.

4. Control. If I write this code from scratch, I'll be able to modify it, and control it more effectively. Particularly for open source libraries, this is also a combination of 1) and 3).

I've considered the following solutions to my problems.

## Solution

1. Understanding. Writing code is a laborious way of understanding it. A process that takes so much longer than reading the code. However, it not completely without advantage. Writing is an active activity, while reading can be more passive. Hence, making code reading more active will help with understanding. I often make extensive notes of the 3rd party code base, often drawing charts and diagrams.

2. Security. This is a legitimate question, but most 3rd party software is likely to be as secure as some proprietary software we seldom question (like Mac OSX which I'm writing on my personal computer right now).

3. Code Quality. If the style, format and quality of the 3rd party software is significantly out of sync with my own code base, I would wrap it in a wrapper library, which will make its interface look more like what I'd expect.

4. Control. My "hacks" for understanding help here. Additionally, I try to think of ways in which I can extend and modify the 3rd party software — forcing me to think of ways in which I can control and exploit the code.

#### Article 2 · January 3, 2018

# Fragile Employees vs Fragile Companies

In August 2015, the New York Times, published "Inside Amazon: Wrestling Big Ideas in a Bruising Workplace.". The following excerpt reasonably summarizes the whole:

>>> "Even as the company tests delivery by drone and ways to restock toilet paper at the push of a bathroom button, it is conducting a little-known experiment in how far it can push white-collar workers, redrawing the boundaries of what is acceptable. The company, founded and still run by Jeff Bezos, rejects many of the popular management bromides that other corporations at least pay lip service to and has instead designed what many workers call an intricate machine propelling them to achieve Mr. Bezos' ever-expanding ambitions. "This is a company that strives to do really big, innovative, groundbreaking things, and those things aren't easy," said Susan Harker, Amazon's top recruiter. "When you're shooting for the moon, the nature of the work is really challenging. For some people it doesn't work." "

![Image](https://cdn-images-1.medium.com/max/800/1*XN7Xh3ey3zbnOTPS-crK-Q.png)

The piece was seen by many as been a "dystopian expose". Jeff Bezos sent a memo to Amazon employees, including (among other things) the following rebuttals.

>>> "The NYT article prominently features anecdotes describing shockingly callous management practices, including people being treated without empathy while enduring family tragedies and serious health problems. The article doesn't describe the Amazon I know or the caring Amazonians I work with every day."

>>> "The article goes further than reporting isolated anecdotes. It claims that our intentional approach is to create a soulless, dystopian workplace where no fun is had and no laughter heard. Again, I don't recognize this Amazon and I very much hope you don't, either"

### Antifragilty by Layers

![Image](https://cdn-images-1.medium.com/max/800/1*qpa9HjxQ3qJ9WhqjUEXpkA.png)

I have not worked at Amazon, and while I have heard many anecdotes from friends and colleagues on the pros and cons of Amazon Culture, I don't feel qualified to judge if the "little-known experiment in how far it can push white-collar workers" has succeeded or failed. However, it did remind me of this quote from Antifragile: Things That Gain From Disorder by Nasim Nicholas Taleb:

>>> "This chapter is about error, evolution, and antifragility, with a hitch: it is largely about the errors of others — the antifragility of some comes necessarily at the expense of the fragility of others. In a system, the sacrifices of some units — fragile units, that is, or people — are often necessary for the well-being of other units or the whole. The fragility of every startup is necessary for the economy to be antifragile, and that's what makes, among other things, entrepreneurship work: the fragility of individual entrepreneurs and their necessarily high failure rate."

In the book, Taleb introduces antifragility as follows:

>>> "Some things benefit from shocks; they thrive and grow when exposed to volatility, randomness, disorder, and stressors and love adventure, risk, and uncertainty. Yet, in spite of the ubiquity of the phenomenon, there is no word for the exact opposite of fragile. Let us call it antifragile. Antifragility is beyond resilience or robustness. The resilient resists shocks and stays the same; the antifragile gets better"

The relationship between the fragility and antifragility of various layers of a system, is a common theme in the book. The key premise is that fragility at one layer, promotes Antifragility one level higher, and vice versa. For example, Taleb talks about how fragile start-ups makes for an antifragile start-up ecosystem in Silicon Valley, while conversely, how antifragile too-big-to-fail banks, led to a fragile banking system during the 2008 financial crisis.

### Antifragile Companies

The "Amazon Experiment" (For the rest of this note, I'll use the term "Amazon Experiment" to refer to the picture painted by the New York Times, and not necessarily reality) could be caricatured as "maximizing employee-layer fragility, to maximize company-layer antifragility". One could argue that if achieving the companies mission is the top-priority, then doing everything possible to maximize company-layer antifragility, which might necessarily involve maximizing employee-layer fragility. In this light, the stresses, pressures and "Nearly every person I worked with, I saw cry at their desk."-type culture seems reasonable, even optimal. Through one lens, this almost sounds like to argument the NYT is trying to make.

![Image](https://cdn-images-1.medium.com/max/800/1*d2xTS8p4gFlEaRS_Vq0dRA.png)

However, I find this argument weak, for one simple reason: There are other ways of achieving company-layer antifragility. While overly stressing employees might work, why adopt a draconian strategy, when softer strategies might exist?

Two of my favorite company-layer antifragility strategies are Teams and (what I'd like to call) "Kicking fragility downstairs".

### Teams

Teams seek to balance competition with cooperation. Teams of employees working together to achieve common goals are more antifragile than individual employees who might be forced to compete unnecessarily with other employees. To frame this in "Antifragility-by-layers"-speak, we shelter all employees in a new layer known as a "Team" which is less fragile.

![Image](https://cdn-images-1.medium.com/max/800/1*sTcg0LNq_WvT_vRnXVHAiQ.png)

Now, in some cases, teams can be too antifragile, leading to the company as a whole becoming fragile. Often teams and broader sub-organizations become too powerful, political, and start behaving in ways that are counter to the company's overall interests. Sometimes the company consists of many such teams which are locked in machinations and mutual distrust.

![Image](https://cdn-images-1.medium.com/max/800/1*lVa7hmQjrtKMO73TKAmd9Q.png)

Hence, some constraints are needed to ensure the right balance is reached. For example,

* Common Goals. Teams should have goals and missions which are closely aligned with the company's overall goals and mission. This is a top-down way of constraining what a team does to things that are acceptable to the company as a whole.

* Communication. While things like "mission" and long term "vision" are common across companies, and are communicated top-down, it's more efficient that shorter term strategies and tactics are framed at the grassroots level. However, these tactics must also be aligned across teams, and inter-team communication is vital for this.

* Small Teams. One obvious way to prevent antifragile teams that lead to fragile companies is to make sure that no team is too big. However, with many questions of "small is good", the challenge to make teams as small as possible, but not too small.

### Kicking fragility downstairs

An alternate approach is to move fragility down a level from employees to something else. But to what? The sometimes chastised adage "Move fast and break things" offers some clues.

In its most generous interpretation, "Move fast" simply means that employees can operate in a efficient manner, while minimizing time and resource wastage. A corollary of "Move fast" is "Fail fast" — or an environment where employees experiment, try things, understand what works and what does not, and move on to the next thing quickly. "Break things" implicitly implies an environment where an employee can break things without actually breaking things — or in other words, there are safeguards against the consequences of moving fast — experiment at low cost.

![Image](https://cdn-images-1.medium.com/max/800/1*q-U8iJLMtuO-ZUhKPKFeow.png)

In other words, a "Move fast and break things" culture and environment, enables employees to be antifragile, by moving fragility down to the level of processes and experiments. In such a world, an employee can succeed by failing 99 times, and succeeding once. As opposed to a "Move slow, and don't break things" world, where they are fired for failing once.

### Concluding food for thought

Hence, there are some reasonable ways to mitigate Company-Employee Fragility tensions, without too much pain. Let me end with describing a tension one level higher.

The Herfindahl-Hershman Index (HHI) measures the level of inter-company competition in an industry. It's computed as follows: First, for every company in the industry, we compute its market share as a percentage; Second, the squares of these percentages are summed-up to give the index.The higher the HHI, the less competitive the industry. For example, an industry where one company has an absolute monopoly (i.e. a 100% market share), has an HHI of 10,000. An industry where two companies dominate equally (i.e. with 50% market shares each), has an HHI of 5000. A highly competitive market with 100 companies each with an equal market share of 1%, has an HHI of 100.

Many tech giants dominate their industries. For example, Google boasts nearly 80% of the Desktop Search, leading to that industry having an HHI in excess 6,000. Applying some of the principles discussed above, we might conclude that overly antifragile companies will lead to fragile industries. This is probably a much bigger fragility problem.

![Image](https://cdn-images-1.medium.com/max/800/1*G6_kPn38esdMDpsbH2ZXMA.png)

Bon Appétit!

#### Article 3 · January 8, 2018

# Markets, Managers and Beyond

In 2016, a UK employment tribunal ruled that Uber drivers should be classified as workers with minimum-wage rights. Uber appealed this ruling, which they subsequently lost in November 2017. What I found interesting about this episode, was less the legal battle, and more one particular implication of classifying Uber drivers as Uber Employees.

![Image](https://cdn-images-1.medium.com/max/800/1*K2J2EY_7344Mt1h1qNzceA.png)

Until now, all employees at Uber (except, possibly the CEO), have a designated human manager. Uber drivers, on the other hand, are completely "managed" by the market forces, and the systems that try to predict and simulate them. It is supply and demand for rides, rather than some human agency, that determines what management they get. Hence, the ruling implies that Uber (at least theoretically in the UK) now has two types of employees: 1) those managed by humans, and 2) those managed by the market.

![Image](https://cdn-images-1.medium.com/max/800/1*8nP3WXaBPS0kx0f3wr040w.png)

This led me to ask:

* QUESTION 1: While, the connection to a market is very clear in Uber's business, in reality, all workers work in some market for goods or services or both. If so, can all workers be "managed by the market" via some automated system?

* QUESTION 2: If not, it must mean that managers provide some unique and meaningful value addition — which the workers cannot obtain by "observing" the market themselves. This understanding this value addition is existentially important to "management" as a profession. What is this value addition?

To try and answer these questions, I thought about my profession (Software Engineering/Computer Science) and field (Web/Tech), where I have played the role of both a manager and a non-manager.

### A "Market Driven" Tech Company

Software Engineers (like me) design and build software systems. We (Software Engineers) also test these systems and maintain them. We fix bugs, and add new features. In a traditional Tech Company, engineers will be "told what to do" (to various degrees of specificity) by their manager, or one or more people playing a project management role. A junior engineer might be asked to work on a specific task — sometimes, having the specifics of how to accomplish it spelt out, quasi-verbatim. A more senior engineer, might be just given a broad problem-sketch, possibly with no known solution. In this sense, a senior engineer might not be explicitly told what to do, but implicitly assigned an area, within which they are expected to find meaningful problems and solve them. But either way, the engineer (junior or senior) receives some guidance (explicit or implicit) about what needs to be done — usually from a human manager.

[NOTE: In reality, a tech company needs workers in many other roles (Product Managers, Product Designers, Data Scientists, Researchers, Content Strategies...the list is very long) -not just Software Engineers. For clarity, I'll only refer to the software engineer role in this thought exercise. The ideas and conclusions are easily extensible to other roles]

How might this process of guidance look like in a "market driven" Tech Company?

To start with, what is the "market"?

One way of thinking about a market, is to think in terms of problems to be solved. There is a "supply" of problems, which "demand" that engineers solve them. In a typical engineering problem, a senior engineer will take a broad problem, and break it down in to smaller problems. One or more of these tasks might be assigned to other engineers, who might directly work on them, or recursively break them down and assign them to further engineers.

![Image](https://cdn-images-1.medium.com/max/800/1*EL9fpmqUFVYwM7XS1M35kA.png)

A large problem broken down into smaller problems is more "valuable" than the original large problem, because it's possible to solve it with less effort. This difference in value is the "contribution" of the senior engineer performing the break-down. Similarly, solved problem is more valuable than an unsolved one — and this difference is the contribution of any engineer (junior or senior) who solves it.  [NOTE: By "seniority", I mean competence and skill, and not tenure or age. Also, my separation of senior and junior is somewhat arbitrary and black-and-white. Most companies have several "levels" of engineers. But for the purpose of this note, this crude separation should suffice.]

Now, suppose we actually built a system (as in a computer system) that "connects engineers with problems" the same way Uber connects drivers with passengers.

We would have one database with engineers, and some data which would help determine what sorts of problems they could work on. We would also have a database of problems. Initially, the database would have only one problem, say "Organize the worlds information, and make it universally accessible and useful" (let's call this initial problem, the "Mission Problem"). Also, initially, the company would probably be small and have a small number of employees — say 2. Let's call then Page and Brin.

Suppose, the system (magically) decided to assign Page the "Mission Problem". Page breaks the mission problem into two problems:

* Organize the information on the internet, and make it accessible and useful, and

* Organize all the other information in the world, and make it accessible and useful.

Page and Brin, decide to tackle Problem 1 first (say, because it's easier, or more "impactful"), store Problem 2 in the database for future retrieval, and start working on Problem 1.

![Image](https://cdn-images-1.medium.com/max/800/1*4sPXC7keoARcB_6XkWyM0A.png)

Let's take a closer look at this magical "system" which is connecting problems with Page and Brin. What functionalities must it have?

* It must "understand" and store information about problems

* It must "understand" and store information about engineers

* It must know how to assign which problems to engineers

* It must know how to evaluate the solution, and how much to reward or rebuke each engineer for a particular good or bad solution.

### QUESTION 1: Can all workers be "managed by the market" via some automated system?

The answer to this question depends on whether some automated system can satisfactorily possess the above qualities. I'm going to avoid directly answering this question just now, because I'm less interested in whether some magical AI system can satisfy these qualities, and more interested in what us humans might learn from this thought experiment.

The first and most obvious learning is that human managers should also possess all these functionalities. To rephrase each quality as "human" functions:

* Managers need to clearly understand the mission of the company, how it relates to the organizational subset they operate in, and how that mission decomposes into specific problems.

* Managers need to clearly understand their people. This might seem obvious, but I want to stress this point, because verbs like "enabling", "supporting", "optimizing" and "leading" tend to get more emphasis in management practice, than "understanding", which is a necessary pre-verb to all of these.

* Managers need to have an efficient process of mapping people to problems (Read "problem" as a general term for "task", "project" etc.)

* Managers need to accurately evaluate their people, evaluate performance, and manage performance.

To me, these four qualities seem core manager functions.

My second learning is that these qualities are not uniquely manager tasks. For example, all employees should be expected to understand the mission of the company, and how it relates to the specific problems they are individually solving. They should also be expected to have self-awareness (i.e. understand themselves), and manage their own performance to various degrees. Employees often also participate in the understanding and evaluation of their peers.

My third learning is that the process of executing these qualities also leads to generating meta-problems. For example, just as achieving a company's mission is one problem, making sure the company has the right employees to achieve that mission is "emergent" meta-problem. Some of the most interesting "manager problems" are such meta-problems.

My fourth learning is that even if we had a magical system that juggles problems and people, whenever there is a market, people find interesting and complex ways to interact with that market. One such "complex behaviour" is how people collaborate. For example, several engineers might decide to collaboratively work on the problem. Their interaction might be ad-hoc and organic. Maximizing positive ad-hoc and organic behavior is, in turn, an interesting "meta-problem", and one that many organization give a lot of attention.

But back to Can all workers be "managed by the market" ?

Assigning passengers to drivers is a lot simpler that assigning problems to engineers, particularly given the complex way humans behave. My guess is that it would be easier to build an artificial system that write codes, as opposed to one that manages humans that do. Rather than spend more time on this question, let's move on to the next one.

### QUESTION 2: What is this value addition of managers?

Before, answering this question, what or who exactly is a "manager"?

Here are a couple of candidate definitions:

* People who are expected to perform the four core manager functions (described above)

* A person with a job title "manager", and has a set of duties, responsibilities, rights and privileges associated with that employment title.

* Someone who is responsible for larger set of problems, relative to other employees

* A person who specializes in solving people problems, as opposed to technical problems.

There is some degree of "trueness" to all these definitions.

However, individually, each definition is problematic.

* The problem with 1) most employees perform one or more of these functions to some degree. In that sense, everyone is a manager.

* The problem with 2) is that it refers more to a designation, and less to expectation. And without expectation, it is hard to evaluate value addition.

* 3), like 1) is completely role agnostic.

* 4) is probably the most accepted and agreed-upon definition of "manager". However, for me, it has the serious problem that in most cases the best managers need to balance their people and technical specialities, at times flexing technical muscles, and at other times people ones. Hence, a true and absolute specialist in one or the other would be a poor manager. Also, the duality of "People" and "Technical" is somewhat arbitrary, and does not exhaustively cover the types of things a manager should do.

Hence, I don't have an answer to QUESTION 2, because without defining what a manager is, it can't be satisfactorily answered. Instead, let me cheat and try to dance around the question.

### Beyond Managers?

In Automate/Informate: The Two Faces of New Technology, Shoshana Zuboff describes the effect of new technology on the historical role of the manager as follows:

>>> Managers have traditionally been considered the representatives of ownership. Only they could be countered on for the loyalty and dedication that this symbolic investment of property rights implied. It followed that significant information could be entrusted only to those who could be relied on to serve the interests of ownership. But the informating process unleashed by new technology can provide the nonexempt worker at the information interface with access to data that convey a broad scope of the organization's functioning.

...

>>> For middle managers who measure their worth in terms of their ability to exert control and maximize the certainty of out- comes, the choice to create "smart people" can be a threat. Even those willing to consider the obsolescence of their traditional function can find the ambiguity of their emerging role painful enough to elicit resistance.

>>> As one manager explained, "As we face change, the big issue is, ‘What's in it for me?' If I can keep the box narrowly defined, then I know my worth as a manager. I don't know what my new skills will need to be, so that is uncomfortable."

Hence, traditional "middle-management" relied on managers holding a monopoly over information, which enabled them to direct workers. This role was undermined as information became more broadly accessible.

Many companies have already moved away from managers who are information gatekeepers and controllers, to one in which they mostly provide the core manager functions that I describe above. But as I explained earlier, the problem with this new job description is that it is not unique to managers.

Is it time to move beyond the role of the "manager"? At least in tech companies where information is freely available and sharable, this seems feasible. Should companies be organized purely based off what subset of problems people are working on, and what volume of problems each individual is responsible for? In such a model, each there would still be levels of seniority, and even hierarchies of employees, based on who is responsible for what "people meta-problems" but no separation of managers and non-managers.

![Image](https://cdn-images-1.medium.com/max/800/1*zl5vT4nm0v25lEF7eIp74w.png)

#### Article 4 · April 1, 2018

# Classification Algorithms, Elections and Electoral Metaphors

### Including "What is democracy analogous to in the Machine Learning discourse?"

![Image](https://cdn-images-1.medium.com/max/800/1*oZEcwIj9LoNj-64W-satnQ.png)

A classification algorithm assigns some observation to some class of things. For example, given an email (the "observation") a spam detection algorithm could determined if it should be classified as spam or not-spam (the two "classes"). The algorithm will use various attributes of the email (e.g. who sent it, the text in it, what time it was sent etc) to determine which class it belongs to. These "attributes" are known as "features".

In elections, people vote to choose an individual to hold political office. The Electoral System determines how the aggregate votes are used to determine the winner. For example, the recent UK parliamentary election uses a "First-past-the-post" system, while Sri Lankan parliamentary elections use proportional representation.

Elections are analogous to Classification Algorithms. The observation is a single election. The features are the people voting. And the class selected by the algorithm, is the winner of the election.

Here is a list of some well know Classification Algorithms and Concepts, as "Electoral Metaphors". For readers familiar with Basic Machine Learning, I'll leave it as an amusing exercise for you to guess what these might be. If you're not, you could reflect on how Electoral systems have many things in common with Machine Learning algorithms — even when these commonalities might not be desirable.

* The election has exactly two candidates. Different people have different numbers of votes. People determined to be more likely to pick the "right" winner have more votes. "Right" means "likely to be successful based on past elections". Some people who are known to consistently pick the wrong candidate have "negative votes". Each person assigns all there votes for one of the candidates. Finally, all the votes are added up, and the candidate with the most votes wins. In some instances, one candidate might get some "bonus votes", if they are determined to be more suitable, irrespective of what the voters thing.

* The election can have two or more candidates. First, the person deemed most likely to pick the right winner votes. The election might end at this point, if "the system" is confident enough that the person got it right. If not, another person gets to vote. Exactly, which person gets to vote next might depend of how the previous person voted, and based on which next person is most likely to pick a winner "rightly". So, the order in which people vote might change depending how the people before them voted. This process continues until the system is sure of the candidate. As is evident, often not everyone gets to vote, as the election might be already decided before it's there turn to vote.

* In some systems, the number of people who get to vote in an election is artificially constrained to a small number. The assumption is that if too many people vote, the election will be made complicated by too many considerations and issues, and might not lead to the most "optimal" result (whatever that means).

* The election can have two or more candidates. The people don't initially select the final candidates, but select a set of proxy candidates, who will then vote on their behalf. These proxy candidates might then vote for the final candidates, or might, alternatively, vote for and select another set of proxy candidates. As with 1), both the initial voters and the proxy candidates might have unequal numbers of votes, which are determined according to who is most likely to pick the right candidates.

* The election can have two or more candidates. From all the people eligible to vote, a sub-group is selected at random, asked to vote, and the winning candidate for the sub-group is chosen. This process is repeated for many sub-groups. Each sub-group is then analysed for how well they might pick the "right" winner, and assigned a weight — with some subgroups having a higher weight than others. Finally, the winner is determined by the candidate who wins the most number of sub-groups, weighted by each subgroup's weight.

* In electoral systems where people are allowed to have unequal numbers of votes, we might want to restrict the amount of "unequalness". Because, if political power is too unequal, them the results of elections might be meaningless or even harmful. So sometimes we force each person to have at most only some number of votes over the mean number of votes per person.

* In some electoral systems, people don't vote for candidates, but vote for a list of political propositions — aligned with their political beliefs. Each of the candidates promise to carry out various political propositions. The winning candidate or candidates, are those whose political promises are most similar (or, as is referred to in the trade: "nearest") to those picked by the people.

* People don't vote. Instead, a subset of them are selected to be political candidates at random. The candidates then discuss their political opinions and form groups of like-minded people. The group with the largest number of people governs.

* Elections can get complicated when too many political issues are actively under discussion (security, immigration, taxes, education, healthcare etc). Hence, sometimes opinions on different issues are bucketed, into single groups. For example, if most people who favour higher taxes on the rich, also favour free universal healthcare, the two issues can be bucketed into "the High Tax and Free Healthcare" bucket. This process can be extended until the many issues and opinions, are minimised into a small set of lobby groups. Care is taken to ensure a manageable number of buckets.

#### Article 5 · April 1, 2018

# Emancipating Humbots

![Image](https://cdn-images-1.medium.com/max/800/1*kQT_d5RwMSiNDJEOx-g0mw.jpeg)

### Taylorism

In her 2001 article, "Automate & Informate: The Two Faces of Intelligent Technology", Shoshana Zuboff cautioned against the pitfalls of focussing solely on automation, and proposed a better balance between Automating and "Informate-ing" (which — roughly — describes the process of humans creating new information and product from analyzing and manipulating data). She discussed various deficiencies of automation, particularly those arising from its Taylorist roots. She also speculated on whether some of the newer (at the time) tech organizations would inherit this Taylorism or whether they would embrace informate-ing (as opposed to automating).

Frederick Taylor's ideas of scientific management, focussed on increasing labour and capital efficiency and productivity, and hence, profits. They involved identifying the most optimal process for carrying out various tasks, and defining manufacturing flows accordingly. This led to human assembly lines where workers performed mundane, and repetitive tasks at high speed. The workers were essentially human robots ("Humbots")

This Taylorism led to a new class of worker: the manager or "boss". Unlike the "worker", who had a single repetitive task, bosses had complete visibility into the factory, and what might improve its processes. They also had the authority to command and control workers, such that these processes were performed optimally. Bosses were considered "part of the organization" or "insiders" as they had ownership of processes, and could be considered loyal to the organizations aims.

With progress in technology, the human assembly lines were increasingly replaced by machines — a direct substitution of capital for labour. This aggravated an already tense relationship between workers and the organization. Workers increasingly saw their role as undignified, and temporary until the organization found some way of automating Humbot work into robot work.

### Happy Employees

The open plans offices of, say, Google or Facebook, look nothing like the factory assembly lines described above. All around, one sees smiling faces pampered with free food and other perks. Unlike the workers who were commanded and controlled to do a specific set of tasks, modern tech employees operate in flat organizations where (often) no boss tells them what to do, and they are asked to pursue whatever cause that best achieves the companies "mission". They are driven by uplifting maxims like "nothing is someone else's problem" and "Don't ask for permission" — implying that they can do anything. They are their own bosses to the fullest.

The freedom of tech employees goes even further. There are few restrictions to how employees can use the companies data, and as a result have the opportunity to try out new ideas, and build new products that might utilize this data. Many wildly successful products have emerged from a small number of employees taking some data and seeing "what they might build around it". Hence, Zuboff's idea of "Informating" is probably most vibrant and successful in the modern tech company. And similarly, no place is further from the Taylorism command and control assembly line.

However, there is another, darker side.

### The Modern Humbot

I'm going to use Google as a guinea-pig, but my observations apply to many data-centered tech companies.

While the mission of Google is "to organize the world's information and make it universally accessible and useful", in practice, it's core business (currently) is manufacturing. It manufactures ad impressions (which account for most of Google's revenue).

Ad impressions are manufactured by two classes of Google employees. The first class of employees spend large amounts of time on Google properties (Google Search, YouTube etc, Shopping), performing various actions (searching, watching videos, buying things). The second class of employees build systems that make sense of these actions, and build more products that will help the first group of employees perform more actions.

Google treats the two classes of employees very differently. It is the second class that I described above as empowered, pampered, and happy.

The first class of employees, are not even officially referred to as employees. They are varyingly referred to as "community" or "people", and in a few situations "customer". The organization often reminds these employees on how lucky they are on getting a service for free — conveniently hiding how valuable they are to the company (not necessarily individually, but immensely in aggregate), or the darker truth that they are actually modern reincarnation of the Humbot.

The lot of the modern Humbot is terrible. It works for free. It is completely expendable, as millions of its kind are waiting to take its place. The slightest disobedience of the boss, results in dire consequences.

This is the dark paradox of many modern tech companies. They have two classes of employees: One class, which enjoys high remuneration, and intellectual freedoms, and largely operates in a post-Taylorist, enlightened informate-friendly and informate-heavy micro-organization. This is conjoined with a vast heard to Humbots which forms a Neo-Taylorist macro-organization where automating out-dominates informating.

### Ending Neo-Taylorism

In "Automate & Informate: The Two Faces of Intelligent Technology", Zuboff recommended that a Informate-friendly organization needs to 1) empower employees to take action based off data, and 2) provide them with the necessary skills, training and education to do this satisfactorily. There is a third, implicit requirement, which is that these employees should also have access to the said data.

The only way to end Neo-Taylorism in tech macro-organizations is to transform it into a more informate-friendly form. For example, what if Google Search could be transformed into its true role as an organizer of information, and all of its search indexes and people information is broadly shared)obviously with the appropriate privacy and security controls)? Google becomes, not an advertising company, but an infrastructure company, with millions of other developers building new products on its infrastructure.

There are obvious barriers to this approach. Bosses, or "Middle Managers" as Zuboff described them, have always resisted informating. In automation-heavy organizations, the boss has a privileged positioned, endowed with exclusive access to information, the support of the organization as a loyal employee, and one who has rights to command and control. The "employee" in a tech micro-organization enjoys almost identical privileges, and where "command and control" involves almost infinite flexibility on how Humbots are treated. Hence, extending informating outside the micro-organization and into the macro-organization democratizes privileges that a small elite enjoyed, and that elite will resist it.

### Silver Linings

Many have proposed building informate-friendly, often "open" versions of tech giants. However, given the level of market monopoly that many tech giants enjoy, this is going to be near impossible. The failed attempts by Bing and Google+ to topple Google Search and Facebook respectively, demonstrate how hard it is, even for giants to slay giants. Hence, "building a new version of X" is probably not going to work. Others have hoped that governments will break monopolies through anti-trust regulations — though, the enormous lobbying power of giants makes these efforts usually impotent. Also, half a giant is usually still a giant — so splitting a Google into two, will hardly solve the problems expressed above.

There seems to be no obvious solution for existing products. However, there might be some hope for new products.

What if all new products are designed such that data is distributed across the macro-organization instead of a small micro organization? What if data is, by design, distributed? And control free for all the nodes in this giant graph? The obvious downside of this approach is that no single entity will have exclusive access to data, and hence will not become a giant like today's modern tech giants. On the other hand, this system would be far more beneficial to the majority.

While today's modern tech-giants are the fruits of capitalism, they are themselves highly anti-capitalist. They stifle free markets and thrive on monopolies and anti-competition. They hoard and hinder the movement of the most important form of capital: data. An informate-friendly distributed market is the ultimate free-market of data. It is the ultimate form of capitalism. And surely, the best future for humanity.

#### Article 6 · April 1, 2018

# Every thing we think is wrong. And that's ok.

![Image](https://cdn-images-1.medium.com/max/800/1*Kr1tTsOfpKQPaSS5r8GzCg.png)

>>> "All models are wrong, but some are useful" — supposedly said, George Box.

The world we perceive is a model — constructed by our brains. For example, while we think we can "see in real time", that "realtime streaming video" is actually constructed from a set of still snapshots (about 10 per second), and then expertly stitched together by our brain — creating an illusion of continuity. All models are always incomplete, and often inaccurate — which is what I meant by "wrong".

So, if all models are wrong, and our perception of the world is a model, everything we think and feel is wrong. But happily, as Box implied, some things we think are also useful.

Let's now pause for a cup of tea.

### Little Tea Leaves

If you, like me, drink a lot of tea, and you, like me, brew tea directly from leaves, instead of tea-bags (what I call "from first principles"), you'll find that you need to strain the tea. While the bulk of the leaves lodge in the strainer, a few little leaves will escape through its holes. None of the little tea-leaves "designed" to "survive" the strainer. Randomness happened to make them small — and as a result they "survived" the strainer.

We are all tiny tea leaves. We happen to be descended from lucky few who survived the trials of evolution, because we happened to posses the bodies and brains, which, by chance, adapted to survival. Our brains don't create "correct" or "accurate" models of the world, merely ones optimized for survival. Sometimes these models are wrong, but it's still ok.

For example, consider the snake.

### Snake

>>> Slithering serpent. Staring. Beside my bedside. In shadow. A belt.

Recently, I mistook a belt for a snake. This is not surprising. Given the choice of I) mistaking a belt for snake vs, II) mistaking a snake for a belt, my survival optimized brain would much prefer the first type to the second (Statisticians refer to rejecting the benign hypothesis incorrectly as Type I Error). If my (and your) ancestors had the type of brain that mistook snakes for belts (assuming that early humans on the African Savanna wore belts), they would not have survived, and I (and you) would not be here.

The snake episode is one instance of a pattern. Our brain focuses on a small detail, and ignores the big picture that is (supposedly) less useful. It looks for the slightest characteristic of a snake in a belt, ignoring the other characteristics of the belt (like the fact that, most belts have buckles).

### "Usefulness" Principles

With my snake episode, I gave just one example of a broad set of phenomena known as cognitive biases. If you'd like to learn more about these biases, I'd recommend Rolf Dobelli's The Art of Thinking Clearly, which succinctly describes over a 100. I've also compiled a personal "cheat-sheet" on how to interpret and act, given that "Every thing we think is wrong", which (happily) attempts to make some things useful.

Curiosity

While most things our brains tell us are mostly inaccurate, they also have nuggets of usefulness. When we are alarmed by something that looks like a snake, our brains are actually telling us "there is a small probability that this might be a snake". By being curious, observant, inquisitive, and open to ideas we can expose ourselves to as many such nuggets. While there is a lot of noise, there is also some signal — and so it's useful to get comfortable with noise. The opposite of curiosity is being boxed into a silo of narrow ideas — like Religious Fundamentalists, Fascists, and "Liberals" (in the US), and Non-Liberals (Rest of the world).

Skepticism

While there might be some signal, there is also a lot of noise. Hence, its prudent to be skeptical about what we think, what others think, and what we think others think. I'd be highly skeptical of people who "read too much" into their thoughts, observations, ideas, planetary positions, or tea-leaves, or prematurely jump to conclusions — like Astrologers, Journalists, European Doctors in the late 10th Century, and Economists (both European and otherwise) in the 20th Century.

Pessimism and Optimism.

It is easier to carry an umbrella, than it is to forecast rain; as it is to be alarmed by a belt that looks like a snake, than to be bitten by a snake that looks like a belt.

While someone who always carries around an umbrella expecting rain might be described as a "pessimist", this is purely a matter of viewpoint. You could argue that the individual lives in California (like me), where we don't get enough rain, and (like me) loves rain — and walks around with an umbrella (sadly, unlike me), in eternal hope that it is going to rain. Rather than "Pessimism" or "Optimism", a better word is probably "Preparedness" for the unexpected, both fortunate and unfortunate.

A lot more on that in Taleb's Black Swan.

Modesty and Forgiveness.

No one is as good or bad as people think they are.

Given the highly noisy model our brains makes of the world, we probably overestimate both our strengths, and our perception of those in others. Hence, we need to "correct the model" with a healthy dose of modesty. The same applies to weaknesses — we are probably far too harsh on ourselves and as we are on others.

Ajahn Brahm's Two Crooked Bricks is a good parable highlighting this point.

>>> Happy thinking, little tea leaves!

#### Article 7 · April 7, 2018

### Aphorisms

# On Small Plans and Big Plans

![Image](https://cdn-images-1.medium.com/max/800/1*47eKyJD3avxlyboMieKA_w.png)

### Costs, Benefits and Success

* Small plans have small costs. Big plans have very big costs.

* Small plans have small benefits. Big plans have unknown, and possibly non-existent benefits.

* Small plans have a small chance of success. Big plans, with no intermediate validation, have no chance of success.

* It is impossible to know the cost, benefit or chance of success of a plan, with any certainty, for all but the smallest of plans.

### Action

* A plan that has a combination of too high costs, too low benefits, or a too low chance of success, or too much uncertainty about any of these factors, is not actionable.

* Beyond a certain bigness, all plans are non-actionable. They are less plans and more hunches, hopes or dreams.

* It is easy to represent a meaningful problem as an abstract, big plan. But it is hard to decompose a big plan into concrete and actionable small plans.

### Fatality

* There is a maximum cost a business can bare at any time. Any plan that risks exceeding this cost is potentially fatal for the business. Obviously, fatal plans must be avoided at all costs.

* For any plan that has a 50% chance of being fatal, dividing it into 2 sub plans — that each bear half of the costs, half of the benefits, the same 50% fatality risk, and are risk-wise independent — reduces the fatality risk to 25%. With 10 sub plans, the fatality risk is less than 0.1%.

* Hence, in general, a big number of small plans are significantly less fatal, than a small number of big plans.

### Missions and Strategies

* A "business mission" is a very big plan, and hence, on its own, is rarely actionable. Its value chiefly lies in providing a yardstick for measuring the benefit of small plans.

* A "business strategy" is a constrained business mission, which trades-off size for certainty. But too often, most business strategies are also too big, and hence non-actionable.

* It is easier to compose a meaningful big plan from many small plans, than it is to decompose many small plans out of a big plan. This is the biggest problem with big plans. The biggest problem with Small plans is that it is hard to predict what big plan their composition forms (or in other words if they are collectively beneficial).

* Some of the best business missions and strategies are retrospective. They "emerge" from small plans.

### Organizations

* A business can either work on a small number of big plans, or work on many independent small plans. The latter businesses are almost always more successful.

* A manager can either decompose big plans into small plans and assign them to their reports, or create an environment where their reports can work on small plans, and provide feedback on how beneficial and successful those small plans are. The latter managers are almost always more successful.

* Hence, management is more ecology, than zoology.

* The skill of executing a small plan can be wholly measured in terms of the cost and benefit of that plan. The skill of executing a large plan can be only measured in terms of environment and feedback.

#### Article 8 · July 22, 2018

# Japan Reflections

![Image](https://cdn-images-1.medium.com/max/800/1*sesSZhYyxuVh8caVdHFPNQ.jpeg)

A couple of weeks ago, Kanchana and I visited Japan for the first time. To say "we had a good time" is an understatement. Japan was "Food heaven, Jazz heaven, and (especially relevant to me) Train heaven — all rolled into one".

But beyond this material appreciation, the trip also awakened some spiritual curiosity. I was particularly interested in the following observations.

* Non-Individualism. Whether it's through extreme hospitality and politeness, or through the way that everyone seems to blend in, or through the focus for more collective space at the expense of individual space, Japan seemed a deeply non-individualistic culture.

* Formalism. From greetings to dress to how train drivers behave, there is a lot of Formalism. This felt less mechanical and scripted, and more a sense of peace and flow.

* Minimalism. This was obvious not only in art, furniture, food, and design in general, but also in outlook and discussion. A focus on essence, voiding elaboration. An embracing of simplicity and austerity.

* Quality. Every product and service in Japan seemed to be very high quality. It was difficult to find anything that was 2nd grade of shoddy.

Much of this seemed connected and embodied in Japanese Zen Buddhism. I was particularly interested in the concept of Wabi Sabi (侘寂) — which I learnt about after the trip from Marcel Theroux's BBC documentary, and this useful blurb by Alain du Botton. Roughly, Wabi and Sabi are being at peace and appreciating Suffering and Impermanence, respectively.

At the back of my mind, I always felt that there was some common thread linking all these ideas. To say the common thread was "Buddhism" felt partly true, but also felt incomplete. I wanted something more specific.

A couple of days ago, it occurred to me that the following explanation is consistent with the observations:

Non-Individualism, Formalism, Minimalism, Quality and Wabi Sabi are all connected to living through contemplation, as opposed to living through thought.

As I thought about this more, the following contrasts occurred to me.

## The Contemplative Life vs. the Thoughtful Life

* Thought pursues a specific goal. Contemplation has no specific goal. With thought, the destination is more important than the journey. With contemplation it's all about the journey.

* Thought consists of navigating a large set of ideas, until a single idea is reached. Contemplation consists of focusing on a small set of ideas, or one idea — with repetition. [Minimalism]

* With thought, not only is the journey secondary, a shorter (more "efficient" or "optimal") journey is considered preferable. The ability to "think quickly" is better. With contemplation, there are no such constraints on the journey.

* With thought, success depends on efficiently reaching the destination goal. With contemplation, success depends on the quality of the journey. [Quality]

* The results of thought are easier to measure, and often possible to define beforehand. It's difficult to measure and describe the effects of contemplation, and usually impossible to predict.

* Thought is said to be "creative" — "Creative thought". Contemplation, on the other hand, often involves, formal, mechanical tasks (e.g. Observing one's breadth) or formal steps (e.g. walking slowly). These tasks and steps are often scripted and have been used for hundreds of years [Formalism].

* Paradoxically, often it's hard to be creative by trying to "think creatively". More often, mechanical contemplation leads to more creative and better quality results. The subconscious is often better at creativity than the conscious.

* Thought is optimized for "single tasking". It's impossible to think of more than one thing at the same time. Switching between different trains of thought (multi-tasking) is tiring. Contemplating involves sub-conscious multi-tasking. The subconscious is good at multi-tasking.

* Thinking is always focused on our individual identities — even when we are thinking about something outside ourselves or trying to achieve a non-individualistic goal. Contemplation draws us away from ourselves and is unconstrained by our individualism [Non-individualism].

* With thought, success and beauty are precision and correctness. A successful result is robust and constant. With contemplation success is transient, impermanent, and ambiguous. It is appreciated while it lasts [Sabi].

* With thought, there is the constant allure of success; reaching the goal; winning; a perfect destination. There is no such thing with contemplation. There is no goal, and often the journey is difficult, imperfect, and must be peacefully endured [Wabi].

## Disclaimers

* The reader of this note might incorrectly infer that our experience of Japanese culture and society was unanimously positive. This is not the case. Some things we did find alarming, troubling and sometimes disgusting. This note focusses on a subset of our experience; not all of it.

* This note is inspired by Japan, but not a description of Japan.

* When it comes to history, philosophy, neuro-science and religion, I'm very much an amateur and layperson. Hence, internalize the spirit of my writing, if not the letter.

#### Article 9 · August 20, 2018

# Deep Consumption

There is so much information out there — both online (blogs, videos, articles, e-books, music) and offline (books, discussions, concerts). On the other hand, time is increasingly limited. So much information — so little time. How does one decide what to consume and what not to?

I have thought a bit about this question: Sometimes proactively (usually, to find ways in which I might spend my time more wisely); at other times reactively (often, after I have felt that I've "wasted time" watching, reading, or listening).

This note is a set of "guidelines to self" about what information to consume, and what not to. I am sharing with you either because I would like your feedback about it, or because I feel it might be useful to you.

Before I start, a couple of disclaimers. I propose some "models" on how our brain processes information. I am not a neuroscientist and many of these models are not scientifically conceived. They are mostly metaphors to aid understanding. Also, a lot of these ideas are not completely original. I have been influenced by conversations with friends, and books (most importantly, The Shallows, by Nicholas Carr).

## Goals

Let us start with the "why". Before arguing about "what" information to consume, we need to clarify "why" we consume information.

For me, I feel I consume information for the following reasons:

* To Understand. We consume information to understand the world better. This might be as simple as looking-up the definition of a word in a dictionary — or spending a couple of weeks "acquiring a specialization" on Coursera.

* To Create. We might not do this consciously, but often we make connections between different pieces of information we have consumed to produce new and sometimes original information. Unlike "To Understand", we do not consciously seek specific pieces of information because it makes us creative.

* To Stimulate. Finally, we consume a lot of information, for no other reason, except because it is fun, enjoyable, or entertaining.

## Models and Theories

Now that we have specified our goals, I am going to present some speculations on how these goals might be met, to set a foundation for the "guidelines" that might help with better achieving these goals.

### On Understanding

Whenever we consume information (be it watching, listening, or reading), are brains are bombarded with ideas, concepts and images. Some of these we remember, others we do not. In fact, at the time of consumption, our brains have a sort of "buffer" which temporarily stores the pieces of information. Some forms of information need larger or deeper buffers, while others can do with smaller, shallow buffers.

Maintaining a deeper buffer needs more mental effort. Often, our buffers "run out" and we need to re-consume information, to make use of it (e.g. Re-reading a section of a book which is profound, or otherwise difficult to understand).

Our brains also store information with significant redundancy — meaning that the same information is stored multiple times in many places. Hence, repetitive consumption of the same information often results, not just in easier recall, but also a better understanding of that information. In fact, in many disciplines (e.g. music) memorization (acquired through repeated consumption) has been considered essential for a more complete understanding.

### On Creating

As implied above, by "creativity" I'm specifically referring to the "creation of ideas". My mental model for describing "how creativity happens" goes something like this: two or more ideas or pieces of information join or combine to form a new (sometimes original) piece of information. Matt Ridley describes creativity as what happens "when ideas have sex".

Creativity is intricately connected to the process of understanding. The more ideas and concepts we deeply understand, the larger opportunity for ideas to combine and recombine to form novel ideas.

### On Stimulation

What makes an idea stimulating? For me, the process is akin to resonance. Just as a glass shatters when subject to a loud voice that exactly matches its natural frequency, we find ideas stimulating when we feel some familiarity with the idea. However, its not familiarity alone — but a combination of familiarity and variety. We are stimulated the most when we consume information which is familiar, but also novel and imaginative in some way. If information is familiar alone, it is boring. However, if it is pure variety, with no familiarity, we are confused.

## Deep Consumption vs. Shallow Consumption

There are many ways to "classify" information. But for the purpose of this note, I'd like to present to idea of "deep" and "shallow" information. One can think of the "depth" of a piece of information as how much mental effort is needed to process it. A good intuition of depth is how deep a "buffer" (as presented above) is needed to consume the information, and how much time is needed to consume the information. Deep information needs a deep buffer, and more time to consume.

Let me try and add more colour to this spectrum by comparing its extremes: Deep information and Shallow information. I'm going to refer to the consumption of deep and shallow information as "deep consumption" and "shallow consumption" respectively.

* Size and Time: Deep consumption involves consuming large pieces of information, which might take hours or days. Shallow consumption involves smaller pieces of information consumer over a short time.

* "Buffer Size" and Mental Effort: Shallow consumption requires a smaller mental buffer; deep consumption requires a deeper buffer. A deeper buffer also implies more mental effort. It might also involve false starts and repetition.

* Knowledge and Understanding: Deep consumption results in more ideas being consumed, and results in more understanding and more knowledge. Shallow consumption on the other hand results in a few new ideas being gained.

* Connections and Creativity: Deep consumption results in the opportunity for more new connections — and hence more creativity.

* Redundancy and Recall: Deep consumption results in the same information being stored in many parts of the brain. As a result, memory is more persistent and recall is easier.

* Time to stimulation. Shallow consumption usually exploits simple familiarities, and hence results in quick stimulation ("instant gratification"). Deep consumption requires some time before familiarity can be established.

* Initial consumption cost: Given the mental effort and delayed stimulation associated with deep information, Deep consumption has a much higher "initial cost". Shallow consumption has very low cost.

* Depth of stimulation. On the other hand, deep consumption results in connections being established with many familiar concepts as well as contrasting new ideas in a wider variety of ways. Hence, when stimulation happens it is deeper and more satisfying.

* Complexity. Deep consumption involves consuming many different ideas. In contrast shallow consumption involves consuming a small number of ideas.

* Similar information. As a result of lower complexity, it is easier to find other pieces of information similar to a given piece of shallow information — and justify why it is similar. This is much harder with complex deep information.

* Suggestion and Chaining. Given that it is easier to find other similar pieces information to piece of shallow information, it is easier to "suggest" other pieces of information similar to shallow information. Hence, consumption of shallow information often involves the "chaining" of many pieces of similar information. For example, you might watch one short Cat-Video on YouTube, and end up watching 13 in succession. This type of "chaining" is hard with deep information.

* Push vs. Pull. In contrast, since it is hard to "push" deep information to a consumer, consumption usually follows a "pull" model — with the consumer actively specifying what information he/she wants to consume.

* Finite vs. Infinite. Another consequence of "chaining" is that shallow consumption is often unbounded. There is no limit of how many similar pieces of information you can consume. For example, "cute cat videos" returns nearly 800,000 results on Google. On the other hand, "a deep consumption session" actively chosen by the consumer is finite.

## Credo

If the goal of information consumption is knowledge, creativity, and stimulation, then I believe that deep consumption is clearly preferable to shallow consumption. The "guidelines" I am going to propose hinge on accepting this belief.

## Guidelines to Self

All that was "theory". What does this all mean in practice? I have distilled these thoughts into the following guidelines:

* Do Long Duration. Have a "minimum duration limit" on consumption. For example, a video should be at least 30min. Avoid short, click-baity articles. Instead, read articles that are long enough to build a reasonable an argument.

* Do Make Time. If we consciously make time to do something, we are more likely to make better use of that time. Conversely, if we sneak in some actively into time which we were supposed to be doing something else, we are more likely to spend it unwisely. Most shallow consumption happens on this "stolen time". On the other hand, if we consciously make time, we are likely to choose to spend it on deep consumption.

* Do Finite. Limit consumption to information which is finite. Hence, I avoid infinite feeds of information, and apply some "bounds" that make the information finite. With news, I've restricted myself to the print version of papers — even when reading it online or in different formats (e.g. I "consume the Economist print edition", in audio form using the Economist App).

* Don't follow suggestions. I watch a lot of videos on YouTube, but don't follow YouTube suggestions. Instead, I search for the content that I want to watch. Most of the suggestions by YouTube belong to a small subset of topics that I've watched in the past, and, were I to solely follow suggestions, would result in me getting passively "siloed" into consuming solely these topics.

* Do Active. More generally, I try to actively pick what information I consume, as opposed to follow passive suggestions.

* Do Repeat. Often when I like a book, I read it again. Often, I find that I learn many new things on the second read. Sometimes, I also consume the same information in different ways. For example, I might first listen to an audio book, and then "manually" read it off a hard copy.

* Don't Chain. I've shifted to consuming Newsfeeds more like "News-papers", where I will look at my feed (say) once a day, and consume a limited number of articles. This applies to Facebook, Quora, Twitter and LinkedIn. To limit passive chaining, I've uninstalled feeds from my phone.

* Do add friction. One reason it is easier to shallow consume, is because it has a lower initial cost. We can get around this by artificially adding friction to shallow consumption tasks (e.g. block sides on your browser),

* Do remove friction. Conversely, we can reduce friction to deep consumption tasks (e.g. keep a book where you can see it, buy a ticket to a concert or movie — forcing you to go).

* Do Offline. Sometimes, deep consumption can only happen offline. This is particularly true with the information transmission that happens (or should happen) with human relationships. The internet simply has insufficient bandwidth to transmit all the nuances that must be sent and received.

![Image](https://cdn-images-1.medium.com/max/800/1*OXZjezwMY_xkP4VmgwWClA.jpeg)

#### Article 10 · September 9, 2018

# Who do you side with?

## But not simpler

This week's Economist has an excellent article on how European political issues and topics are tangled and complicated. It gives some good examples of where the simplistic "right-left" classification and other binary over simplifications breakdown:

>>> "Look more closely, however, and it all seems more tangled. Mr Orban may be undermining the rule of law in Hungary, but he sits in the European People's Party (EPP), a group that includes Angela Merkel, Germany's chancellor. Mr Macron may be a globalist, but he nationalised a French shipyard to prevent its takeover by an Italian firm last year, and this June declined to take in Aquarius, a refugee ship rejected by Italy. Ordinary Europeans are similarly complicated. Most residents of Chemnitz, for example, attended neither pro- nor anti-migration protests." [1]

## Meanwhile in California...

Earlier today, among the elegant citizenry promenading Palo Alto's University Avenue, was a scruffy looking woman, pushing a shopping cart, piled with various grey tinged clothes, papers and baggage, with a big "I love Trump" sign taped to the said cart.

In the same block was a retired educator collecting donations for some drug rehabilitation related charity. In return for a small contribution, he presented me with a bunch of "thank-you" marketing material, including a comical list of poems praising the virtues of a certain Bernie Sanders, and poking fun at the said much-loved Donald Trump. He somewhat bizarrely, prefaced this presentation with a "Do you hate Trump?" question (apparently expecting nothing but full agreement).

Whatever the Economist might pontificate, simplistic "right-left" classifications seemed alive and well, at least in Stanford-educated Palo Alto. One might tolerate some bias among "ordinary people". However, when I looked at the latest Facebook posts of the Representative in Congress for Palo Alto [2], the two senators for California [3] [4], and the President [5], I noticed exactly the same phenomenon.

While there were no funny poems, or declarations of undying love, almost all posts I read had three things in common: 1) they attack the opposing political party; 2) issues are described as black vs. white, non-negotiable issues; and 3) "blame" is posited, not on individuals but on the opposing party as a whole ("Republicans", "Democrats"), or one of the synonyms for the said groups ("Conservatives", "Liberals", "Right", "Left" etc.).

## Who do I side with?

I've been annoyed, irritated and worried by this over simplification for some time. Related, I wrote this note, Frustrations and Fears [6] soon after the 2016 presidential election. It seems impossible to have a reasonable conversation about politics without siding or being sided into one of the two sides. I found this particularly frustrating because, as I wrote in the said note:

>>> "I've struggled to exclusively identify with a particular party. This is because, once I list all the issues, I agree with the Blue team on some, with the Red team on others, and neither on still others. On most issues, I'm more aligned with the Blues, but there are others which I'm more aligned with the Reds. In this sense, I'm neither Blue, nor Red, but Purple; even if its a Bluer shade of Purple." [6]

Often friends on the Blue team ask me about the issues "I'm more aligned with the Reds", and friends on the Red team vice versa. It is usually difficult to give a good answer, particularly in a real-time conversation, because there are so many issues, and I've often thought of a more efficient way to answer these questions.

## A Quiz to the rescue

I found a reasonable solution in https://www.isidewith.com/. Basically, you take a quiz on various issues and topics, and it gives you some statistics on how you align with various politicians and political parties. For example, I took a quiz on the 2016 Presidential Election candidates, and got the following results [7].

![Image](https://cdn-images-1.medium.com/max/800/0*rqcSJkCoiYIwHryj)

Unlike some of my friends who swore 100% loyalty to Hillary Clinton, or Donald Trump, I had non-zero "agreeableness" with all the candidates, including a decent 28% with "the Donald". Sadly, my top two candidates had almost no chance of winning the election, but I think that's a problem with the system not their candidacy. Some of the most vibrant democracies, have weak political parties, and minority governments. The ability for a new party to overthrow the status quo is usually a good sign.

Digging deeper into the results, I learnt how I stand, not just on one "Left-Right, Black and White" binary question, but on several "spectrums" with many shades of grey.

![Image](https://cdn-images-1.medium.com/max/800/0*vXRfTbU7a4M8NUrb)

[The colours reflect how important the issues are for the candidate, where "Red" is most important, and "Green" is less important]

Finally, the best answer to "I'm more aligned with the Reds/Blues..." came from a graphic which compared the degree to which I agree with the various candidates on various topics:

![Image](https://cdn-images-1.medium.com/max/800/0*xp_9euzzyl-pmPhb)

While I agreed with some candidates more than I did with others, I was at least neutral with all the candidates on at least some issues. I also disagreed with my best-matched candidates on a few issues.

[The quiz analysis has a lot more detail. I shared just a sample.]

## Disclaimers

I love caveating my ramblings. My caveat for this note is, I don't know how scientific the ISideWith.com quiz is.

On the other hand, I found its results for me quite reasonable, and definitely preferable to a blunt instrument that obtusely chucked be in the Red corner or Blue corner. Also, I'm sure there are other, possibly better quizzes around.

## Happy Voting!

Regardless of how we perform on this quiz, it is universally good for all of us to be more nuanced about our political opinions. It will lead to better conversations with friends, funnier poems, more love, and better governance across the world (note, these ideas are hardly restricted to the US).

#### Article 11 · November 19, 2018

# Black or White?

## Donkeys or Elephants?

![Image](https://cdn-images-1.medium.com/max/800/0*iqpoGybMJS49dfFt)

In the lead-up to the 11/6 Midterm Elections in the US [1], I shared some thoughts on "binary politics" and more the one-sided, partisan nature of political discussions [2] — Either you support the Democratic Party (Donkeys) or you support the Republicans (Elephants), with no middle ground, or room for debate.

Meanwhile in Sri Lanka, we have been witnessing an interesting constitutional drama (also known as #CoupLK and a the "Constitutional Crisis"). The timeline is roughly as follows:

* 10/26: The executive President Maithripala Sirisena fires the Prime Minister (PM), and appoints former president Mahinda Rajapaksa as the new PM [3]

* 11/9: The president then dissolves the parliament, and calls for general elections on 1/5 [4]

* 11/12: The supreme court suspends the dissolution [5]

* 11/14: Parliament meets, and votes for a No-confidence-motion against the new PM [6]

I'm no expert to share my own opinions on the constitution, but I did make the following observations about the political discussion surrounding the drama on Facebook, Twitter and news media.

* The vast majority of people's opinions are still defined by their allegiance to one of the two major parties (i.e. the UNP, the party of the old PM, and the SLPP, the party of the new PM) or their allies.

* In a worrying number of cases (though hopefully not a majority), this binary party affinity seems to be more important than upholding the constitution

* Voting in a future election is likely to be cut along this binary choice.

## Black Eyes

![Image](https://cdn-images-1.medium.com/max/800/0*djcgXpipl54tZVIZ.jpg)

And now for something completely different.

What colour are my eyes? If I said, "they are black", it would be easy enough for you to understand.

On the other hand, if I told you "they are not black", what would you comprehend?

If you have met me in person, and observed my eyes, you might say "dark brown". If you have not met me, but live on Planet Earth, you might say brown, blue or even green. If you are from Mars (and do not know the colour of human eyes), you might even think red, yellow, or purple.

What I am trying to get at is this:

While "Black" has a specific, objective meaning, "Not Black" is a lot more subjective — and varies a lot depending on one's point of view (and planet of birth).

## මගේ ඇස් කළු නැත

In fact, "not Black" has no concrete meaning. It's meaning is completely abstract, and derives from the binary logical operator "not". Note, this logic is "binary" because it has two states: Something and "not" Something.

Now what if our logic was not binary? What if we did not have a "not" operator. While binary logic dominates our thinking, there is some evidence that other forms of logic were prevalent in many cultures, including Sri Lanka. There is a hint in the Sinhalese translation of "My eyes are not black". Google translate spits out "මගේ ඇස් කළු නැත". Now if this sounds wrong, do not be too hasty to blame google.

The "hint" is that there is no good translation. "My eyes are not black", while straightforward in English, is a bit of an alien idea in Sinhala.

## Not Binary

Now, what might a "non-binary logic" look like?

Let us start with binary logic and break-down some of its laws.

For example, let us consider "My eyes are black". Let us label this proposition, "P". Then, "My eyes are not black" becomes "Not P".

* P = "My eyes are black"

* Not P = "My eyes are not black"

Now, the laws of binary logic state that both "P" and "Not P" cannot be true at the same time. In other words, my eyes cannot be black and not black at the same time. Also, the laws also state that at least one of the two have to be true: That is, either my eyes are black, or they are not black.

What if we break these laws? Then, the following could also be true:

* Both P and Not P: "My eyes are black, and my eyes are not black"

* Neither P nor Not P: "My eyes are not black, nor are my eyes not black"

Note, we have moved from binary (2-state) logic, to 4-state logic.

## Two types of Ignorance

But what does "My eyes are black, and my eyes are not black" and "My eyes are not black, nor are my eyes not black" mean?

Consider the following types of ignorance:

* We are ignorant of nuance. For example, the earthling who had not met me (described earlier) thought "not black" meant brown, blue, grey or green. For it, "not black" simply could not be something else.

* We are ignorant of overlap. For example, my perception of black might overlap with your perception of dark brown. In fact, my eyes do look black in certain conditions and dark brown in other conditions.

Assuming these two types of ignorance, "My eyes are black, and my eyes are not black" is true, because my eyes are indeed black, but they are also dark brown, so they are not black. At the same time, they could be a shade of black which, to you, is not black, and a shade of colour, which is inconsistent with your perception of "not black". Hence, "My eyes are not black, nor are my eyes not black" is also true.

This reasoning can be taken further — to 8 state logic, 16, 32, and so on ad infinitum.

## Beyond Donkeys, Elephants and Lotus Buds

![Image](https://cdn-images-1.medium.com/max/800/0*MNa9VDAKkrvExu8h.jpg)

Now, some of you might have understood me; some of you might have misunderstood me. Some of you might have both understood me and misunderstood me; while some of you might have neither understood me, nor misunderstood me.

Either way, let me conclude with an exercise for the reader. (I have localised the questions for a Sri Lankan audience. Friends in other parts of the world should appropriately localise the questions. For example, in the US, UNP/SLPP should be replaced with Republican Party/Democratic Party.)

Suppose by some magical power you ceased to be ignorant of nuance and overlap. In this blessed state, which of the following would you label as TRUE, and which as FALSE?

* All UNP politicians are illiterate, incapable, and corrupt.

* All UNP politicians are intelligent, capable, and honest.

* All SLPP politicians are illiterate, incapable, and corrupt.

* All SLPP politicians are intelligent, capable, and honest.

* I agree with all the policies and track-record of the UNP

* I agree with all the policies and track-record of the SLPP

* My perception of "Not UNP" is SLPP

* My perception of "Not SLPP" is UNP

* To win an election, an Parliamentary or Presidential candidate should be a member of the UNP or the SLPP (or an alias of one of these).

* I am a UNPer, therefore I am not a SLPPer.

* I am a SLPPer, therefore I am not a UNPer.

* I am not a UNPer, therefore I must be a SLPPer.

* I am not a SLPPer, therefore I must be a UNPer.

Please comment with how many TRUEs you got, and how many FALSEs you got.

## Works Cited

[1] [Online]. Available: https://en.wikipedia.org/wiki/United_States_elections,_2018.

[2] [Online]. Available: https://medium.com/@nuwan.senaratna/who-do-you-side-with-c983109e304f.

[3][Online]. Available: https://www.aljazeera.com/news/2018/10/sri-lanka-president-sacks-prime-minister-appoints-rajapaksa-181026174208405.html.

[4][Online]. Available: http://www.wect.com/2018/11/10/sri-lanka-president-dissolves-parliament-calls-election-2/.

[5][Online]. Available: https://www.bbc.co.uk/news/world-asia-46196979.

[6][Online]. Available: https://www.bloomberg.com/news/articles/2018-11-14/sri-lanka-parliament-passes-no-confidence-vote-against-new-pm.

#### Article 12 · November 20, 2018

# The History of AI

### (in less than 60 seconds)

![Image](https://cdn-images-1.medium.com/max/800/0*Bi81jXVxWABeNVWQ.png)

### AI 0.0 = Human generated Rules (Before 2000)

Humans codified their knowledge and intuitions into Rules, and programmed machines to implement these rules.

>>> "Dear Machine, If your opponent played this move, then play that move."

### AI 1.0 = Learning from Data (After 2000)

Progress in computer hardware, and the ability to collect large amounts of data, led to Statistical Machine Learning on Data.

>>> "Dear Machine, Here's a history documenting millions of chess games. Try and learn how to play chess.

### AI 2.0 = Learning from Data, generated from Simulation (After 2010)

Further progress in hardware, led to fancy simulation software. Simulation led to vast amounts of data, which in turn could be used to do more elaborate statistical machine learning (also running on fancier hardware).

>>> "Dear Machine, You can learn how to play chess by playing millions of games your self"

### AI 3.0? (After 2020)

Simulating complex behaviour, including human behaviour?

>>> "Dear Machine, This stuff is too complex to get my head around. Can you run zillions of simulations and see how things will turn out, and then tell me what to do?

#### Article 13 · November 24, 2018

Shashank Bharath: "This" means a more freer distribution, and a more egalitarian distribution of data. One important shift with decentralized apps is that data could be stored, owned or controlled by the original owner. This gives the owner more control on data — and leads to a more equitable distribution. See https://medium.com/@timberners_lee/one-small-step-for-the-web-87f92217d085 for more details.

#### Article 14 · November 24, 2018

# Web 4.0

![Image](https://cdn-images-1.medium.com/max/800/0*kaJmESRg-8CbWx_R.jpg)

Technology (both Hardware and Software) is full of "version numbers". For example: I use an iPhone 8, running iOS 12.1. I'm writing this blog on a computer running Mac OSX 10.13.6, using TextEdit 1.13. Often, we are on the lookout for new version (and their new version numbers), because they might have "cool" new features, or patches to problems in old versions. Often, we are also reticent to install a new version, because it might not be sufficiently tested, and might have unexpected bugs.

The Internet, or World-Wide-Web (WWW) or simply the "Web" is also a giant collection of hardware and software. It is continuously evolving, and unlike OSX or TextEdit, it has not explicit version numbers or releases. On the other hand, it is possible to look at the Web as a whole, and observe various characteristics that can be compared to what the web was 5 or 10 years ago. It is also possible to identify what characteristics might be desirable for the web, and encourage builders of hardware and software to implement these.

In this article, I share a short list of "characteristics" that might be desirable for the future web (which I call "Web 4.0"). Like iPhones or OSX, I consider these "desirable" because A) they add new functionality to the web, and B) fix bugs in the current version.

However, before that, let us review the previous "versions" of the web.

### Web 1.0, 2.0 and 3.0

The term "Web 1.0" is a "retronym"; it was invented retrospectively contrasting it to "Web 2.0". Web 2.0 enhanced Web 1.0 principally in the following ways [1]:

* Producers and Consumers: In 1.0, there were few producers of information, and (relatively) many consumers. In 2.0, with the advent of social networking provides and low cost web hosting, the number of produces also significant increased.

* Static and Dynamic: In 1.0, content was static. In 2.0, there was more dynamic content, with consumers able to comment and interact directly with the content.

While there is no universally agreed upon definition of Web 3.0, it is trending in the direction of a "collective intelligence" made up of billions of devices and humans connected in a single intelligence whole [2]. That is, while 2.0 was made up of many independent systems, 3.0 will form a collective whole.

### Web 4.0

I'm going to list my characteristics "comparing and contrasting" it to the current web (which is probably best described as a mix of 1.0, 2.0 and 3.0).

* Centralization to Decentralization: Web 3.0 is increasingly dominated by a small number of big players (e.g. Google, Facebook, Amazon), who individually own massive "collective intelligences". This is not optimal for several reasons, including the fact that a small number of humans don't have the creativity to make the best use of a large amount of data. Hence, Web 4.0 should have a much freer distribution, and a more egalitarian ownership of data and distribution. One obvious way of making this happen is through decentralized apps, with private ownership of data.

* Optimization to Sub-Optimization: The most interesting problems on the web involve applying artificial intelligence to ranking and prediction problems (e.g. Google Search, Facebook Newsfeed, Amazon Product recommendations). One danger of this approach is that it channels large numbers of humans to behave in such a way to optimize a few numbers (e.g. Google Search Clicks, Time Spend on the Facebook Newsfeed, Amazon Sales). This is a problem because, while the "numbers" might make sense, the emergent human behavior is difficult to predict. "Sub-Optimization" could solve many of the behavioral bugs of Optimization. By "Sub-Optimization" I refer to a sub-optimal form of optimization which results in more predictable behavior. Example of "Sub-Optimization" include randomization, "fair" ranking methods (like simple time ranking), and biasing results to encourage psychologically optimal behavior.

* Web to Meta Web: Despite the huge impact the web has on our lives, there is relatively little study and education about it. For example, while most schools teach children how to read, play sports, and cross the road safely, few teach child about the web and how to use it. In Web 4.0, I hope there is a lot of retrospection and education about the web, and a corresponding enlightenment and education.

### References

[1] https://en.wikipedia.org/wiki/Web_2.0

[2] https://www.webopedia.com/TERM/W/Web_3_point_0.html

#### Article 15 · November 25, 2018

# Random Ballot

### On having the cake and eating it

## FPTP

Until 1977, Sri Lanka had a "first-past-the-post" or FPTP [1] voting system. The country was split into several regions known as "constituencies", various individuals contested elections in these, and whoever got the most number of votes, won the election. This was a simple system, and candidates were known to, and hence (at least in theory) accountable to the voters.

FPTP also had several disadvantages, including the fact that, for a given party, the number of candidates who got elected, was not proportional to the number of votes the party got.

For example, in the 1970 Parliamentary Election [2], the SLFP 91 seats with 36.86% of the vote, while the UNP won just 17 seats with 37.91% of the vote. The LSSP which got just 8.68% of the vote, managed to get 19 seats.

![Image](https://cdn-images-1.medium.com/max/800/1*rOE6ubAr_lc7oNDnAjF85A.png)

## PR

After 1977, FPTP was replaced with Proportional Representation or PR [3] for the general elections that elected candidates for the 225 seats in parliament. 196 seats were allocated to districts and were distributed to parties in proportion to the votes they got in each district. The candidates with the highest votes from each party were voted in. Similarly, a remaining 29 seats were allocated at a National Level, and each party had a "National List" of candidates.

While FPTP solves the "proportionality" problem, candidates were associated, not with constituencies, but with districts, or a broader National List. As a result, it was more difficult for voters to know who their representative was. The power to select representatives was effectively with the party.

![Image](https://cdn-images-1.medium.com/max/800/1*90fGLYr0yOKhsLtLtFbwCQ.png)

## Having the cake and eating it

The problem with FPTP is that it is not proportional. This is a problem because many votes (in theory, and often up to 50%) don't get to influence who gets elected. On the other hand, it is a simple, easy to understand system — a vital characteristic for a participatory democracy. The problem with PR is that voters don't know who their representative is, and conversely, representatives are less accountable to the voters.

What if there was a constituency-based voting system, which was also proportional?

## Random Ballot

A Random Ballot or RB [4] works as follows: The country is split into "constituencies", and Various individuals contested elections in these, just like FPTP. Of all the votes cast, one vote is selected at random. Whoever, the candidate is, wins the election.

RB has never been tried out in practice, and was first suggested by Akhil Reed Amar, as a "thought experiment" in 1984. It has the nice property that every vote has an equal probability of determining the outcome of the election. On the other hand, it also possible that a candidate who does not "win" the election (i.e. gets the most number of votes), does not get elected.

Any chance that RB will be considered in Sri Lanka, or anywhere else?

## References

[1] https://en.wikipedia.org/wiki/First-past-the-post_voting

[2] https://en.wikipedia.org/wiki/Ceylonese_parliamentary_election,_1970

[3] https://en.wikipedia.org/wiki/Proportional_representation

[4] https://en.wikipedia.org/wiki/Random_ballot

[5] https://en.wikipedia.org/wiki/Sri_Lankan_parliamentary_election,_1989

#### Article 16 · November 28, 2018

# #CoupLK

### From First Principles

## What is #CoupLK about? What do you think?

* A. The "Crisis" is all about the constitution. The President @MaithripalaS ‏ violated the constitution appointing #FakePM @PresRajapaksa. He mustn't be allowed to do that.

* B. The "Crisis" is about getting rid of the incompetent @officialunp. The @MaithripalaS has the right to get rid of them. We should support his actions, and vote in a new parliament. #LetMeVote

* C. This "Crisis" is about rotten politicians. It shows that all our parliamentarians (@officialunp, @SLPP everyone), are rotten. We need to get rid of all of them, and vote in some new faces.

90% of opinion and discussion on our (Sri Lanka's) constitutional crisis (a.k.a. #CoupLK) fall into groups A or B — split firmly along partisan lines. There is a small minority who purport C. While the options are true to some extent, not one represents the whole truth.

But then, what is the whole truth about #CoupLK? How should we think about it? What should we do? If you're interested, read on.

## Which hat is the President wearing?

Laws (including the constitution) are paradoxically circular. Citizens elect legislators. Legislators pass laws. Laws govern citizens.

![Image](https://cdn-images-1.medium.com/max/800/1*qnERuuGTgXvY_Tk_q4aI8Q.png)

Since citizens (through their elected representatives) pass laws, citizens are the masters of laws. But since said laws govern the said citizens, the citizens are also servants of the laws. Hence, citizens need to wear two hats: MASTER and SERVANT. To complicate matters, when a citizen is allowed to be MASTER and when they should be SERVANT is also defined in the said laws.

At the core of the #CoupLK is a particularly special citizen, the President, and it is not clear which hat he is wearing, or should be wearing.

* A. If you believe A, your claim is that @MaithripalaS is playing MASTER, when the constitution says he should be playing SERVANT.

* B. If you believe B, your claim is he's indeed playing SERVANT, or that he should be allowed to be MASTER.

* C. If you believe C, your claim is that all this is irrelevant. Everyone is playing MASTER when it suits them, and rotten politicians are solely to blame.

## Why be SERVANTs?

For laws to work, all of the following must be true.

* Definition. Citizens need to know what the laws are, either individually, or through the help of experts (lawyers).

* Transparency. Processes must be in place to know who is obeying the law, and who isn't.

* Enforcement. Citizens breaking the law need to be punished.

All of the above require the support of citizens and institutions made up of citizens. For example, transparency needs a free press, and enforcement needs an honest and efficient police force. For laws to work, all the citizens who are part of these processes must agree to be SERVANTs of the law.

## But, why laws?

Why go through all this trouble to be SERVANTs of the law?

After all, why did I have to waste 90 seconds at a red light, at 1 am, with no other vehicles anywhere to be seen? Why obey rules that innately curtail our freedoms?

This is true. All rules curtail our freedoms. But on the other hand, they also create freedoms which we might not have. For example, if no one adheres to road rules, it will not be safe to drive. Hence, effectively, stopping at a red light gives us the freedom to drive.

We shouldn't think "Why do I need to obey law X?". Instead we should think, "What if everyone disobeys law X?"

## But, why care?

Why would an ordinary citizen of Sri Lanka care about the constitution being violated?

Despite a lot of hype in the press (particularly the international press), things are surprisingly normal in Island. Except for the odd protest (and the ensuing traffic jam), for most people, it is business as usual. This is likely to change in the new year, particularly with a budget needing passage, but for now, it is what it is.

But back to our question: Why care? Even if I did care about laws, the powerful (especially politicians) of this country don't. So even if I do care, is there anything I can do?

## (Disguised) TODO List

I'm not going to list a TODO list. It's not because I don't have any TODOs in mind, but it's because I don't want to come across as "a person who tells other people what to do".

Instead, I'm going to describe "types" of citizens in this country. You will (probably) fall into one or more of these types. As for TODOs, with a little bit of reflection, it should be evident what you need to do.

### Types of Citizens

* The Legal Alien. You are a Sri Lankan citizen who doesn't care about politics or government or civics. While you have the right to vote, you have never voted in an election. All the laws you obey have been enacted by politicians who were voted in by other people. Hence, effectively, you are an alien forced to conform to an artificial set of laws. You might as well be in another country, or another planet. But then again, you don't really care about this country. Your birth here was mostly a random event, beyond your control.

* The Alien who loves Sri Lanka. For most part, you are just like "The Legal Alien". However, you have an emotional attachment to the country. All your close friends and family are Sri Lankans, and though you don't actively think about it, there are many things about Sri Lanka, that you love — from food, to music, to culture. At the same time you wish life could be better in Sri Lanka, and you wish you could do something about it. But like "The Legal Alien" you are civically inactive, and you despair that there is nothing you can do.

* The Armchair Citizen. Irrespective of your emotional attachment to Sri Lanka, you diligently vote in elections, and keep abreast of political news. You engage in robust conversations with your friends, and sometimes strangers. You can elaborate theories on fixing politically motivated problems. People often ask you if your interested in enacting these ideas — to which you reply that you have don't have enough time at the moment. Unknown to you, people consider you a bit of a joke — all wind, and no action.

* The Hopeless One. Like "The Armchair Citizen" you are a civically responsible citizen. You vote, you read, and you discuss. You also want to act, but don't see how — after all, power and money is centralized in a few hands. There are some contradictions in your thinking — for example, while you believe that "All politicians should be honest", you've often voted for politicians with dubious financial records. You justify this by claiming that there were no other options, particularly since the new candidate had no chance of getting elected.

* The Party Hack. Elections are a formality for you. You've always voted for the Party X, and that's how you will continue to vote. You are considered part of the "Voting Base of Party X". In effect, you don't have any political rights because your vote is a forgone conclusion. You think that the party considers you a loyal, even distinguished supporter. You are deaf to the title "sucker" voiced in your general direction.

* The Child. You are not old enough to vote, so some of the above might not be relevant. At the same time you don't want to repeat the mistakes of the older generation. They will soon die, leaving you to face the music.

What are you going to do? Comments welcome :)

#### Article 17 · November 29, 2018

# On Democracy

### And what next for Sri Lanka

![Image](https://cdn-images-1.medium.com/max/800/0*3kCQhD_UQ-aBg_64.jpg)

## Pre-Democracy

### The Individual (1 Human)

They say "no man is an island" [1]. But suppose you were a man or a woman on a desert island. On one hand, you'd be lonely, facing danger, and trying your best to get off the island. On the other hand, you'd be completely free, and able to do whatever you wanted, and you would make all the "decisions" on the island.

The island (in a trivial sense) would be both a democracy ("A system of government by the whole population or all the eligible members of a state, typically through elected representatives." [2]), and an autocracy ("A system of government by one person with absolute power." [2]).

### The Family (~10 Humans)

Now suppose you weren't alone on the island, but were with a small group of people; say about 10; like a family. Would things be different?

There would be some division of labour, based on the skills of the various people. For example, the stronger people would be doing the physical work. Some people (elders, or the "smarter" members of the family) would have greater influence in decisions.

### The Tribe (~100 People)

Suppose, now, that your family has grown larger, and there are many families on the island. Everyone still knows everyone, but everything is happening at a greater scale.

The division of labour is more "defined". There are people in trades, and social stratification is emerging. There are people who have accumulated wealth over time, and these people begin to form a plutocracy ("Government by the wealthy." [2]). The "smart" people in trades and professions feel their ideas should influence decisions more. They form guilds and other meritocracies ("Government or the holding of power by people selected according to merit." [2]). Everyone else continues to have some say, and hence the village also has some characteristics of a democracy.

A few people, or perhaps one person might want to gain more power over the tribe. This one person uses a combination of force and influence to achieve this end. He or she might create stories and beliefs to justify his or her aims — for example, that the "Gods want them to be leader of the tribe". Similarly, the various people favoring plutocracy, meritocracy, and democracy would also put forward their respective arguments, propose new "beliefs", some of them divine, often putting words in the mouths of gods. ‘

All said, whatever is is "what works".

### The Nation (~1000 People)

Your island has continued to grow. Many tribes have lived and died. The tribes that lived have grown and prospered. Some of them have conjoined to form mega-tribes.

Your mega tribe has over 1000 people. It's so big that, now, not everyone knows everyone else. There are many people you don't know, have never seen, and will (probably) never see.

However, you have a connection to these unheard and unseen people. They are all part of your nation ("A large body of people united by common descent, history, culture, or language, inhabiting a particular state or territory." [2]). While you might have nothing in common, at the same time, you have everything in common.

Your nation is united by a common story of how everyone in the nation belongs to it, and how that nation is the greatest, most noble nation in the world. Your nation is also united by common institutions. The tribal guilds are no longer mere functional institutions, but have become part of the nations story. While there are many nations in the world, your nation is the greatest, just as every other nation is the greatest to its people. Different nations are autocracies, plutocracies, meritocracies, and democracies to various extents. Each nation believes that its form of government is the best.

There is a happy convergence of "what works" and "what is right".

## The Emergence of Democracy

### Needs, Power and Evolution

![Image](https://cdn-images-1.medium.com/max/800/0*_xEEjjyZVx9-Oo1e.png)

What we saw above is an evolution: How individuals become families, how families become tribes, and how tribes become nations. Evolution is defined by the distribution of power. Individuals will promote whatever evolution satisfies their needs. These interests depend on what needs are already satisfied. For example (following Abraham Maslow [3]), an individual would first look to satisfy their basic physiological needs for warmth, air, water, food, shelter, sleep and sex. Next they will try to guarantee their physical safety — physically, emotionally, and financially. Once this is also satisfied, they will try to satisfy more complex, social needs from family and friends. Continuing this process, they will try to higher and higher needs like esteem, self actualization, and transcendence.

The form of government at a given time is defined by the distribution of power at that time. Power is determined by wealth, skills and influence. For example, if one individual has a disproportionate amount of force, wealth, skills and influence, they are going to have a disproportionate influence on the government. The extent to which the government is autocratic, plutocratic, meritocratic, or democratic, depends on the the effect of force, wealth, skills and influence respectively.

### Development, Equity, Enlightenment, Identity

There are examples of democracy ("A system of government by the whole population or all the eligible members of a state, typically through elected representatives." [2]) in various parts of the ancient world — from ancient Greece, to India — though in most cases "the eligible members of a state" was a restricted subset of the population — usually male, and wealthy.

However, in almost all cases, four factors seemed to caused the emergence of democracy, or the "evolution" of government into democracy.

* Development: The "eligible members of a state" had their basic physiological, safety, and social needs satisfied, and hence they wanted to satisfy esteem, and self actualization. This was in turn caused by prosperity, and technological developments.

* Equity: At least some group in the population had sufficient freedom to demand democracy, and hence they would have had some equity of power, relative to those with the most power.

* Enlightenment: The enlightened belief that all "eligible members of a state" were indeed eligible would have been more radical that it sounds, particularly since most of the early democracies evolved from autocracies with beliefs in the divine rights of kings and chiefs.

* Identity: The "nations" that adopted democracy had a strong national identity. Especially, relative to other nations. The citizenry felt a strong need to be part of the nation, and defend its nationhood.

### The Second Wave, and a causal fallacy

This emergence in the ancient world was again replicated in post-industrial-revolution Western-Europe, and then gradually spread to the rest of the world. All the early examples in the "second wave" of democracy (like the first wave in the ancient world) emerged out of development, equity and enlightened beliefs and a sense of identity. Like the city states in ancient Greece and India, the second wave democracies had smaller populations, adopted democracy in small evolutionary and partial steps. The choice of democracy also tended to be more pragmatic than ideological.

All this changed with US independence.

While the causal factors (development, equity, enlightenment, and identity) were similar to earlier examples, the ideological aspect of democracy was given precedence over the pragmatic aspect. For the first time, the "what is right" aspect took precedence over the "what works" aspect. Along with this ideological view of democracy, opinion on causality also began to reverse. While before democracy was a emergent property of development, equity and enlightened beliefs and a sense of identity, a new class of intellectual began to forward the idea that a democratic government will cause development, equity and enlightened beliefs and a sense of identity.

## Flawed Democracy

The success of the US and the west in the 20th century (particularly their cold war victory over communism), hugely increased the "brand value" of democracy. In fact, all the countries of the world but six (Saudi Arabia, Oman, the UAE, Brunei, Fiji, and the Vatican) officially admit to being democratic de jure [4].

![Image](https://cdn-images-1.medium.com/max/800/0*sNa9W2GlNtF40yr8.png)

The reality, is a bit different. According to the Economist's "Democracy Index" [5], only 19 of the 167 countries surveyed are rated "Fully Democracy" (or score 8.0 or above on the index). The US (7.98), Japan (7.88), India (7.23), and Sri Lanka (6.48) are all rated "Flawed Democracy" (6.0 to 8.0).

![Image](https://cdn-images-1.medium.com/max/800/0*dvXSsPES70RPFNZ7.png)

The 10 most democratic countries (in order, Norway, Iceland, Sweden, New Zealand, Denmark, Ireland, Canada, Australia, Finland, and Switzerland) have several striking characteristics:

* While they obviously claim to be democratic, and in every respect are, they are not "ideologically" democratic. Their most important reason for being democratic is "because it works", not "because it is right". This difference is obvious from their relationships with non-democratic countries — whom they don't "look down" upon. Note, this last point does not mean that these countries don't condemn human rights violations, terrorism etc, by non-democratic regimes. It's just that they don't hold a causal connection between these negatives, and a lack of democracy.

* They are small countries with high levels of development and strong national identities, where equity is easier to implement.

* Historically, they became more democratic has they become more developed, equitable, and enlightened, as opposed to the other way around.

In contrast, many of the worst democracies have had democracy imposed on them — sometimes by force. In such places democracy is unstable, and certainly not in equilibrium.

## Post Democracy

Our current decade is further proof of the causal direction of development, equity and enlightened beliefs and a sense of identity, and democracy. Many countries that self describe as "strong democracies" are battling authoritarian forces. It's difficult to ignore the following observations:

* Falling development. While the US and Europe continue to develop economically, there are significant sections of the population (e.g. Less educated white men in the US, and the youth in southern Europe) are seeing a significant decline in their quality of life.

* Falling equity. As Thomas Piketty pointed out [6] huge increases in inequality are rampant across the world, especially in the said faltering democracies

* Falling enlightenment: The internet is breaking the monopoly of a few "enlightenment" ideas, including the idea that "democracy is right". The distribution machines of Google, Facebook and Twitter mean that new ideas (both good and bad) proliferate (literally) at light speed. The filter bubbles and echo chambers created by "personalization" and "optimization" mean that discussion and deliberation is minimal, instead replaced by reinforcement of a narrow set of memes.

* Falling Identity: All but the smallest democracies had weak national identities. "Credal" identities like that in the US have always been fragile, and can easily breakdown. The strong "race" based identities in England, Germany and France are breaking down with immigration. These countries are struggling to replace their former identities with more "Credal" multicultural identities.

All these points to a weakening in the "causes" of democracy. It also highlights the fallacy of ignoring the fact that democracy is more an complex, emergent effect, than a simple cause.

## Sri Lanka: To Democracy or Not To Democracy?

For the first 2 millennia of our recorded history (~500 BCE to 1500 CE), Sri Lanka was an absolute monarchy. For the next ~450 years it was ruled by European powers who were in turn absolute or constitutional monarchies [7]. We have been a democracy for a relatively insignificant 70 years. And when I say "been a democracy" — I don't imply things have been perfect. Our democracy has been marred by violence, corruption and exclusion.

While, the last couple of elections in Sri Lanka have been relatively free and fair, the politicians elected have been, with a few exceptions, abysmal. This begs the question — "What's wrong with our democracy?" And more significantly, "Is democracy the right way for Sri Lanka?"

Reading so far, you might assume that I'm skeptical about democracy. You might even assume that I'm opposed to democracy, and am directly or indirectly proposing an alternative. If so, you misunderstand me.

Let me summarize my feelings towards democracy as follows:

### Qualities of Democracy

* Democracy is an emergent phenomena caused by development, equity, enlightenment and identity. In a nation with development, equity, enlightenment and identity, democracy emerges as a pragmatic and effective form of government. There is no special justification for that, other than it works.

* The causal relationship is not true in reverse. I.e. democracy doesn't necessary cause development, equity, enlightenment and identity. There are plenty of nations which are democratic which don't have development, equity, enlightenment and identity, nor have an increased chance of achieving these.

* Many nations (including some of the most successful democracies) took undemocratic paths to democracy. A "bad means doesn't justify good ends" argument does not work in this case, because "no-democracy" in isolation is not necessarily bad.

### So what should Sri Lanka do?

As Sri Lankans we should not be overly obsessed by Democracy as a virtue by itself. Instead, we should focus on the causal factors out of which democracy will emerge.

* Development. While Sri Lanka has achieved significant development in the last couple of decades, the job is by no means complete. We should focus on continued development, particularly in terms of technology, product development and intellectual property.

* Equity. Sri Lanka is, to a large extent, controlled by a small elite of wealthy, influential people. Law and Order, and Institutions are, to a large extent, subservient to this elite. The most effective way to create an equitable society is to make institutions, and law and order, strong, and this elite weak. Again, technology might come to the rescue.

* Enlightenment. While Sri Lanka has a relatively literate population, it is still somewhat backward in terms of intellectual freedom. Philosophy and thought are still very much grounded in religious texts and feudal identities. Technology and the internet have mostly made things worse. We need to find ways of turning this around, including finding more enlightening uses of technology.

* Identity. Last and most important. Sri Lanka has no national identity. We have various racial, religious, caste, and class identities, but these always trump the national identity. Hence, everyone is more Sinhala, Hindu, Govigama or "English-Speaking" than they are Sri Lankan. Our country needs a strong identity and a unifying story.

If we achieve progress in these dimensions, we'll get democracy for free. If we just blindly focus on democracy (because it is the right thing), then we'll probably end up like "Democratic" Republic of the Congo: 1.51 on the Democracy Index, but still proudly (i.e. de jure) "democratic".

## References

[1] https://en.wikipedia.org/wiki/Devotions_upon_Emergent_Occasions

[2] https://en.oxforddictionaries.com

[3] https://en.wikipedia.org/wiki/Maslow's_hierarchy_of_needs

[4] https://en.wikipedia.org/wiki/Democracy

[5] https://en.wikipedia.org/wiki/Democracy_Index and https://www.eiu.com/topic/democracy-index

[6] https://en.wikipedia.org/wiki/Capital_in_the_Twenty-First_Century

[7] https://en.wikipedia.org/wiki/History_of_Sri_Lanka

[8] https://www.dnaindia.com/world/report-chaos-prevails-in-sri-lankan-parliament-as-leaders-hurl-chilli-power-furniture-2686428

[a] They style and spirit of this article was inspired by https://en.wikipedia.org/wiki/Sapiens:_A_Brief_History_of_Humankind, and Yuval Noah Harari other writings.

#### Article 18 · November 30, 2018

# A Tale of Three Friends

### A philosophical fiction

![Image](https://cdn-images-1.medium.com/max/800/0*PsN2a8VDOr_AaXPT.jpg)

Mr. Lucky, Mr. Smart and Mr. Success have been the best of friends for years and years, and since I don't know when, they have been meeting every Friday evening, at their favorite pub ("Ye Olde Head and Tail"), for a drink, and play their favorite game. The game is the simplest possible. They get a coin from the bartender (a Mr. John Walker), and try to guess the outcome of tosses. Whoever guesses correctly the most times, wins.

Now unknown to his other friends, Mr. Smart is "friends" with the bartender's wife, Ginny Walker. She happens to know that the coins in the bar are actually weighted — with a higher chance for falling heads, or tails. Each week, she tells Mr. Smart what the weight of the coin is. Unfortunately, Ginny gets awfully muddled sometimes (it's the Gin), and tells Smart the wrong side. Regardless, Mr. Smart guesses correctly suspiciously often. Lucky and Success also suspect funny business — and tell off Mr. Smart. At times like this, Mr. Smart tends to reply smugly, "I'm always Smart, ain't I?"

Now Mr. Walker is unhappy with his wife machinating with Mr. Smart. So he decides to do something about it. He builds a special mechanism on the three friends' table (upon which the tossed coins fall) such that the special mechanism (magically) listens to Lucky's call, and flips the coin accordingly. The mechanism is not perfect — but still works most of the time — certainly more often than Ginny Walker is "un-muddled". So Lucky calls correctly more often than Smart. But unlike Mr. Smart, Mr. Lucky has no explanation for his unusually good luck. And whenever, one of his friends notice that Lucky is unusually Lucky, Lucky shrugs and replies "I'm just Lucky — I've always been Lucky. Haven't I?".

Now which friend ends up winning? (You might ask)

Lucky? (You might say) No.

So Mr. Success won! (you might reply).

Well — Yes — And — No.

Mr. Success, when he's not tossing coins, is a renowned particle physicist. Unknown to his two best friends (and even the rest of the scientific community), Success has built a time machine (which he activates with his mobile phone). A few seconds before he needs to guess a coin toss, he activates the time machine, travels into the future, observes to outcome of the toss, travels back to the present, and guesses correctly. Unlike the muddle Mrs. Walker, or the faulty mechanism in the table, Mr. Success's time machine is perfect, and he never mis-observes the coin toss. Hence, Mr. Success always wins.

(But you protest) So Mr. Success won? Then, why did you say yes — and No?

Well, unknown to Mr. Success, each time he activates the time machine, the future duplicates itself into two parts, duplicating the whole universe with it. So in actual fact, two copies of Mr. Success travel into two different futures. In one future, the coin falls heads — and in the other tails. So while in one future Mr. Success always wins, in the other he always looses, and Lucky (or somewhat less often) Smart, ends up winning.

The End.

## Quod ex historia moralis

* It's better to be lucky than smart

* The one who is successful is the one who is successful, and success beats both luck and smarts.

* Success is not as it seems.

#### Article 19 · December 3, 2018

# Meta Resolutions

### (I originally posted this on Facebook at the start of 2018 [1]. I hope to review these resolutions on medium, before the end of the year. Hence, this sharing.)

In 2015, I made some new-year's resolutions. In 2016 and 2017, I decided not to. This year, I thought of setting myself, not really resolutions, but some "meta-resolutions" — things that should influence everything I "resolve" to do.

## i. Work Hard

Work Hard. Working hard is giving this moment all. All the attention I can muster. All the attention that moment deserves — which is all the attention. There is no other moment but this moment. And there is no such thing as bad or useless hard work. Work Hard.

## ii. Be Simple

Be Simple. Embrace what really matters. What I know what I want. Discard and renounce everything else. Especially things I think or feel I want but know is unnecessary or meaningless. Be Simple.

## iii. Play the Long Game

Play the Long Game. Nothing of short term is of value. Resist and desist the ephemeral, the transient and the evanescent. Everything of value needs time and hard work. The long game doesn't end at some magical point in the future. Or at the end of some mystical time window. The long game begins now, and persists as long as meaning and purpose exist. Play the Long Game.

## iv. Unjustify Pain

Unjustify Pain. Pain is when pain is. The hardest pain stems from justice denied. When justice is rationalized as rational even when it might not be. Let go of that lust for justice and the pain goes with it. Unjustify Pain

## v. Untether from time

Untether from time. Untether time or time will tether. Be a slave to a window of moments, and what I create in that window will be constrained and contained into that brief casing. Consequence derives from meaningful time. Infinite value stems from the promise of infinite time. Untether from time.

## vi. Finish

Finish. An unfinished moment begets unfinished moments, gradually straying from the original purpose. Finish the moment. Ask why. Why it happened in the first place, and let it end. Finish.

## vii. Give-up

Give-up. Meaningful work needs time. And if I'm to work on valuable things, I'll need to give-up valueless things. Give-up.

## viii. Break Rules

Break Rules. Walking in a straight line is easy. But achieving a goal might involve walking along a curving, even distorted path, even in circles, or completely turning around and walking in the opposite direction. Momentum can be the wrong momentum. Habits can kill. Some rules are the wrong rules. Break Rules.

## ix. Plead Ignorance

Plead Ignorance. Failure springs from refusing to accept what I don't know. Leading to miscalculation, misjudgment and mishap. Get comfortable with saying "I don't know" perhaps even "I won't know". Plead Ignorance.

## x. Be Humble

Be Humble. Success is the child of proficiency, probability and provenance. When I succeed, I, too often, embrace the former, and forget the two latter. Be Humble.

[1] https://www.facebook.com/notes/nuwan-i-senaratna/meta-resolutions/10155358836008565/

#### Article 20 · December 5, 2018

# On Pain and Pleasure

### From Philosophy to Calculus

### Philosophy in a time of influenza

Do you remember the last time you got the flu? I had an attack of flu some months ago.

The first day was bad. I had a temperature. Sore throat. Cough. Dull headache. It was difficult to sleep. Nor did I feel up to reading a book, or listening to something. I had no appetite to speak of. As I said, it felt pretty bad. That was the first day.

But it's the second day I want to talk about. Or more specifically, the evening of the second day. Because on the evening of the second day, I was beginning to feel a bit better.

I was still quite sick and weak. The mercury was not quite back to normal, and I coughed a lot. But I had the first indications that the disease was on its way out. I felt better. And oddly, clearly better than I was before I got sick in the first place — when I was "not sick". I felt pleasure, optimism, gratefulness, and the overwhelming sense that things were going to get better, not just with my health, but with life in general.

Pain and pleasure are like the first and second days of flu; completely relative. You feel pleasure if what you felt before was worse. And you feel pain, if what you felt before was better. Hence, there is a limit to the amount of pain and pleasure you can feel. For after a couple of days, "feeling good" becomes pleasure-less, boring and meaningless, and perhaps even annoying. Conversely, while "feeling bad" might painful and hard to deal with at first, but soon becomes bearable as time goes on.

### Calculus in a time of procrastination

* So, if what you feel at time t is f(t), you will feel pain if f(t) - f(t-1) is negative, and pleasure if it is positive. In the notation of calculus, pleasure = df/dt. Or equivalently, pain = -df/dt.

* For constant pleasure (a), what you feel must uniformly get better (df/dt = a implies f = at + b). The amount of pleasure is independent of the base feeling (b) from where you started. You can feel bad initially (b < 0), but experience pleasure (df/dt > 0), if how you feel is getting better (a > 0).

* Pain and pleasure are consequences of time, and more specifically memory. If you have no memory of how you felt in the recent past, pain and pleasure are meaningless. In calculus-speak, df/dt cannot be defined if f is not continuous.

* If you are focusing single mindedly at the present moment, ignoring past and future, you can't feel pain or pleasure. You are measuring f at a single point of time, and hence df/dt has no meaning.

* Pain and pleasure are consequences of feeling. Feeling is often subjective, and can change course suddenly. For example, we might be feeling increasingly worse, and then something sudden happens, and we start feeling increasingly better. There is no pain or pleasure at the "cusp" at which this change happens. In other words, df/dt cannot be defined if f is not differentiable.

* If you want to feel a constant level of pleasure (df/dt = a), you need to find ways to constantly feel better and better (f = at + b). In the real world "better and better" requires more and more material goods, in turn requiring constant economic growth.

* The only level of pleasure which is growth neutral is zero. This coincides with no change in feeling. In other words, df/dt = 0 implies f = b (constant).

* The routines of most people are fairly constant, as is the way they feel. Most people attempt to embellish this even-keel with bursts of "feeling better" (E.g. Entertainments, Vacations, Affairs etc). Each of these episodes are characterized by pleasure (with the "feeling better" burst), neutral feeling (when feeling plateaus, "maxima" in calculus-speak), and then pain (when things go back to normal). Hence, pleasure is borrowed in return for future pain. If your goal is extreme pleasure, you need to be prepared and acquire a taste for extreme pain.

* Conversely, when things "hit bottom" (lowest level of feeling, "minima" in calculus-speak), pleasure is just around the corner.

* While "feeling" often has real meaning, pain and pleasure have little meaning in isolation; just the absolute state of the economy has more meaning than the economic growth rate in isolation. For example, Iraq had a GDP growth rate of over 50% in 2004[2], while Japan's growth rate has been almost "stagnant" for a generation [3]. The question is whether you'd like to be Iraq or Japan.

![Image](https://cdn-images-1.medium.com/max/800/1*I1pk6WPDDhZ5MV_Rbv04hQ.jpeg)

[1] https://www.flickr.com/photos/internetarchivebookimages/14596852489/

[2] https://tradingeconomics.com/iraq/gdp-growth-annual

[2] https://tradingeconomics.com/japan/gdp-growth-annual

#### Article 21 · December 5, 2018

# On work

### Confessions of a working man

>>> "You need to do something today" [I say]

### Doing my bit

>>> Why? [You say]

![Image](https://cdn-images-1.medium.com/max/800/1*5we6iLu8Eop8QwW6CbsZGA.jpeg)

Because that's what people do. People do stuff. People work. People are productive.

In other words, people are supposed to be changing things for the better. And people are.

Doctoring sick people. Engineering bridges and microchips. Teaching stupid kids to be smart kids. Cooking chickens into curries. Accounting spreadsheets into annual reports. Policing the guilty into jail. Lawyering the innocent out of jail. All sorts of betterments and bettermentations.

So, I need to do something today, because I need to do my bit to change things for the better.

### Money makes the world go round

Oh, and because you get paid.

People pay money for better things. And pay money to other people make things better. For example, people don't want to be sick, and hence pay a doctor to make them better.

So it's generally accepted that betterment is measured by money. The more betterment, the more money. If you find a way to make a lot of better for a lot of people, you can bring home a lot of butter.

### Feeling good about yourself.

But it's not just about the money. There's potential. — your potential. "Actualizing" all the potential you're endowed with.

Hence, if you can run, you must run faster. If you can study, study harder. And if you can cook, cook spicier. And do all of this to make things better. For bettermentation.

>>> "But why"[You say]

### But why?

Because you can be a good person. You can have all the good things people have. You can get married. Settle down in a nice house. Rare children. All of these required self actualization, bettermentations, and money. In other words, you need to do your bit and work.

>>> "But why"[You say, again]

### But why? (Revisited)

>>> "What if I have a different definition of a good person?" [You continue] "What if you don't need all the things "normal" good people should have?"

>>> "What?" [I say] "A different definition. Like what? What if you don't need money and the house, and all the other nice things? But then how will you live? Where will you find money? And what about selfing your actualization? And doing your bit?"

>>> "I have some money. Enough money" [You say]. "And I think my actualization is bit different from your actualization".

>>> "But what about doing your bit?" [I say] "And being a good person?"

>>> "Who says what a good person is? " [You say]

>>> "Good People" [I say]

>>> "And who says what a good is? " [You say]

>>> "Good People" [I say]

>>> "And who says they can say that? " [You say]

>>> "Good People" [I say]

At this point, you realize there is little point arguing with me, and go about your business.

[1] http://media.iwm.org.uk/ciim5/142/980/large_000000.jpg

#### Article 22 · December 10, 2018

# He said, she said

### Frustrations on "ABC (said XYZ)".

![Image](https://cdn-images-1.medium.com/max/800/0*lZfkPg5xwzsAG9be.jpg)

I just read yet another post from a friend (let's call them PQR) of the form "ABC (said XYZ)" where the post had no justification for the statement ABC, but one was supposed to accept it solely on the basis that person XYZ was learned, wise, knowledgeable, "an expert", popular, or simply a "good person" — whatever that means. The 90% of the social media traffic around Sri Lankan's ongoing Constitutional gymnastics falls into this "He said, She said" category.

My first reaction to this is frustration — especially when I don't agree with ABC, but also in cases when I do agree — but feel it lacks detail or nuance or context.

>>> "Why?" [You might ask] "These people are not posting under oath? Is a post like this significantly different from the memes, selfies, kitten, puppy, baby or other infant mammal pics and videos one encounters on social medial?"

You have a point. So why do I care?

This is why:

* An increasing number of people get their news, have their discussions and form their opinions on social media.

* This processes are predominantly based on "He said, she said" type data-points.

* This misinformedness leads to all manner of social, political and economic sins.

### Enter, Advocatus diaboli

>>> "But" [you say, for you're the Devil's Advocate] "I have the following objections"

>>> OBJECTION 1: What's wrong with data points of the form "He said, she said" ?

>>> OBJECTION 2: Suppose (for a moment) that we agree that something is wrong. But no one actually agrees with us, right?

>>> OBJECTION 3: Suppose you were right. And something was wrong with "He said, she said" — and everyone also agreed with you. It's not like we can do something about it, right?

### OBJECTION 1: What's wrong with data points of the form "He said, she said" ?

The problem with person PQR posting "ABC (said XYZ)" is that the truth of the statement ABC is anchored to the authority of XYZ. The visibility of this statement (in turn) is tied to the popularity of PQR. A special case of this is when PQR and XYZ is one and the same; the words and deeds of famous people get a lot of airing on social media.

The problem with all this is that XYZ is judged on authority and popularity; not rationality. An "authoritative" or popular person's lie is truer than an unknown person's truth. And this is, in turn, problematic, because truth is repressed in favor of popular lies, from the mouths of "authorities".

>>> "But wait" [You say] "Surely, you take medicine on a doctor's authority? How is this different from going to a doctor, and getting medical advise?"

Disagree! Going to the doctor's is very different.

* Doctors have qualifications. The institutions giving these qualifications are regulated. The said doctors and institutions can be sued if they malpractice. On the other hand, many commentators on the internet have dubious qualifications. The memes and sound-bites they produce are more like candy or cocaine, than a medical prescription; they give you a quick dopamine rush, are easy to hide, and have delayed and little understood negative effects. You can't sue an internet celebrity for lying or misleading. You can't even question or contradict them — because your reply will only be seen by your 10 best friends, and none of their 10 Million fans. To summarize, the medical profession has checks and balances (literally as well as figuratively). Social media does not.

* If you have a complex disease you can and should do some research, discuss at length, and even get multiple "second opinions". Given that health is important, most people are willing to put in the extra work. On the other hand, few people (deep down) really care about quality and truth on the internet. There is little checking, and validation. In other words, people take quality in the medical profession seriously. Few people take the effects of social media seriously, until the patient is already terminally ill.

### OBJECTION 2: Suppose (for a moment) that we agree that something is wrong. But no one actually agrees with us, right?

What exactly will we be agreeing on disagreeing on? There are a few different things.

* "He said, She said" make poor data-points

* Social Media has led to political, social and economic problems.

Now, most people will agree with 2, even if they don't completely agree with 1. The statements 1 and 2 are also different in that 1 refers to a specific aspect of social media, and 2 is general; and "political, social and economic problems" is easier to observe and measure than ""He said, She said" make poor data-points".

In fact, 2 is a delayed effect of 1 (and many quirks like it). This is difficult to measure without a lot of data, but many early studies already confirm it. Like smoking, the process of realization might be slow, painful, and punctuated with controversy. But the faster it happens the less people will die.

### OBJECTION 3: Suppose you were right. And something was wrong with "He said, she said" — and everyone also agreed with you. It's not like we can do something about it, right?

Let me answer this question by a series of cause-and-effect statements.

* What is the cause of "He said, she said" posts? They are engaging, and easy to create.

* Why is "easy to create" so popular? Because people are not penalized for being lazy. A puppy photo that takes 3 seconds to upload will get 100x more likes than a painfully researched blog or article written during the course of 3 weeks.

* Why are "engaging" posts popular? Because they result in people spending a lot of time on the platform.

* Why is "spending a lot of time on the platform" so important? Because the people can be monetized in the short term, and the metric "time spent on the site" attracts investors and advertisers in the long term.

>>> "Can you please get to the point?" [You complain] "How do you get rid of "He said, she said" posts?

Well you need to get rid of the causes of "He said, she said", as follows:

* Social Media platforms should reward long-form articles over short-form memes, pics, and tweets. More on this in [2].

* Social Media platforms should have more conservative expectations on revenue from advertising (note "conservative expectations" not "zero expectations")

### References

[1] https://medium.com/@nuwan.senaratna/black-or-white-d56dc119bed2

[2] https://medium.com/@nuwan.senaratna/deep-consumption-8c32fbd1633d

#### Article 23 · December 10, 2018

# Slaves of Evolution

### On Cognitive Biases and Meaning

![Image](https://cdn-images-1.medium.com/max/800/0*H14pRVTRKYNjL5ZE.jpg)

### The Origins of Slavery

In "The Art of Thinking Clearly" [1], Rolf Dobelli lists over 100 cognitive biases — or patterns where humans consistently behave irrationally. These biases exist for a good reason: they help us survive. In fact, we are here on earth today, not despite these biases, but because we have these biases. If not for them, we might not have survived. For example, many biases involve over-estimating risk; in other words we are irrationally risk averse. This is because being risk averse in a hostile, wild environment (like the African savanna, whence we spread across the planet) is a good thing. It's better to mistake a stick for a snake, than a snake for a stick [2].

Homo sapiens have roamed the earth for over 200,000 years, and for much of that time we have struggled for survival. It is only relatively recently (<10,000 years) that humans have started to dominate the planet. With this domination, humans have increasingly begun to introspect "rationally". We have tried to use logic and reason to understand the world. We have even begun to think of ourselves as "rational". In contrast, our mental machinery (our brain) hasn't evolved much in these many years. We still have a brain optimized for evolutionary survival, as opposed to cold rationality. Hence, the many biases Dobelli describes so well.

Many of the motivations and forces that govern our lives have evolutionary roots. For example, regardless how "modern", rational, and sophisticated we are, we still find food and sex immensely pleasurable. While we might be dining in a Michelin star restaurant, or moving to Vātsyāyana's Kamasutra, we are still, in essence, slaves of evolution. To survive we need to eat, hence we eat. To survive we need to breed, hence we breed. This is not to say that there is anything crude about beings that eat, sleep and have sex. We have generously embellished these acts with culture, history, spirituality, and even the divine. But there is no getting away from our humble origins.

### Slavery in the modern world

To what extent have we escaped from these origins? Not much, really. Today's archetypal "successful person" has the following two characteristics:

* Has a good job (or alternative sources of wealth) ensuring that he and his are well fed, well sheltered, and "well healthy".

* Has a family, ensuring that his genes are transmitted to the next generation.

In the times of absolute kings and emperors, the alpha males "family" consisted of harems of thousands of wives and concubines, more children, and millions of descendants. One study claims that 1 in 200 humans alive today are descendants of Genghis Khan [3]. Today, driven by better health, and a more equitable distribution of wealth, families tend to be much smaller, and uniform. On the other hand, the need for status, particularly a "good job" is stronger than it has ever been. Today's most "successful" people are powerful politicians and businessmen. And like their historical forefathers, they continue the tradition of making sure that they and theirs are well fed, well sheltered, and "well healthy".

It is not my intent to poke fun at institutions like the family, and aspirations like wanting a good career. These have ensured our survival. Instead my intent is to revisit the underlying motivations and goals — which are firmly grounded in evolutionary biology. If we are to take this path, we need to depend on some very primitive instincts and processes for all our motivation and meaning. In this sense, we are no different from animals.

But unlike animals, we have evolved minds, and this mind rebelling against its primitive roots. It is questioning its origins, and searching for new meaning. It has often "reasoned" in directions which are harmful (e.g. fundamentalist and violent sects and religions). It is constantly a source of stress and mental illness.

We are in a stalemate: We are increasingly trying to use a rational mind, to rationalize an innately irrational body. The animal and the human in us are at war. Something has to give.

There seems to be three paths forward.

* Go back to the animal in us. Accept that we are animals. Accept the innate primitiveness of our motivations and aspirations.

* Escape from the animal in us.

* Look for some middle ground. Accept that we are animals, but make use of this tool called a conscious mind.

Which path you take depends on what you want. Though, at the same time, what you want depends on what path you take. I find this "feedback loop" extremely unsatisfactory (Hence, the motivation for this article).

### End of Slavery (A Meta Solution)

To me, "End of Slavery" consists of finding a way out of this feedback loop. I don't have a good sense of what a "solution" to this problem might be, but I have a sense of the "characteristics of a solution" — or a "meta solution".

* We need to find something to "want" or "aspire to" (the "goal" of our solution)— which does not involve animal needs (like food and sex), nor the mind (which is essentially a product of these needs).

* Achieving the goal cannot make use of the "rational" mind, because it is flawed machinery, and not really rational.

* We can't trust other humans to tell us what the solution is, because speech and other forms of communication, and our brains that "understand" these forms of communication are flawed machinery. Hence, it has to be a solution that is self realized.

* We need to have some way of measuring the value of the solution. This measurement (like understanding), should also be "self-measurement".

* While we can communicate to other people about our solutions, we cannot be overly sure about the quality of our communication to these other people — again, given the primitive nature of our communication equipment.

* We cannot trust anything that promises results "in the future", because our notion of time, might be flawed by our animal brains. Hence, the solution must yield results in the present.

### References

[1] https://en.wikipedia.org/wiki/The_Art_of_Thinking_Clearly

[2] https://medium.com/@nuwan.senaratna/every-thing-we-think-is-wrong-and-thats-ok-d467a38d841b

[3] https://en.wikipedia.org/wiki/Descent_from_Genghis_Khan

[4] With apologies to https://en.wikipedia.org/wiki/Thomas_Becket

#### Article 24 · December 11, 2018

# On Programming

### What next?

### Programming 1.0 — Writing Textual Code

![Image](https://cdn-images-1.medium.com/max/800/1*xnaWJP9xiKrqnB9zjB1qSA.png)

The first programming language I learnt was BASIC — way back as a teenager. This was followed by Visual Basic, Pascal, C++, C#, Java, Python, PHP and JavaScript. Some languages came and went. Others went, and came back.

Despite this evolution, one thing did not change. The "code" consisted of text in a text file, and the "coding" happened on a text editor. Of course, there were fancy editors and even fancier "Integrated Development Environments" (IDEs). But the simple act of "writing code in text" seemed eternal.

### Programming 1.5 — Meta Programming

![Image](https://cdn-images-1.medium.com/max/800/1*Vj19XDUX6XtKyZwF0NFp9g.png)

Programming 1.0 or writing textual code, still dominates programming on most technology projects. However, there's also an interesting parallel trend — Meta Programming — or writing programmes that write other programs.

The best known type of programming is Supervised Machine Learning [1]. Programmers don't write the final code — instead, write meta programs (Machine Learning Algorithms) that take data and generate the final code based on this. This "final code" is known as a machine learning model, and is used to evaluate further new data.

You might argue that this is still Programming 1.0, with the human programmer writing the Machine Learning Algorithm as textual code. However, there are two important differences.

* The Machine Learning Algorithm can be reused with little modification, for different sets of data. Hence, the Compiled Machine Learning Algorithm (rather like a compiled utility library) remains unchanged, while the Compiled Machine Learning Model changes with the data.

* The actual "heavy lifting" (or processing) is mostly done by the machine generated (or meta programmed) Compiled Machine Learning Model.

I've labelled this meta-programming as 1.5, and not 2.0, because it still relies on 1.0, and is very much a parallel phenomenon, not a replacement.

### Programming 2.0 — Artificial General Intelligence, and the End of Human Programmers

![Image](https://cdn-images-1.medium.com/max/800/0*cpTSzaBZag1sKPWU.jpg)

What if there was a meta program that could learn from any data? And solve any problem? This idea has been referred to as "Artificial General Intelligence".

Artificial General Intelligence [3] is a "meta program" or a Compiled Machine Learning Algorithm that can learn from any data set. Hence, once this is written, there is no need for humans to write any more programs.

There are many doubts and concerns about when and how Artificial general intelligence will come about. I don't have enough original information to contribute meaningfully to this discussion. Instead, let me speculate on what might happen between now (1.5), and Artificial General Intelligence (2.0).

### Programming 1.75 — Or what next?

I wanted to write about, not Machine Learning or AI, but about programming. (For my thoughts on the "what next" in AI, refer to [4]).

How would things be different for programmers and in programming in the next few years?

* Meta Programming Beyond Machine Learning and AI. For everything from User Interface Design, Databases, Server Design, and Computer Networks.

* Minimizing redundant commands in programming languages. What is the minimal number of characters with which a program can be defined? This is all a human needs to type. And the rest can be machine generated. Programs will be shorter.

* Minimizing programmer error. The "boring" aspects of programming will taken over by machines, with humans doing the "creative" aspects. Things like debugging, testing, and quality assurance can be automated away.

* Beyond Text Editors. With "non-redundant" and creativity-optimizing programming languages, the advantages of a keyboard would be minimal. More visual-spatial-tactile interfaces are likely to "inspire" programmers more.

* "Informate" [5] programming. Humans and machines will be programming in parallel. Machines will process less-creative-more-processing-heavy code, while humans will create more-creative-less-processing-heavy code.

### References

[1] https://en.wikipedia.org/wiki/Supervised_learning

[2] https://pixabay.com/en/photos/artificial%20intelligence/?

[3] https://en.wikipedia.org/wiki/Artificial_general_intelligence

[4] https://medium.com/@nuwan.senaratna/the-briefest-history-of-ai-def2a34ab883

[5] http://www.layoftheland.net/archive/web/mis-575/course_docs/topic_5/zuboff.infomate.pdf

#### Article 25 · December 20, 2018

# Upgrading vs. Evolving

### A Prelude and Fugue

![Image](https://cdn-images-1.medium.com/max/800/0*sS3RRe0j6y4FIeX9.jpg)

### Prelude: Definitions

* Evolving: Optimizing an entity, by making many copies of the entity each with small changes, then destroying those entities that are less optimal, and continuing the process with the entities that are more optimal.

* Upgrading: Optimizing an entity, by making a specific set of well defined changes to it, known to make it more optimal.

### Fugue: Aphorisms

* Means and Ends. To Upgrade, both ends and means must be known. To Evolve, only ends needs to be known. In practice, often neither ends nor means are known.

* Knowledge. Understanding the means of solving a problem, is much harder than understanding the nature of a solved problem (which is usually the same as understanding the problem). Hence, knowing how to upgrade is almost always harder than knowing how to evolve.

* Justification. An upgrade can be justified, by explaining how the improvement improves fitness. The only justification of evolution is that "it works". The justification of an upgrade is easy to communicate, but rarely valid. The justification of an evolution is often valid, but difficult to communicate.

* Hindsight. The result of evolution over many generations can be described as an upgrade of a single step. However, such descriptions are usually incomplete, and the correlation often lacks causation.

* Generations. Upgrading involves improving the fitness of an entity within a single generation. Evolving involves destroying the entities of one generation, so that the next generation might be slightly fitter.

* Cruelty: When the entities and generations involved are human, evolution is cruel, despite being effective. Hence, often Upgrades are chosen as a less cruel (but also sadly, less effective) alternative. For example, many strong nations have emerged out of centuries of hardship. However, hardship is never prescribed as a path for economic development. Instead, economist design various "Upgrade playbooks".

* Scale. Evolution favours small scale, while Upgrading favours large scale.

## Appendix: References

* [OED] https://en.oxforddictionaries.com

#### Article 26 · December 25, 2018

# On Clean Humour, Comic Faiths, and Serious Denial

### Questions based of a Venn Diagram

![Image](https://cdn-images-1.medium.com/max/800/1*60pTLBGvJaJ7myzd3s58Tw.png)

* GREEN = Set of ideas which you accept as true

* RED = Set of ideas which you are open to make fun of, or ridicule. By "not open to" means that you would want any person making fun of or ridiculing these ideas punished.

* BLUE = Set of ideas which you can justify in a manner that most people will find acceptable.

I have also given various parts of the Venn Diagram labels. Please consider these labels as "nothing but labels", and answer your questions based on the definitions of the sets.

### Questions

* For each of the labels (Comic Truth, Serious Denial etc), what are some example that intuitively (but not analytically) come to mind?

* Can you justify your "Serious Truth" candidate? Why are you not open to exposing this idea to fun or ridicule? I.e. why are you not open to classifying this ideas as a "Comic Truth", and why do you want to punish people making the jokes?

* What are some ideas which might be serious truths to some people, and serious facts to other people?

* What do you think is the best idea in the universe? Where on the Venn Diagram would this idea go?

* If you could move all the ideas in one group into another group, what would these groups be?

* Do you feel that this Venn diagram misrepresents idea? If so, why?

* What effect does society have on your choice of group?

* If you could do so anonymously, would your classification of ideas to groups be different?

#### Article 27 · December 27, 2018

Good point. I agree.

#### Article 28 · December 27, 2018

RE: Neocortex

What were the engineers who developed the adaptive software actually goaled on? Was it the same (survival) goals as the remaining more primitive parts of the brain, or was it a set of different goals?

My intuition is that the Neocortex is not actually better software, but better hardware. I.e. more RAM, and (possibly) better internal busses.

#### Article 29 · December 31, 2018

# Happy 2019!

### Contemplations

![Image](https://cdn-images-1.medium.com/max/800/0*FJsaThBQS0apr-6B.jpg)

"Is there such a thing as past and future?" [I contemplate]

"Of course there is", [you say]. "We studied the past for history."

"And as to the future", [you continue]. "It must exist — because in the past, the "present" (which we know exists) was the future. So there."

But what is history? An honest study of the past, or nit-picking the present to unearth pieces of "evidence" that might support biased pronouncements about the past? And predictions about the future? Are they any more accurate than "predictions" about the past?

What I really want to say is this: For approximately 365 days, the "present" will be 2019. The past and the future are inaccurate at best. So I hope we all make the most of the only thing that is not past or future: The present.

Happy 2019!

#### Article 30 · December 31, 2018

# Meta Resolutions 2019

### Or Properties of Resolutions

### On Goals

* Be present, at all times.

* Be mindful, at all times

* Be kind, and compassionate.

### On Letting Go

* Let go of prejudices, conventions, and traditions that have no justification but ego.

* Let go of shallow stimulation, shallow excitement, shallow w distractions, and shallow consumption.

* Let go of time, past and future.

* Let go of the need to give things names, generalize and abstract.

### On Contemplating

* Contemplate, don't think.

* Create

* Journey

Happy 2019!

![Image](https://cdn-images-1.medium.com/max/800/0*cHXAk5fRI1ugJ12F.jpg)

[wabiSabi] https://www.flickr.com/photos/lacatholique/5098514073

#### Article 31 · January 3, 2019

# Mind Minding

### Confessions of a Meditator

I'm sitting, soundless, breathing deep,

Upon my belly, upturned hands,

As one would in the blinds of sleep,

My mind drifts towards foreign lands.

And as I see this misdemeanour,

My mind's misconduct, growing keener,

It breeds upon a world of nothing,

Unseeing that goal that is upcoming...

It tries to run away again,

So like an arrow unleashed now,

One from a bow-string made of bough,

It tries again to break its chain.

As I sit still and try to mind,

My mind, my mind is unaligned.

...

It dreams of dreams gone by and by,

It dreams of futures burning bright,

Like lakes and castles in the sky,

It dreams of dreams if can't rewrite.

And sounds and colours through my eyes,

That chance upon my mind like lies,

It names them — often simple words,

Turn black to white, and bees to birds.

And as my body runs away,

My mind in panic throws a fright,

Like armies glimpsing foes in sight,

It pounces like a beast astray.

And Like a demon unexiled,

It celebrates its triumph wild

...

But I keep going, unconcerned,

About the concerns of my mind,

Its little wins, its bridges burned ,

I turn away. I leave behind.

The need to name things, abstract thoughts,

The need to judge things, casting lots,

With this or that thing right or wrong,

A word less poem, A soundless song.

And with each sitting, I feel calm,

Some good to do, some good to feel,

The pain that gathers head to heel,

Is like a soothening touch of balm.

And with each sitting, my mind unchains,

A bit by bit, like drops in rains.

#### Article 32 · April 3, 2019

# On Ideas

### Aphorisms

## On those who eat at other tables

![Image](https://cdn-images-1.medium.com/max/800/1*VaSlh00XjAepcqLZIStSnA.jpeg)

* A parasite is an entity that depends on another entity for its survival.

* DNA is a parasite, because it "survives" through the survival and reproduction of its host organisms. The organism might die, but the DNA survives in the organisms offspring.

* Ideas are also parasites. They live in the minds of people, and occasionally in other mediums like books, art and engineering.

## On surviving through survival

* Ideas survive through the survival of their hosts, and they often continue to "survive" after their hosts have died or have been destroyed, or are "like not cool any more".

* For a parasite to survive, it needs to live in its host long enough for the host to propagate the parasite to the next generation.

* (Until then) For a parasite to survive, it must be able to cohabit with its host, and promote the host's survival.

## On the two methods of human reproduction

* Human Ideas survive through Human reproduction. There are two methods of human reproduction: 1) Breeding children; 2) Breeding students, disciples or followers.

* Almost all humans are suited to breeding children. Our parasitic DNA enforces this. DNA that led to humans that were less likely to breed would not have survived.

* On the other hand, only a few humans are naturally suited to breeding students, disciples or followers.

* Both methods are effective. One is significantly more asymmetric than the other. The Buddha had only one son, who himself had no descendent. Conversely, there are over half a billion humans alive today who claim to be students, disciples or followers of the Buddha.

## On books, art and engineering

* Ideas are intellectual concepts, and need to be understood by their host humans. Hence, simple ideas are more likely to survive in human mediums, compared to more complex ideas.

* Complex ideas tend live in books. Many also tend to die in books.

* There are two types of books: Books that host many ideas, and books that repeat the same idea many times. The latter almost always outlives the former.

* Art is the art of making ideas beautiful. Art hosts ideas in a manner that is beautiful to the humans that surround it. Hence, those humans have an incentive to help that the art survives.

* When analysing a book, or a piece of art, or a bridge, it is difficult to judge whether the ideas they host are good or bad. On the other hand, it is easy to measure how long they have survived.

* The expected lifespan of an idea is proportional to age. Old ideas have longer life expectancies than newer ones, and are more likely to survive even longer.

## On intolerance

* All parasites compete for hosts. As do ideas.

* Ideas that help their hosts dominate others of their kind tend to survive more than ideas that don't.

* Ideas that are intolerant of other ideas tend to survive longer than tolerant ones.

* The ideas of liberalism, tolerance and intellectual freedom, that are promoted as representative of our age, are significant anomalies, considering broader human history. For almost 99% of our history, humans have been illiberal, intolerant, and intellectually bankrupt.

* There is no evidence or reason that this anomaly should survive long. It is either an anomaly, or these ideas are themselves in a schizophrenic and parasitic coexistent with a set of very different ideas.

## On the schizophrenia of ideas

* For a tolerant idea to survive it has to be coupled with an intolerant one, which enforces its survival.

* Liberalism has historically parasited itself on a conservative, white-centric and nationalistic host. More recently, this host has been replaced by a Neo-liberal and increasingly Alt-Left/Anti-fa host.

* Religions with a core of peace and tolerance (e.g. Buddhism, and New-Testament Christianity) have depended on nationalism and autocratic ideas for support and survival (e.g. For much their history, all majority Buddhist countries were autocratic monarchies which autocratically supported Buddhism). This is the only way these "tolerant" ideas can survive in the light of intolerant ideas (e.g. Religions that condone the enslaving, mistreatment, and killing of non-believers).

* Academic institutions that worship intellectual freedom, often have highly intolerant, and out-of-date administrations that suppress new ideas, in the interest of a narrow status quo, and a small set of "acceptable" ideas.

## Concluding thoughts

* Ideas must be seen for what they are: Parasites that have an ulterior motive — Survival. Both good ideas and bad ideas have this motive.

* It is easy to confuse a good idea, with one that has merely survived a long time. ("When a thousand people believe some made-up story for one month, that's fake news. When a billion people believe it for a thousand years, that's a religion" — Yuval Noah Hariri [2])

* There are many good ideas, e.g. Liberalism, Tolerance, Intellectual Honesty, that are generally bad at surviving — and might not survive for much longer. That does not make them bad ideas which are unworthy of a host.

References

[1] https://en.wikipedia.org/wiki/DNA[2] https://www.theguardian.com/culture/2018/aug/05/yuval-noah-harari-extract-fake-news-sapiens-homo-deus

#### Article 33 · May 13, 2019

# I believe. I identify. I label — Not.

### A pledge.

![Image](https://cdn-images-1.medium.com/max/800/1*s4ZL8C-jaqwqj2okKZ5GCg.jpeg)

## Belief

There are things we know to be true. There are things we know might be either true or false. When we say we "believe" something, we choose to treat something that could be true or false (often false) as true — as something we "know".

The world is complicated. And there are many things we do to simplify this complicated world. "Beliefs" are simplifications. Ancient humans didn't know if the sun would rise tomorrow. Hence, without worrying, they chose to believe that each day a Sun-god drives his chariot over the skies.

## Identity

"Identity" is another such simplification. I "identify" as all sorts of things: Male, Sinhala, Sri Lankan, Buddhist, Computer Scientist, Musician etc etc etc. These identities, to some extent, describe me, and are, to some extent useful. For example, my "Male" identity tells me which lavatory to use in a public place. At the same time, these identities tend to over-simplify me — they don't, even in aggregate, capture who I actually am.

Believing in something doesn't make it true. Believing in a Sun god doesn't generate, or create a Sun god. In that sense, belief does not change the world. But it does change the believer. In fact, it is the first thing that is changed. When a believer believes, he or she acquires an identity — that of the group that believe.

Hence, some identities stem from belief. For example, if you believe in the four noble truths, or the three characteristics, and act accordingly, you might call yourself a Buddhist.

But do all identities stem from identity? What about Sinhala or Male? Surely, these are facts?

All humans are supposed to have evolved out of Africa, moving to Asia and Europe, and then Australia and the Americas. A few moved to the Island of Sri Lanka, and over time, established an ethnicity and culture we call Sinhala. I don't know the exact date on which "Sinhala" came into being — there must have been some day where one could say "Today there are Sinhala people. But yesterday there weren't". I don't know. What I do know is today, myself and another ~15 million humans identifying with this ethnicity and culture call themselves "Sinhala".

But surely, you might say, "Male" is a "fact" isn't it? If one has an XY chromosome pair, one is male. But it's not that simple. When most of us think "Male", do we think of chromosomes? It's more likely that concepts like "behavior", "dress", "likes", "dislikes" come to mind. I know for a fact that I have an XY chromosome pair. But I don't "know" that I should where trousers, instead of skirts — Or prefer blue to pink*, or women to men. These are all preferences I have "identified" with.

[* Pink for girls, and Blue for boys is a relatively new phenomena. In many older contexts, these colors are reversed. For example, in the Catholic church, Pink is often associated with males — cardinals and Christ, while blue is associated with females — the Virgin Mary, and nuns].

Computer Scientist and Musician are even weaker identities. Does a degree or a diploma in some subject confer anything of meaning on one? Neither Alan Turing nor Mozart had degrees is Computer Science or Music.

## Labels

In the end, beliefs and identities are labels; labels that simplify the world. They are illusions that make us assume that the world is simpler that it is. Some of these assumptions can be very dangerous. For example, we might assume that some people are evil, and others are good. That some deserve our compassion and kindness, but others don't. That some people are, innately better, or superior, or more worthy of our respect.

There can be no true understanding, as long as we rely on beliefs, identities, and labels.

## Concluding Pledge

This article is actually a pledge; A "pledge of letting go" which I want to take in front of you all, my friends.

>>> "I pledge to let go of all beliefs, of all identities, and all labels."

Of course, such a pledge is easier taken and observed. I'm likely to break it often. Hence, it will need constant retaking and renewal. But at least, I hope, it will be a start.

#### Article 34 · May 14, 2019

# On News

![Image](https://cdn-images-1.medium.com/max/800/1*GbnY1r2of2IU7IN_mGHNWA.jpeg)

## Ancient Times

In the beginning, humans lived in small groups — perhaps a few dozen people — a hundred at most. Everyone knew everyone. "News" consisted of what one person told another person — and was exclusively about things that happened in the group. The "Latency" or "Speed" of news was determined how fast a human could travel. The "Bandwidth" or "Volume" depended on what a human could remember.

For 1000s of years, not much changed. Latency got a little faster as news was carried by animals (horses and pigeons), and then physical machines (trains). With the printed word, the "precision" of news improved. But "Latency" and "Bandwidth" were within an order of magnitude of pre-historic times.

## Three Step Changes

Then, around 200 years ago, the invention of the electric telegraph changed latency forever. What was previous limited to the speed of a man, horse, pigeon or train, now travelled at the speed of light.

The second step change came about 20 years ago, with the invention of the internet. "Bandwidth" and the volume of news was now almost infinite. But telecommunications were still expensive.

The third step change came a few years ago, with the rise of digital advertising. Suddenly, many people could transmit infinite amounts of data at the speed of light — for free — paid for by advertisers buying their attention and data.

## Nostalgia

We lament that ours is an era of #FakeNews and journalism that cares only about #ClickBait and #impressions. In reality, the issues is that the third step change has changed the world, and, driven by this change, news, media and journalism is having a crisis of identity.

Was news actually better 20 years ago? When a few governments and big organizations had a monopoly over its content? When the world of a few journalist was the word?

I'm not going to express an opinion on this — nor claim to be nostalgic. Instead, I'll pose a set of hypotheses:

1. News is a byproduct of its technological context. Each step change, changed that context, and with it News.

2. If we want to change news, we need to change the context

## Concluding Questions

Would any one of you agree to any of the following? I don't necessarily agree or disagree with any of them. They just happen to be interesting questions.

1. Would you go back to a world where news is controlled by a small number of governments and big organizations?

2. Would you go back to a world where either a) News has high latency, or b) News has low bandwidth, or c) Transmitting news is expensive?

3. What might a fourth step change be?

4. If news is going to be a victim of the third step change, what will its other victims be?

#### Article 35 · May 16, 2019

# The Knife of Thought

### Confessions of a wannabe Non-Entity

![Image](https://cdn-images-1.medium.com/max/800/1*s-Ge8B6EHrgvMXbM4ED-0Q.jpeg)

>>> "I think X".

Whenever one thinks of something (e.g. X = "I had a good breakfast"), one cuts the universe into two parallel universes.

1. The universe where breakfast was good

2. The universe where breakfast was not good

In the simplest of cases (e.g. "I think 1 + 2 = 3"), one or the other might be true. But in most cases, one or the other, or both or neither might be true.

Hence, the process of ones thought "cuts" the universe into two parts, and disposes of one in favour of the other. In a sense, it shrinks (or narrows) ones universe.

## Example: Cogito Ergo Sum (René Descartes)

>>> "I think, therefore I am"

This statement should actually be, "I think, I think, therefore I think I am" — because it is the same thought process that supposes "I am" — not some other, absolute, independent logic.

There are at least two cuts happening here.

1. Cutting the universe into one where 1.1) René thinks, and 1.2) René does not think

2. Cutting the universe into one where 2.1) René is, and 2.2) René isn't.

Hence, the universe is cut into four parallel universes, of which one is favoured, while discarding three. Note, the world where "René is, but does not think" (whatever that means) is also discarded.

[Note, this process need not stop here. "I think, I think X" could be expanded to "I think, I think, I think X" and so on. Hence, the fallacy of Descartes and the fallacy of thought is this innate recurssiveness. This "thought" would never conclude anything.]

## Binary Logic

Thought is bound to binary logic. For a cut to be successful, the negation of thought (E.g. "I did not have a good breakfast") has to be completely discarded. The possibility of the thought and its negation co-existing is not possible.

Before "I thought", the universe could have accommodate both "good breakfast" and "not good breakfast", or even neither. But not after thought.

Binary logic is dangerous because it misleadingly implies that the thought and its negation are somehow equal in volume and scope. Too often we only understand one (thought) and assume that the other (the negation of thought) can be understood completely through thought.

For example, when we say "He is a terrorist", we assume that this thought is completely sufficient to explain the world. We are happy to reinvent the world to match our thought. We don't stop to think of the implications of "He is not a terrorist" and the implications that might have at also explaining the world.

Hence, when we choose "to think", we choose to identify with a simplification of the world. Too often, we call this simplification "knowledge" (and sometimes other things like "belief"). Somehow the respectability and profoundness of words like "knowledge", seems to confer some respect to our thoughts. However, this is misleading. Whenever we choose to identify with knowledge, we are choosing to identify with a simplification.

## Identity

Identities like religion, race, ethnicity, nationality, gender etc, all require thought. I have to think I am a Buddhist or Sinhala. Without this thought, it does not "occur" naturally. I don't "feel" my identity the way I see, or hear, or smell, or feel.

Hence, all forms of identities are also cuts of thought. When I say "I am a Hindu", I'm actually saying "I think, I am a Hindu". There is no other way of making sense of the phrase (I think). The universe is cut (and shrunk) into one where "I am a Hindu" — the remainder (in my mind) is discarded.

## Non-Identity

To belong to an identity, we need "to think" certain things. For example, the Catholic Apostles' Creed has a set of beliefs starting with "I believe in God, the Father almighty, creator of heaven and earth.".

[The line between knowledge and belief is a fine one, and for the purpose of this article — they are one and the same]

Whether it is the Catholic religion, or any other identity, we choose to identify with knowledge (or one of its many equivalents, like belief). What if we could identify with everything that we don't know instead?

Such an identification cannot be expressed in a creed, or set of rules, or theorems, because if it could be, it would itself become knowledge or belief. Hence, this "Non-Identity" consists of an openness of mind to everything that is not known — which is (rounded for practicality) 100% of the universe.

## A Non-Entity's creed

1. I will think as little as possible (most thought is useless anyway)

2. When I do think, the thought process will be governed by loving kindness, compassion, empathy, and equanimity.

3. When I do think, I will not "identify" with that thought. I.e. it's a thought. Not "me".

## Update 5/31/2019: On the inclusion of Buddhist Values

>>> "2. When I do think, the thought process will be governed by loving kindness, compassion, empathy, and equanimity."

When I first wrote this, I too was aware that the unexplained inclusion of "Buddhist Values" would be somewhat jarring. I was also aware that I was not writing down what I intuitively wanted to convey. Hence, I spent some time contemplating this point, and have come to a slightly different conclusion.

I started with trying to understand the relationship between "thinking" and these "buddhist values" which are also known as the Brahmavihara [1]. The all seemed to follow from the Buddhist "three marks of existence"[2], namely impermanence, unsatisfactoriness and non-self. For example, the realisation of non-self helps one realise that all other beings as are ones self, leading to unlimited loving kindness. An appreciation for another beings impermanence and unsatisfactoriness leads to compassion. Empathy and Equanimity are similarly driven by a realisation of a combination of these makes.

The key connection with "The Knife of Thought" is as follows: Not to realise impermanence, unsatisfactoriness and non-self, necessarily requires thought. For example, to identify with self, requires thinking about a "me"; to see something as permanent is an assumption of thought, as is the assumption of satisfactoriness. Freeing oneself of thought necessary frees one from ignorance of the marks, and whatever remains would be consistent with loving kindness, compassion, empathy, and equanimity.

Hence, I should have said:

>>> "2. When I do think, I will be mindful of any thoughts which oppose loving kindness, compassion, empathy, and equanimity."

[1] https://en.wikipedia.org/wiki/Brahmavihara

[2] https://en.wikipedia.org/wiki/Three_marks_of_existence

#### Article 36 · June 13, 2019

# Where to locate an office in Colombo

### A very rough analysis

A friend and I were debating on the pros and cons of various locations around Colombo for locating offices. Traffic was an important determining factor, and the optimal location was that which as many employees could travel to and from with least difficulty.

To quantitatively augment our mostly qualitative discussion, I did a Google Maps API search, for a selection of office locations, on how long it takes to travel to that location from various parts of Greater Colombo, during the morning rush hour around 8am.

The selected "office locations" were:

* World Trade Center, Colombo 1

* Thummulla, Colombo 7

* Narahenpita Junction, Colombo 5

* Dehiwala Junction, Dehiwala

* The Parliament, Sri Jayawardena Pura Kotte

* Malabe Town, Malabe

This is what I got.

![Image](https://cdn-images-1.medium.com/max/800/1*qsvZ-vUiLOQ76baLETgNjg.png)

The colour legend is:

* Blue < 15min

* Green 15–30min

* Yellow 30–45min

* Orange 45–60min

* Red 60–90min

* Dark Red 90–120min

* Black >120min

![Image](https://cdn-images-1.medium.com/max/800/1*56GP73FHtoZOGanCfsIjdA.png)

![Image](https://cdn-images-1.medium.com/max/800/1*o-0UktsPm3T3uqlhyTfhpw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*N86QQMumpsiekWDwYIZTZQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*fFiQrraIS0hvvxy4CJxVkw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*16mlSjepxYfqLF4EsjyGdA.png)

## Caveats

* "The optimal location was that which as many people could travel to and from with least difficulty" — this visualization only factors travel time. It does not factor the density of population, and hence travel volume of various locations. One location could have a large "quick to travel" zone (Blue/Green), which is sparsely populated, while another location could have a small "quick to travel" zone which is densly populated, and hence with more travel volume.

* The data does not factor in non-traffic features, like proximity to amenties, proximity to customers, "nice neighbouhood", etc.

* Travel time only factors one direction of travel (to work around 8am), and does not factor in travel to and from customer/client offices during the day, and the return commute at the end of the day. Also, many people increasingly travel at unorthodox hours to beat the traffic (probably any time from 4am to 12noon).

#### Article 37 · June 21, 2019

# On Employee Performance Management (EPM)

### A Short Playbook

## Why EPM?

Everything a business does is focussed on maximizing its long-term value (LTV). "Maximizing LTV through managing the performance of employees" is an important subset of this focus. Also, compared to mature companies that have built significant customer brand, this subset is disproportionately important to start-ups, as employees (particularly founder employees) play a disproportionately important role in its direction and success or failure.

## Why "Sophisticated" EPM?

Very often, companies make the mistake of over-depending on monetary compensation for motivating employees and "keeping them happy", when there are many levers that can and should be used simultaneously. These various "levers" could be framed in terms of "Maslow's Hierarchy of Needs" as follows:

* Physiological/Safety. Salaries, Benefits

* Love/belonging. Treatment from colleagues, particularly superiors

* Esteem. Acknowledgement and Recognition

* Self-Actualization. Personal Growth

"Sophisticated" Employee Performance Management would use all these levers, not just the first.

![Image](https://cdn-images-1.medium.com/max/800/1*gwgZRC1t7JueVnczLPZfYw.png)

## Characteristics of Good EPM

* Alignment with LTV. As described above, EPM is primarily a tool for optimizing LTV. Hence, all carrots and sticks associated with EPM should be aligned with LTV. How to weight the short, medium and long-term is an open question — but too often organizations overly optimize for the short-term.

* Fairness. A good way of differentiating a company with a good EPM and a bad EPM is to ask an employee why they think another employee gets paid more, and particularly if the latter deserves it. In other words, EPM must be seen to be fair.

* Simplicity. A business can't afford to let complicated EPM (and other "support" processes) distract from its core operations. Also, a system that is difficult to understand is rarely seen as fair. Finally, since EPM is both art and science, simplicity is one way of avoiding false precision.

## The Process

A good EPM system will have the "Good Characteristics" and also use all the "Levers of Sophistication".

* Best guess "LTV picture". EPM starts with a best-guess-timate of the companies LTV, and how various projects will contribute to this. The picture will consist of well-defined tasks, looser projects, problems with no specified solutions, known problems currently "unsolvable" and unknown problems.

* Assignment of work to people. To do EPM well, there must be a clear assignment of problems to people. Everyone must know what is expected of them. They should see both their work as yielding meaningful LTV, and as an opportunity for them to grow personally (i.e. Self-Actualize). Note, this assignment process can happen in a distributed manner. For example, a large project can be assigned to a tech-lead or engineering manager, who in terms divides the work further.

* Progress Measurement and Feedback. Often, and lightweight. Performance reviews (both formal and informal) are good opportunities for real-time acknowledgement and recognition (i.e. Esteem).

* Rewarding performance. Bonuses and Promotions. Promotion levels and performance ratings, unambiguously tied to salary bands, and are a useful tool for making bonuses and promotions simple to understand.

[1] https://en.wikipedia.org/wiki/Maslow's_hierarchy_of_needs

#### Article 38 · June 23, 2019

Great Question. Thought it deserved its own mini-article: https://medium.com/@nuwan.senaratna/on-stack-ranking-b6d93f07a107

#### Article 39 · June 23, 2019

# On Stack Ranking in Performance Evaluation

### Some brief thoughts, from my days at Facebook

What I understand by the "Stack-ranking approach" is "sorting" all employees in order of performance, and rewarding/punishing them accordingly. The most extreme example of this was practiced by Jack Welch (CEO of GE), where the top 10% performers were promoted, and the bottom 10% were fired.

Stack-Ranking has at least two serious problems

* Complexity. Performance is complex, and multi dimensional. Hence, it is difficult to sort people, because sorting implies that there is one numerical dimension which can be used for the sorting process. For example, Facebook engineers were evaluated on 4 qualitative dimensions (each with many sub-dimensions)

* Hostility. Stack-ranking creates very hostile and unhealthy relationships between co-working employees

These two problems result in very dysfunctional organizations — hence my dislike.

At Facebook, we evaluated engineers on an individual basis on their own merit. However, we did do the following exercises to make sure that the system was fair.

* Guidelines: Engineering Levels (E3, E4...E10) had detailed descriptions, explaining what is expected of an engineer at a certain level. Within each level, there were similar guidelines for ratings (Meets Some Expectations, Meets Most, Meets All , Exceeds, Greatly Exceeds, Redefines). There were also case studies and mock descriptions of engineers and their ratings.2

* Calibrations. As part of the performance evaluation process, Engineering managers met in groups and discussed similar employees. For example, two E3 (junior) engineers working in a similar area (e.g. Front End Product Development) who are both "exceeding expectations" should have comparable performance. If one looks significantly better than the other, then there might be something wrong.

* Statistics. As the company got bigger, the distributions of how many people got promoted, and the ratings people got were compared across the company, to make sure that they were roughly similar. If a part of the company looked significantly different from the rest, then there would be some investigation as to why, and in some cases engineering managers would be asked to re-calibrate their ratings and promotion decisions. This process was sometimes interpreted as "Stack-Ranking", but I see it mostly as a process to ensure fairness across the company. Note, the statistics involved comparing aggregated statistics for 100s of employees.

DISCLAIMER: I worked at Facebook from 2009 to 2017. My observations are from this period, and specific to the Engineering organisation. I don't have as deep a knowledge of practices in other organizations like Sales/Marketing etc.

#### Article 40 · June 27, 2019

# The Middle Path

### A Philosophical Algorithm

![Image](https://cdn-images-1.medium.com/max/800/1*nXzBMhKx0B0bcl6c4dhmTA.jpeg)

## Inspiration

Many philosophies (including Buddhism) have the "Middle Path" or the "Middle Way" as a core idea. However, I was inspired to write this article by the following series of news stories that I happened to read or watch in the last couple of weeks:

* Why did 52% of Brits vote for Brexit? The Indian yogi and author Jaggi Vasudev described Brexit as a backlash against "a pendulum" which was pushed too hard in the direction of "right".[1]

* The two sides of the Abortion debate (Pro-Life vs. Pro-Choice) are increasingly becoming more and more extreme. And like many Left vs. Right debates, there is increasingly less opportunity for a mutually acceptable compromise. [2]

* One party in a coalition government is severely criticized for negotiating and compromising on policy with their coalition partner [3]

All these scenarios have a common theme: A complex issue, which has been over-simplified by accepting one narrow view to be completely right, and the other (or all others) to be completely wrong.

## The Middle Path Algorithm

While the above scenarios might sound annoying or even stupid, they are common, and like most cognitive biases, have a common cause. Simple ideas are always more popular than complex ones, because they require less brain power to process. This might have been an advantageous evolutionary strategy when we were living simples lives on the African Savana, but it doesn't work in today's complex world.

To prevent myself from falling into similar traps, I thought of the following "Middle Path Algorithm":

>>> For any idea, concept, opinion, or fact (let's call it X) that one is thinking about, and might be inclined to accept, consider the following:

>>> Is X right? Why? What are the consequences of X being right?

>>> Is X wrong? Why? What are the consequences of X being wrong?

>>> Can X be both right and wrong? Or neither right nor wrong? Or some state of rightness or wrongness in between? Why? What are the consequences of X being in such a state of rightness or wrongness in between?

>>> Recursively apply this algorithm to any other ideas emerging from this process.

The goal is simple: To look at an idea from all angles and points of view; not just one.

## Pros of the Middle Path

The Middle Path provides immunization against the following diseases, by driving a contemplation of what lies between extremes.

* Premature Thought: Thought is a knife [4]. The moment we "lock in" to a view, we split the world into two universes, one where the view is right, and another where it is wrong, and accept the former as "truth", and the latter as "false". Very often this choice is simplistic, and the "cut" premature. We narrow our minds, without sufficient investigation

* Nit-Picking: Once we lock into a view, we have to support it and "back it up". Often the facts we have at hand are insufficient, or are not convincing. So we nit-pick ones which support our view.

* Ego: And as this insufficiency and unconvincingness exacerbates, we need to reinforce whatever facts with our egos. Suddenly, an attack on our view is a personal attack on ourselves. And before we know it, we are down the slippery slope of identity groups, "being offended", political correctness and worse.

* Lack of Compromise: It is natural for ideas to compete and contradict. Often two good ideas might be mutually contradictory or even exclusive. Compromise or choice is inevitable, and possibly optimal. Often such compromise is shunned because we live in a "one or the other" world.

## Cons of the Middle Path

Applying "Is X wrong? Why? What are the consequences of X being wrong?" to the Middle Path, the following objections come to mind:

* Sound-Bites: The middle path is poor at generating simple ideas, sound-bites or click-bait. This might sound a good thing, but it makes for poor social media memes, and political speeches. Don't expect a student of the Middle Path to be the next hot new politician, or social media influencer.

* Strong Ideas: It leads to weakly held views. In today's world of strength and strong opinions, many (including many of my friends) found this a "con".

* Evil: It condones "evil" and other bad things. "Hitler, Pol Pot, Stalin....etc were definitely evil weren't they?" you ask. How can anyone argue against that? Well they could. But it would be complicated. To start with, such an argument would begin with "Evil is ABC", and that itself would lead to too many contradictions.

## Concluding Exercise

If you're not convinced about the Middle Path, try considering the following:

>>> Is the Middle Path right? Why? What are the consequences of the Middle Path being right?

>>> Is the Middle Path wrong? Why? What are the consequences of the Middle Path being wrong?

>>> Can the Middle Path be both right and wrong? Or neither right nor wrong? Or some state of rightness or wrongness in between? Why? What are the consequences of the Middle Path being in such a state of rightness or wrongness in between?

### References

[0] https://www.flickr.com/photos/binnyva/26578847920[1] https://www.youtube.com/watch?v=pvcV7kixo1Y[2] https://www.economist.com/leaders/2019/05/16/a-majority-of-americans-want-abortion-to-be-legal-in-the-first-two-trimesters[3] https://www.youtube.com/watch?v=jiK2oWENLHY[4] https://medium.com/@nuwan.senaratna/the-knife-of-thought-7f29ac4e24f9

#### Article 41 · June 28, 2019

# On Time

### 7 Philosophical Conjectures

![Image](https://cdn-images-1.medium.com/max/800/1*8XYp9RSVmWeMp6D1WhnYMA.png)

In his fascinating book, The Order of Time [2], physicist Carlo Rovelli discusses how most of physics is independent of an "order" of time (i.e. a differentiation of past, present and future). While he describes entropy as an exception (entropy can only increase as time passes), he goes on to point out that entropy is a relatively arbitrary concept, that vanishes at quantum levels.

Inspired by this book, I wanted to share some of my own speculations about time, and particularly its relationship with information.

### Conjecture 1: The Relationship between time and information

The present is the past with the addition of some new information.

For example, suppose one tosses a fair coin. After the coin is tossed, one bit of new information (namely "which way the coin landed"), is added to the universe.

Symbolically,

![Image](https://cdn-images-1.medium.com/max/800/1*jwA3ebizWbA3nsX4C1jJMw.gif)

Aristotle described time as a passing of events, that the difference between the past and present was that the present had witnessed more events, and that, independent of events, time was meaningless. There is an interesting parallel in making time dependent on events, and on information. Isaac Newton, on the other hand, described time as an absolute, that passes independent of events. This latter view has dominated physics, until recently when Rovelli and others have started questioning the elite status of time.

### Conjecture 2: Approximating the Future

While we cannot know for sure what the future will be like, we use all manner of models and theories to try and predict the future, using information available in the present. Hence, any expectation of future information is a function of present information, and this expectation is an approximation.

Hence,

![Image](https://cdn-images-1.medium.com/max/800/1*fHrOE9_5vgWV9ces_izoFQ.gif)

### Conjecture 3: Approximating the Past

Now, if we replace "future" with "past" in Conjecture 2, all the reasoning and conclusions still hold. You might ask, "But we know what the past is (unlike the future), so why do we need to approximate it?"

The fact is, we don't know anything exact about the past. Just like the future, we approximate based on memories, records, and other forms of media. These might appear to be more "accurate" than models of the future, but they are still approximate, and based on the present, not the past.

For example, an archaeologist might speculate about how ancient humans lived 30,000 years ago based on skeletal remains, but these speculations are approximations based on the present (a bunch of bones), and nothing else.

So, similarly,

![Image](https://cdn-images-1.medium.com/max/800/1*R09s0ZROWHeIadrcDG_e1g.gif)

### Conjecture 4: On the Exclusivity of the Present

Can we know any information about the past or future or any time that is not the present, which is not an approximation dependent on present information? What if we cannot?

If we cannot,

![Image](https://cdn-images-1.medium.com/max/800/1*qEABUSxmrLH2rZ6Dq0tpGg.gif)

### Conjecture 5: Time as a memory aide

Even if we accept that we can no no information, but that which is in the present, we all have a vert strong sense of time. For example, we care hopeful or anxious about the future, as we might be content or remorseful about the past. So even if time is imaginary, or a construction of our minds, it clearly feels real.

Why? What is the point of time?

Let's start with why our notion of time might be useful for survival, for if this were the case, it might exist because it has evolved as a survival advantage.

When we talk about "the past", what do we actually mean? To me, "the past" is a collection of facts, feelings and thoughts which are consistent with some past event.

For example, I accept that I was vaccinated for measles as a infant. This "acceptation" is based on several facts, including a small scar on my left arm, and another memory of an entry ("measles vaccination") in my immunisation record. There are also many details I have forgotten — like what the immunologist looked like, whether the immunologist had other staff assisting, and which one of my parents accompanied me.

The past event of "getting a measles vaccine" conveniently prioritises relevant details, and excludes all the rest. The most useful detail of this past is "Have I or have I not got a measles vaccine?" and thanks to the "past" I'm able to confidently answer this question. Correctly.

[Almost. Actually, not quite. The vaccination was actually not for measles, but for BCG — but until a few weeks ago, when I re-inspected my immunisation record, I was firmly convinced that it was measles. Even the rock solid past can be made fragile by information in the present]

### Conjecture 6: Past and Future are meaningless [Corollary of Conjecture 4]

"But it's not just about scars and records, is it" you say. "You really did get a vaccine in the past, didn't you?"

Maybe — but we'll never know. There is information in the present that might be framed as "evidence" for the past. But that's all we can say.

The same applies for the future.

### Conjecture 7: Time durations are meaningless [Corollary of Conjecture 6]

Given that past, future, and points of time that are not the present have no meaning, we can't talk about durations.

For example, if you leave Colombo at 6am, and reach Galle for breakfast at 8am, you might say that your journey had a duration of 2 hours. However, this concept of duration and the 2 hours is, like time, another aide to memory. The present might have "evidence" that is consistent with the duration of time, but, again, that is all we can say.

With durations loosing meaning, any concept of "persistent time" is also meaningless.

### References

[1] https://en.wikipedia.org/wiki/Cronus

[2] https://www.penguin.co.uk/books/301539/the-order-of-time/9780141984964

#### Article 42 · July 4, 2019

# I see a tree

![Image](https://cdn-images-1.medium.com/max/800/1*bEpOKeLcAOUdF5bw7YYoXA.jpeg)

>>> I see a tree

>>> I "see" a tree

>>> I see a "tree"

>>> "I see a tree"

>>> "I" see a tree

>>> I see a tree

Note: "X" implies that "X is real"

#### Article 43 · July 7, 2019

# On Radicals and Conservatives

### Some Political Aphorisms

![Image](https://cdn-images-1.medium.com/max/800/1*tBlEOSdiWi7eW8IHSaj3Fw.jpeg)

## On the Survival of Nations

* The world is an ecosystem. Nations are organisms. Their politics are their DNA.

* Nations that are fit to survive, survive. The nations that are nations today, are those that survived.

## On Conservatism

* Conservatives believe in the fitness of the current DNA. There is some justification to this belief. The current DNA has enabled survival. Thus far, at least.

## On Radicalism

* Radicals believe that the current DNA is diseased, and that a mutation is necessary to ensure future survival.

* Most mutations kill the organism. Some even kill the species.

* Some mutations, do, however, result in a better, fitter species. Likewise, sometimes a nation's survival depends on Radicals. Sometimes.

## On Ideas

* Conservatism and Radicalism have nothing to do with specific ideas, and are only relative to the status quo at a given time — the current DNA. For example, a liberal in a fascist nation is just as radical as a fascist in a liberal nation.

* Conservatives believe that conservatism is good, and each radical idea opposing it, evil. Radicals believe the current conservatisms to be evil. This sense of good and evil are relative and transient.

* Ideas change over time. Slavery was a conservative idea for most of history. Today, it would be radical.

## On Actions

* Conservative action (or more often inaction) results is slow or no change. Radical action results in unpredictable change.

* The problem with conservative action is that it won't change things much. The problem with radical action is that it will change things too much.

* "Interventions" (like invading a country) is usually conservative from the intervener's point-of-view, and radical from the intervenee's point-of-view.

## On Appearances

* Conservatives (sometimes) look like conservatives. Radicals rarely look like radicals. A western journalist in a comfortable office arguing for the invasion of another country is a radical. A poorly armed soldier, fighting for his life and that country is a conservative.

* Conservatives want to remain and appear conservative. Radicals want to become the conservatives of the future, and (one way or the other), their wishes are satisfied.

* Successful Radicals define the Conservatism of the future. Failed Radicals convert to the Conservatism of the present, or die trying not to.

## On Policy

* One could be a radical and conservative at the same time. US middle-east policy is conservative domestically (in the US), and radical for Iraq, or Afganistan.

* The same party could have both radical and conservative policies. Universal healthcare is a radical policy in the US, while high global defence spending is conservative. Democrats support both.

* The same policy can be both radical and conservative in different nations. Privatised health-care is radical in Norther Europe, but conservative in the US.

## On Effectiveness

* Political ideas that are effective survive. Political ideas that are good, are political ideas that are good.

* It is easy not to be wrong with conservative policies. And easy not to be right with radical ones.

* The most successful nations have been mostly conservative, with a few injections of radicalism from time to time.

* Nations that have never been radical, have never enjoyed extraordinarily success. Nor have they suffered from extraordinarily failure.

* Nations that have never been conservative don't exist.

#### Article 44 · July 10, 2019

# Cogito, ergo sum

### A Tale of Me, Myself and Mosquito

![Image](https://cdn-images-1.medium.com/max/800/1*27QlIJiEPpbhY6mFNVX_eQ.jpeg)

## From Concrete to Abstract

I smell. Blood. Then a high-frequency, buzzing sound. Like a saw. Then a light rustling feeling on the hairs on my arm. Then I see. At close range, I see her proboscis is erect like a spear, about to bore into my naked skin.

So far, the mosquito has meant many things to me. The complex, sickly metallic smell of blood. The complex nuances and harmonics of the buzzing sound of an insect. The complex and almost imperceptible perception of a small creature landing on ones skin. The complex sight of an organism that has evolved and dominated the earth for millions of years. Complex things. Concrete things.

But, suddenly, I think. Something completely different.

All concrete complexities are replaced by something abstract and simple: She is the enemy. I must kill her.

## From Cogito to Ergo

The smells, sounds, touches and sights are concrete things in the physical world. But the "enemy" is an abstraction of my mind.

She is the enemy because her like carry all manner of horrible diseases (Dengue comes to mind). And that sting. Few things are as painful (or so I think, in that split second). Justifying the label: Enemy.

Immediately, I begin to make plans. Plans for the future. I dream for a time when I will be just as I am, but this mosquito will be squashed dead by a sharp blow by the palm of my hand. I crave a future where I exist, and the mosquito does not.

The moment I make these plans, the future is born. And I will persist into this future. I have become a permanent being. Something real. I, now, am (ergo)!

## From Permanent to Impermenent

And then I realise the time.

Nearly 8pm. Dengue mosquitos don't bite humans at this time of night. The odds are that the mosquito, beyond the pain of her bite, is completely harmless.

As it happens, the said mosquito has been very greedy. She is completely engorged with blood (some other souls' — not mine). She gently topples on her own weight, and falls to the ground.

That future, where I exist and the mosquito does not, has not come to pass. Is this, then, a different future? One where I exist, but so does the mosquito?

It feels like that.

But them, now is not the future, is it? Now is the present. Where did the future go? Was it even real?

And if not, am I a permanent being? Or Am I?

References

https://en.wikipedia.org/wiki/Cogito,_ergo_sum

[1] https://en.wikipedia.org/wiki/Mosquito

#### Article 45 · July 10, 2019

# Spiegel im Spiegel

### On Mirrors, Reality, and Self

![Image](https://cdn-images-1.medium.com/max/800/1*W8sU_ZUEGddqCf5OoUByXg.jpeg)

### Prologue

In German, "Spiegel im Spiegel" means "mirror in the mirror" or "mirrors in the mirror" or "Infinity Mirror". You may recognize it as the title of the Estonian composer Arvo Part's famous tintinnabular (bell-like) composition for Piano and Violin [1][2].

This article is not about music; though it is about mirrors.

## On Mirrors

I'm walking along one of those long corridors one meets at hotels. On one side of the corridor are doors, lamps, pictures, and an array of ornaments. All along the other-side is a mirror.

I'm supposed to attend an event somewhere in the hotel. The receptionist has asked me to enter through the last door, at the end of the corridor. Not paying much attention to the paintings and the ornaments, I walk on. When I reach the end of the corridor, I turn, and reach out my hand to open the door.

Moments before I expect it, my knuckles hit a hard surface. It is painful, also slightly cold. I narrowly save my forehead from the same fate.

All along, I've mistaken the reflection of the doors, lamps, pictures, and ornaments, for the real thing. And the real thing, for the reflection. Perhaps, one ornament, or painting, looked real. And I decided to consider everything real.

A moment before I walk through the (real) door, I look over my shoulder at my own reflection.

## On the Mirror of Reality

In Every thing we think is wrong. And that's ok.[3] I said:

>>> The world we perceive is a model — constructed by our brains. For example, while we think we can "see in real time", that "realtime streaming video" is actually constructed from a set of still snapshots (about 10 per second), and then expertly stitched together by our brain — creating an illusion of continuity. All models are always incomplete, and often inaccurate — which is what I meant by "wrong".

>>> So, if all models are wrong, and our perception of the world is a model, everything we think and feel is wrong. But happily, as Box implied, some things we think are also useful.

Hence, our minds are mirrors that reflect a model of reality that is (hopefully) useful to us. When we perceive a belt as a snake [3], or a mosquito as "The Enemy" [4], we are seeing the world through a mirror.

And what about us? Do we not also see ourselves through this mirror that is our mind? Is there any other way of seeing ourselves?

Or have we somehow convinced ourselves that we are, for some reason, outside the mirror? On the real side?

What are the real consequences of us being on the imaginery side of the mirror? What real thing is the mirror reflecting? And what are the consequences of the mirror itself being on the imaginery side of the mirror?

What does this recursive gobbledegook even mean?

## The Mirror Crack'd from Side to Side

The mirror of thought is a mechanism for transforming concrete things into abstract and relative things. This process of transforming has no innate meaning of its own, except that it has helped humans (and possibly other intelligent organisms) survive.

It is difficult to see beyond, and see through the mirror, or even see the mirror itself, if the only means of seeing involves the mirror as a source of reflection. The only way is to stop looking (so thoroughly and keenly) at the mirror, and seeking other modes of sight.

But what other means of sight?

### References

[1] https://en.wikipedia.org/wiki/Spiegel_im_Spiegel

[2] https://www.youtube.com/watch?v=hV4LlCtvgwE

[3] https://medium.com/@nuwan.senaratna/every-thing-we-think-is-wrong-and-thats-ok-d467a38d841b

[4] https://medium.com/@nuwan.senaratna/cogito-ergo-sum-8d8b03f9c3b4

#### Article 46 · July 16, 2019

# On Observation

### From Objective to Subjective

![Image](https://cdn-images-1.medium.com/max/800/1*Ixuj8dz-1IBv9V1mqTdodg.jpeg)

### Water and Rocks

Yosemite Valley [1] can be visited all year around. It is black and white, and infinite in winter; golden and mysterious in autumn; hot and smoky in summer. But I like it best in spring, when the rivers and waterfalls swell, when the trees and the grasses are at their greenest, and the sky at its bluest.

On one such spring visit, I was sitting by a river, watching water endlessly stream from under a bridge. I plunged my hand into the icy flow, and picked up a rock. I ran my fingers through its smoothness and shape; one only created by thousands (perhaps millions) of years of flowing water, the sound of which I could still hear.

What made the water the water, and the rock the rock?

The water was liquid; molecules moving about in formation; it was cold, which meant that its molecules moved slower than (say) had they been part of a hot bath. The flowing water had a rumbling, rustling sound, as its flow moved against the bed and banks of the river, disturbing the air around it, causing sound.

The rock, on the other hand was hard; molecules packed in solid formation. They also moved, but more slowly. It absorbed most light particles, except for the few reflected that gave it its unique glossy, grey colour. Not disturbing the air around it, the rock was as silent as a tomb.

### From a Changing Universe to Constant Forms

Hence, in my meditations by the river, I experienced many forms of matter: sights (the glossy, grey colour of the rock), sounds (the flowing water), and feelings (the smooth, hardness of the rock, and the icy coldness of the water). All these felt constant. The rock, for example, had, perhaps, held its colour and hardness for centuries. The water would have remained cold, at least, until the afternoon sun heated it up.

But these forms that appeared constant had an underlying reality that was constantly changing. For example, the rock was solid because its molecules vibrated in formation; it was cold because they moved slowly; and it was grey because it absorbed and reflected photons in a certain way.

At a single point or moment of time, these forms would have no meaning, because at a point in time, my senses would not know if a molecule was moving, or if light particles were reflected, or if the atmosphere was disturbed resulting in sound. All these forms were meaningless without observations or measurements that persisted in time.

Hence, my senses that sensed these forms, both recorded and simplified the world for me. They miraculously transformed a stream of changing information, into a constant colour, sound, hardness, or temperature that persisted in time and memory. These simplifications helped me make sense of and realize and comprehend a possibly incomprehensibly complex reality.

But there was a problem.

Was I actually observing reality? Or was I simply observing what I was observing? Was there something (anything?) objective underneath it all? Or was it an imagination? A mirror within a mirror?

### An Objective Universe to a Subjective Observer

I continued my thought experiment.

What were my senses actually doing? For example, did my senses 1) observe the universe all the time, in a continuous stream of observation? Or 2) did my senses observe the universe as a series of discrete snapshots?

Continuous observation must also imply that there was some notion of absolute time, and that the nature of form was relative to this absolute time. For example, "how fast a molecule vibrates" and as a result, whether something is hard, or soft, or hot, or cold, would be a function of this absolute time.

On the other hand, if the observations were a series of discrete snapshots, then the nature of form was also a function of this discrete set of observations. If the snapshots were frequent, a molecule would (appear to) vibrate more slowly, and would appear to be colder and harder. Slow-down the snapshots, and reality would have become softer and warmer.

The second hypothesis had even more startling consequences.

Suppose the universe was random and void of any meaning, like a sequence of random numbers. Just as the sequence could be sampled in such a way to imbibe meaning (e.g. I could sample the numbers 2, 7, 1, 8, 2, 8,...), a certain sequence of snapshots could imbibe a meaningless universe with a definite and apparently meaningful form. Furthermore, two different observers, with different sequences of snapshots could perceive the world in completely different ways.

Another observer could have been sitting where I was, and not see the beautiful Yosemite Valley, but Trafalgar Square, or the surface of Mars, or even something amazing or horrible I could not imagine.

### The Question of Observation

I decided, for arguments sake, to accept my discrete snapshots hypothesis. Several questions followed:

* Why do the snapshots occur the way they do? Can their nature be changed?

* Why do my senses simplify reality the way they do? For example, why is slow vibration interpreted as hard or cold, and not "red"?

* Was the simplification an attempt to simplify, or confound? That the changing was constant?

* Do the forms I see (colour, sound, hardness) have any absolute meaning or reality of their own?

* Is the universe real?

"Interesting questions..." I thought to myself. Yosemite continued in front of my eyes, ears and senses, beautiful as ever, with its water, and ancient rocks. Perhaps I'll answer them on another visit, I thought.

And I went back to marveling.

—

[1] https://en.wikipedia.org/wiki/Yosemite_Valley

#### Article 47 · July 17, 2019

# AI by the Backdoor

### Some contrarian thoughts on how to succeed at AI

![Image](https://cdn-images-1.medium.com/max/800/1*2bJXqLem7kPqzCD0fEPQMg.jpeg)

Many people ask me "How do I learn AI?" or "How can my company use AI?" The latter question most often comes from young undergraduates preparing to study computer science; the former, usually from company executives who have heard about AI, but have no practical knowledge of how it works or what to do with it. Variations of these questions often refer to "experts": "How can I be an AI expert?" or "How can we (our company) become a leader in AI expertise?"

This article attempts to answer these questions, or at least satisfy the motivations behind them. Personally, I don't consider myself an "AI expert" (in all but the most self-deluding senses of the phrase). However, I have studied AI at a graduate level, and have worked on some meaningful AI problems. I have also met, worked and learnt from several people who can claim to be AI experts of world renown. These experiences have influenced this article.

## The AI Expert

What does an AI Expert look like?

### An AI Expert is a Scientist and an Artist

Most AI theory can be understood with undergraduate level Linear Algebra, Calculus and Statistics. With some practice, most cutting edge AI research publications can be read and understood with this knowledge. If you don't believe me, try some AI courses online (e.g. https://www.deeplearning.ai) and read some papers yourself (e.g. https://papers.nips.cc).

All AI experts have had a solid background in these fundamentals (often) from a young age, and acquired a seamless sense of how to apply these in a scientific way. This is what I mean by "scientist".

However, this knowledge alone is not sufficient to succeed at AI. Practical AI involves significant intuition and (sometimes) guesswork. The most skilled AI experts "seem to know" what to do without being able to explain how or why, the same way an artist paints a canvas or a poet writes a poem. This is what I mean by "artist". Just as in the hands of the best poets "the poem writes the poem", in the hands of the best AI experts "the model designs the model" or "the AI writes the AI".

### An AI Expert has access to resources

Almost all world-renown AI Experts are affiliated to top companies (e.g. Google, Facebook, Microsoft) or top universities (e.g. MIT, Stanford, Tsinghua) with access to huge monetary resources. This is because cutting edge AI requires training huge models, on huge amounts of data, on huge hardware infrastructures.

In addition to hardware resources, AI problems also involve significant human participation. For example, a company like Google employs 1000s of engineers and data scientist to work on their AI systems. This too involves huge monetary investments, and the AI experts that head these projects control how these resources are used.

### An AI Expert has access to meaningful data

Most importantly, AI needs data. By "meaningful" data I mean data that can be used to solve meaningful problems. If you don't have good problems to solve, there is no reason to bother trying, even if you have data. Conversely, you might have interesting problems, but without data, you can't use AI.

## The Backdoor Approach

If you want to be an AI expert, you might try and acquire these characteristics: Study AI at a top university, and then join an institution with resources and interesting problems.

However, the odds of becoming an internationally (or even nationally) renown AI expert are slim. And anyway, this article is not about "how to succeed at being an AI expert". Instead, this article is about "how to succeed at AI".

The "backdoor" approach involves following the "what an AI expert looks like" ideas in reverse.

### Step 1: Find a problem you care about

Always start with a problem. What problems do you care about? Solving what problems would result in profit or gain to you? If you can't find a problem you care about, find a problem which other people (say your boss, or other people in your town, region, or country, or company) care about.

Then, see if this problem can be solved using data. You don't have to solve the problem 100%. See if you can solve it 10%. Often, a 10% solution, might yield 90% of the gains. Also, you don't need to apply the most complex AI technique to solve the problem. See if a simple solution can solve the problem. What's the point in using Deep Learning, if a simple rule engine can give you a good enough solution?

### Step 2: Create your own resources

Even partially solving the problem (say a 10% solution), gives you a couple of new advantages: You can use the partial solution to convince other people that you might be able to attempt a complete solution, and give you the resources you need. You can also use the profits from the partial solution to invest in resources (say people or hardware) that can be used for a better solution.

### Step 3 (Optional): Become a scientist and/or an artist

The best way to become a writer, is to write as much as you can. Similarly, the best way to become an "AI Artist" is to work on as many interesting AI problems. Hence, finding good AI problems is the best start to this journey.

The same applies to being a "AI Scientist". You can always go to university and get a Masters or a PhD in AI, or more easily complete a course in AI (in a few weeks or less) online. But if you have interesting problems to work on, you have a lot more motivation to learn new techniques. You're also less likely to forget what you learn.

## Concluding thought

If you should take away one thing from this article, it is that "You should not see AI as a general qualification or privilege. You should see it as a specific tool or servant to solve your problems". The most important thing is to learn to get that tool or servant to work for you. If you can do that, you can instantly start reaping meaningful benefits.

If not, "AI" will be to you, as it is for most people, a meaningless buzzword.

#### Article 48 · August 1, 2019

# On Education

### Why education is what it is, and what it will be

"The Classroom of the Future" and education in general is a hot topic these days. The likes of Sir Ken Robinson wax eloquent on all that is broken about our current education and all that it must be fixed in the future. Growing income inequality, the threat of Artificial Intelligence, and rising education costs and debt have further fuelled this discussion.

I want to consider different questions in this article. Not "What education should be" but "Why education is what it is" and "What education will be".

## Meanwhile in Sri Lanka...

Recently, a group of unemployed university graduates were protesting, demanding that the government provide them with jobs. This state of affairs is not surprising when you consider the following:

* The majority of schools in Sri Lanka don't support advanced level classes in the physical and biological science streams. Hence, most of the students graduating from school follow the arts stream. In an effort not to discriminate these students, the government has pushed universities to align their input with this output from schools. Hence, most students admitted to universities study, and then graduate in arts subjects. These numbers are wildly out of sync with employment demand. There are far too many arts grads with far few jobs, and vice versa for medicine, and STEM jobs.

* There is almost a religious respect for education in Sri Lanka. Hence, any education is better than no education. With the exception of a few discerning parents, many spend vast amounts of money to educate their children at third-rate universities abroad. Many take loans or sell the ancestral estate to pay these bills. For those who are not fortunate enough to receive a university education, there are all manner of two, three, and four-letter qualifications and diplomas available for a fee. For peddlers of such qualifications (especially from the U.K.), Sri Lanka is a favourite destination. Bottom line — many Sri Lankans get some education, without paying any attention to its relevance (or more accurately, its irrelevance).

* Sri Lanka has a highly incompetent mob of politicians, who, in addition to lining their pockets, care only about one thing: getting re-elected, every 4, 5 or 6 years. While they are mostly incapable of delivering development or a better standard of living, there is one thing they can reasonably guarantee: A job in the bloated state sector.

Hence, there are two types of graduates in Sri Lanka:

* Graduates in fields with too many jobs, but too few graduates

* Graduates in fields with too many graduates with too few jobs, who have a implicit employment contract with the state (i.e. "I know I have a crap degree, but you know you have to give me a job")

## Why Education

![Image](https://cdn-images-1.medium.com/max/800/1*j7-nh-Um2HpJtK0OEfYn7w.png)

But what is the point of education? In its broadest sense, education provides (us humans) a set of tools to satisfy (our human) needs, in the broadest sense.

However, as I implied, this is a very broad definition. In general, even the most respected education institutions (e.g. the worlds top universities), mostly focus on a subset of these tools and needs — namely, the bottom "Professional Skills".

"Professional Skills" are the basic skills that define a professions; for example, what enables a doctor to prescribe medication, or a surgeon to perform surgery, or a journalist to write a news article, or a computer scientist to design a computer system. 99% of most university curriculums will focus on these skills. At a needs level, these will guarantee one a job — and hence a salary, enabling physiological and safety needs to be satisfied.

However, beyond doing what you are expected to do and getting paid for it, humans need and crave other skills. Even in the professional workplace, humans need social, behavioural, and cultural skills to effectively collaborate with peers and customers. This is why many top MBA programs are also beginning to offer golfing, sailing and social dancing courses.

Finally, there is there are internal psychological needs, around self-actualization and transcendence. For example, does an employee have the mindset to work hard and grow? Or the ability to self-criticize and reflect? In my professional career as a computer scientist, software engineer and engineering manager, there were many times where philosophy (of Marcus Aurelius, to Socrates, to Lao Tse, to the Buddha) was invaluable, but in nearly 25 years of formal education (in some very good educational institutions), it was never required for me to take a course in any type of philosophy.

Hence, education is broad and important. But sadly, our perception of education, and that of educational instituitions, and the state, is very narrow.

## What education is

It is not surprising that formal education focusses on the bottom of the needs hierarchy. It is simply a matter of prioritization. Educational institutions and states focus the most benefit, at the least cost. Hence, formal education focusses on professional skills.

Even within professional skills, institutions tend to focus on the lower mechanistic skills, which can be imparted at the lowest cost to the most number of students. These include information and processes that can be rote learned, and tested in a standardised (and inexpensive) way. Hence, professional skills that focus on creativity and critical thinking (as opposed to mechanical non-thinking) receieve less attention. For example, through an undergraduate and graduate education in computer science, I never had to build a meaningful computer system that got used by actual people. For this type of education, I had to rely on side-projects, and finally employement itself.

Hence, just as I educated myself on some of the more creative aspects of computer science, the higher means of education do exist. It's just that they don't really happen in traditional educational institutions. Parties, events and other social gatherings are far more educational at social, behavioural, or cultural level than universities, as is reflection and meditation at a mindset and philosophical level.

Traditionally, education has been seen as a social and economic leveller, and the traditional educational institutions (school and university) — the engines that performed this transformation. This worked well in the 19th and much of the 20th century when most of the even most "professional" professions were mechanised and depended on little creativity. For example, the British educational system (an ancestor of Sri Lanka's current system), was designed to produce an army of civil servants from Canada, to Ceylon, to New Zealand, who all performed the same mechanised tasks, in exactly the same way. That world is dead, but we are left with the same education system.

## What education will be

The likes of Sir Ken have grand visions for education in the future: some of them involve significant interventions, most of them top-down, involving huge investments. I prefer to think bottom-up — try and analyse the situation from that stand point, and build my conclusions based on that.

Here are some predictions about the future, based on this bottom-up reasoning:

* Educational institutions (in their current form) will disappear. With advances in technology and artificial intelligence, all the remaining forms of mechanised employment will disappear, and with it the relevance of mechanised education. Education will have to focus on higher level professional skills (like creativity) and providing tools for higher level human needs.

* The void left by these institutions will be largely filled by parents and students. High income individuals will have a huge advantage, as education focussing on higher level needs will require significantly more time and money. Many accuse current educational institutions of being too expensive; those of the future (if any) will be orders of magnitude more expensive.

* Inequalities will increase in wealth, power and dignity. The "education is a leveller" contract between state and citizen will breakdown. Protests (e.g. that of the unemployed arts graduates) will increase; vialble solutions will decrease. This transformation will also happen in fields which currently don't face employment shortages like computer science. In the (possibly near) future, computer science graduates will be the ones protesting for jobs.

These might sound gloomy and pessimistic. Then again, it is what it is. And hopefully, we make the best of the situation.

Acceptance is the first step.

#### Article 49 · August 1, 2019

# On Questions

### Questions startups should be asking

![Image](https://cdn-images-1.medium.com/max/800/1*iZ3DDarqy9lcetxr9SrEtQ.png)

## The most important question

Most startups fail; a few have a small chance of succeeding. But most fail.

For the few that might succeed, most paths to the future will end in failure; less than a handful will result in success.

Hence, there is one question all startups should always be asking: Are we on a path to success? Or simply,

>>> "Are we going to succeed?"

This question can, equivalently, be framed probabilistically,

>>> "What are our chances of succeeding?"

And negatively:

>>> "Are we going to fail?"

Personally, I like the negative-probabilistic framing:

>>> "What are our chances of failing?"

## The next most important questions

"What are our chances of failing?" is, while important, abstract, bordering on philosophical.

Our next task is to break it down into sub-questions which will help put a "number" (however, approximate or qualitative) on the probability. Hence, the next questions are:

>>> "What does failing actually mean?"

>>> "What are all the ways in which we can fail?"

>>> "What are the chances of this type of failure happening?"

>>> "What can we do to prevent that sort of failure?"

For example, "failing" means running out of money. One way we can fail is "We don't get X customers by date Y". We won't hit this goal if we don't do A, B, and C. Hence, we should do A, B and C. (Repeated for all the other ways of failing).

## Nothing else matters

The next most important question is:

>>> "What are the things we are doing that have nothing to do with the most important question?"

If there are things that seem to be disconnected from the most important question, they are actually connected. Anything else, is a distraction. And hence, will contribute to failure.

Hence, stop doing everything that doesn't matter.

#### Article 50 · August 3, 2019

# Fundamental Fundamentalist Buddhism

### The Fundamental Fundamentals

![Image](https://cdn-images-1.medium.com/max/800/1*jpmwIBxlEnzRABH0gXhS2A.jpeg)

## Fundamentalists and Fundamentalism

The rise of agitating monks (like the BBS in Sri Lanka) and attacks against other religious communities (like the Rohingya in Myanmar), has tarnished the peaceful image of Buddhism. When I talk about Fundamentalist you might think that I'm referring to these agitating factions that get up to all manner of naughtiness in the name of Buddhism.

Actually, I wanted to write about something else: A very different intepretation of Fundamentalist and Fundamentalism. I wanted to identify the most fundamental fundamental teachings of Buddhism; which themselves would imply what a fundamental adherent of those teachings would look like — or what, a fundamental fundamentalist Buddhist would look like.

## Standing on one foot

Hillel HaGadol, a Jewish religious leader and Rabbi of the 1st century BCE, was once asked to explain the whole Torah while standing on one foot. To this he replied:

>>> "What is hateful to you, do not do to your fellow: this is the whole Torah; the rest is the explanation; go and learn" [Wikipedia]

Hence, Hillel described the core of the Torah as "What is hateful to you, do not do to your fellow" (also known as the Golden Rule).

What would a standing on one foot core explanation of Buddhism sound like?

## The Essense of Buddhism

To me the essence of Buddhism would be, Anicca, or that everything is impermanent. It is the essence because everything else of importance derives from this essential concept.

The word anicca is often heard with two others: dukkha and anatta.

Dukkha is the unsatisfactoriness felt at the impermanence of things. Sometimes we want things to persist (e.g. a healthy life), but they don't (e.g. we fall ill). At other times we want things not to persist (e.g. a painful illness), but they do (e.g. we continue to suffer from the painful illness). Both are unsatisfactory.

As we want the good times to last for ever, and the bad times to never happen, we also believe in a permanent self (or me). This is not a mere intelectual belief, proved or disproved by reasoning, but a very deep misconception that influences everything we see, feel, and think, and reason itself. Anatta means non-self, or that that there is no permanent self.

Many books explain Anicca, Dukkha, and Anatta in far greater detail and precision. In this article, I only wanted to make one point: That Dukkha, and Anatta are derived from Anicca. The same can be said for everything else of importance.

Hence, a Buddhist Rabbi Hillel could have stood, not on one foot, but on one toe, and said,

>>> "Anicca".

## Pretend Fundamentalists

Much doings in the name of Buddhism (and throughout history), contradict annica. For example,

* Buddhism couples with worldly ideologies. For example, the likes of the BBS and other nationalist groups, couple worldly Sinhala Nationalism with un-wordly Buddhism. They (not inaccurately) tie the survival of Buddhism in Sri Lanka with Sinhala rule and civilization. While it is true that without this rule and civilization (which was at times violent and militaristic) Buddhism might not have survived in Sri Lanka, it is also true that the ideas of violence and militarism contradict fundamental Buddhist tenants. For example, it is impossible to go to war (where you will need to kill the enemy) without breaking the first precept. More fundamentally, the belief in, or the need for, an eternal Sinhala race, contradicts the core of Buddhism: namely anicca.

* Buddhism has also become a huge personality cult. People who know nothing about the core of Buddhism often pray to the Buddha, asking for material gifts, and prosperity. This contradicts anatta (which is derived from anicca). Just as there is no me, there is no Buddha ("The Buddha exists for those who don't know Buddhism; and does not exists for those who do", a famous Zen saying goes). Around the primary personality of the Buddha, there are secondary satellites (usually, Buddhist monks). While monks in rural Sri Lanka often suffer great poverty, it is common for monks in the wealthy parts of Colombo to surround themselves with worshipers who shower them with expensive gifts like cars, land, and grand celebrations, wallowing in their overblown personalities.

* Buddhism has become a religion. By religion I mean "a social-cultural system of designated behaviors and practices, morals, worldviews, texts, sanctified places, prophecies, ethics, or organizations, that relates humanity to supernatural, transcendental, or spiritual elements" [Wikipedia]. Like all religions, the members of that religion act in such a way to ensure the persistence of these aspects: from practices, to texts, to organizations. This contradicts anicca, which implies that all there ideas are impermenent, and that willing them to be permanent will lead to unsatisfactoriness (dukkha). More to the point, the fundamental nature of Buddhism makes it not a religion, and more a set of philosophical statements about the cosmos (like anicca, and its derivations). Hence, the more Buddhism becomes a religion, the less it becomes Buddhism.

Such is the state of Buddhism today: a religion dominated by pretend fundamentalists.

## What next

If you consider yourself a Buddhist, are you a pretend-fundamentalist, a fundamental fundamentalist, or neither, or none of the above?

Either way, I'm not asking you to accept anything I say as gospel. That would itself be a violation of anicca (Note, this is true, even if what I say is true. Why? That's a whole new article — perhaps several).

Instead, perhaps, you could also think about fundamental fundamentals. What might they be? Would they be of any use to you? What is it that really matters? What is it that is really true?