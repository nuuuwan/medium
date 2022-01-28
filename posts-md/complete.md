#### 1

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

#### 2

# Fragile Employees vs Fragile Companies

In August 2015, the New York Times, published "Inside Amazon: Wrestling Big Ideas in a Bruising Workplace.". The following excerpt reasonably summarizes the whole:

![Image](https://cdn-images-1.medium.com/max/800/1*XN7Xh3ey3zbnOTPS-crK-Q.png)

The piece was seen by many as been a "dystopian expose". Jeff Bezos sent a memo to Amazon employees, including (among other things) the following rebuttals.

### Antifragilty by Layers

![Image](https://cdn-images-1.medium.com/max/800/1*qpa9HjxQ3qJ9WhqjUEXpkA.png)

I have not worked at Amazon, and while I have heard many anecdotes from friends and colleagues on the pros and cons of Amazon Culture, I don't feel qualified to judge if the "little-known experiment in how far it can push white-collar workers" has succeeded or failed. However, it did remind me of this quote from Antifragile: Things That Gain From Disorder by Nasim Nicholas Taleb:

In the book, Taleb introduces antifragility as follows:

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

#### 3

# Markets, Managers and Beyond

In 2016, a UK employment tribunal ruled that Uber drivers should be classified as workers with minimum-wage rights. Uber appealed this ruling, which they subsequently lost in November 2017. What I found interesting about this episode, was less the legal battle, and more one particular implication of classifying Uber drivers as Uber Employees.

![Image](https://cdn-images-1.medium.com/max/800/1*K2J2EY_7344Mt1h1qNzceA.png)

Until now, all employees at Uber (except, possibly the CEO), have a designated human manager. Uber drivers, on the other hand, are completely "managed" by the market forces, and the systems that try to predict and simulate them. It is supply and demand for rides, rather than some human agency, that determines what management they get. Hence, the ruling implies that Uber (at least theoretically in the UK) now has two types of employees: 1) those managed by humans, and 2) those managed by the market.

![Image](https://cdn-images-1.medium.com/max/800/1*8nP3WXaBPS0kx0f3wr040w.png)

This led me to ask:

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

Page and Brin, decide to tackle Problem 1 first (say, because it's easier, or more "impactful"), store Problem 2 in the database for future retrieval, and start working on Problem 1.

![Image](https://cdn-images-1.medium.com/max/800/1*4sPXC7keoARcB_6XkWyM0A.png)

Let's take a closer look at this magical "system" which is connecting problems with Page and Brin. What functionalities must it have?

### QUESTION 1: Can all workers be "managed by the market" via some automated system?

The answer to this question depends on whether some automated system can satisfactorily possess the above qualities. I'm going to avoid directly answering this question just now, because I'm less interested in whether some magical AI system can satisfy these qualities, and more interested in what us humans might learn from this thought experiment.

The first and most obvious learning is that human managers should also possess all these functionalities. To rephrase each quality as "human" functions:

To me, these four qualities seem core manager functions.

My second learning is that these qualities are not uniquely manager tasks. For example, all employees should be expected to understand the mission of the company, and how it relates to the specific problems they are individually solving. They should also be expected to have self-awareness (i.e. understand themselves), and manage their own performance to various degrees. Employees often also participate in the understanding and evaluation of their peers.

My third learning is that the process of executing these qualities also leads to generating meta-problems. For example, just as achieving a company's mission is one problem, making sure the company has the right employees to achieve that mission is "emergent" meta-problem. Some of the most interesting "manager problems" are such meta-problems.

My fourth learning is that even if we had a magical system that juggles problems and people, whenever there is a market, people find interesting and complex ways to interact with that market. One such "complex behaviour" is how people collaborate. For example, several engineers might decide to collaboratively work on the problem. Their interaction might be ad-hoc and organic. Maximizing positive ad-hoc and organic behavior is, in turn, an interesting "meta-problem", and one that many organization give a lot of attention.

But back to Can all workers be "managed by the market" ?

Assigning passengers to drivers is a lot simpler that assigning problems to engineers, particularly given the complex way humans behave. My guess is that it would be easier to build an artificial system that write codes, as opposed to one that manages humans that do. Rather than spend more time on this question, let's move on to the next one.

### QUESTION 2: What is this value addition of managers?

Before, answering this question, what or who exactly is a "manager"?

Here are a couple of candidate definitions:

There is some degree of "trueness" to all these definitions.

However, individually, each definition is problematic.

Hence, I don't have an answer to QUESTION 2, because without defining what a manager is, it can't be satisfactorily answered. Instead, let me cheat and try to dance around the question.

### Beyond Managers?

In Automate/Informate: The Two Faces of New Technology, Shoshana Zuboff describes the effect of new technology on the historical role of the manager as follows:

...

Hence, traditional "middle-management" relied on managers holding a monopoly over information, which enabled them to direct workers. This role was undermined as information became more broadly accessible.

Many companies have already moved away from managers who are information gatekeepers and controllers, to one in which they mostly provide the core manager functions that I describe above. But as I explained earlier, the problem with this new job description is that it is not unique to managers.

Is it time to move beyond the role of the "manager"? At least in tech companies where information is freely available and sharable, this seems feasible. Should companies be organized purely based off what subset of problems people are working on, and what volume of problems each individual is responsible for? In such a model, each there would still be levels of seniority, and even hierarchies of employees, based on who is responsible for what "people meta-problems" but no separation of managers and non-managers.

![Image](https://cdn-images-1.medium.com/max/800/1*zl5vT4nm0v25lEF7eIp74w.png)

#### 4

# Classification Algorithms, Elections and Electoral Metaphors

### Including "What is democracy analogous to in the Machine Learning discourse?"

![Image](https://cdn-images-1.medium.com/max/800/1*oZEcwIj9LoNj-64W-satnQ.png)

A classification algorithm assigns some observation to some class of things. For example, given an email (the "observation") a spam detection algorithm could determined if it should be classified as spam or not-spam (the two "classes"). The algorithm will use various attributes of the email (e.g. who sent it, the text in it, what time it was sent etc) to determine which class it belongs to. These "attributes" are known as "features".

In elections, people vote to choose an individual to hold political office. The Electoral System determines how the aggregate votes are used to determine the winner. For example, the recent UK parliamentary election uses a "First-past-the-post" system, while Sri Lankan parliamentary elections use proportional representation.

Elections are analogous to Classification Algorithms. The observation is a single election. The features are the people voting. And the class selected by the algorithm, is the winner of the election.

Here is a list of some well know Classification Algorithms and Concepts, as "Electoral Metaphors". For readers familiar with Basic Machine Learning, I'll leave it as an amusing exercise for you to guess what these might be. If you're not, you could reflect on how Electoral systems have many things in common with Machine Learning algorithms — even when these commonalities might not be desirable.

#### 5

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

#### 6

# Every thing we think is wrong. And that's ok.

![Image](https://cdn-images-1.medium.com/max/800/1*Kr1tTsOfpKQPaSS5r8GzCg.png)

The world we perceive is a model — constructed by our brains. For example, while we think we can "see in real time", that "realtime streaming video" is actually constructed from a set of still snapshots (about 10 per second), and then expertly stitched together by our brain — creating an illusion of continuity. All models are always incomplete, and often inaccurate — which is what I meant by "wrong".

So, if all models are wrong, and our perception of the world is a model, everything we think and feel is wrong. But happily, as Box implied, some things we think are also useful.

Let's now pause for a cup of tea.

### Little Tea Leaves

If you, like me, drink a lot of tea, and you, like me, brew tea directly from leaves, instead of tea-bags (what I call "from first principles"), you'll find that you need to strain the tea. While the bulk of the leaves lodge in the strainer, a few little leaves will escape through its holes. None of the little tea-leaves "designed" to "survive" the strainer. Randomness happened to make them small — and as a result they "survived" the strainer.

We are all tiny tea leaves. We happen to be descended from lucky few who survived the trials of evolution, because we happened to posses the bodies and brains, which, by chance, adapted to survival. Our brains don't create "correct" or "accurate" models of the world, merely ones optimized for survival. Sometimes these models are wrong, but it's still ok.

For example, consider the snake.

### Snake

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

#### 7

### Aphorisms

# On Small Plans and Big Plans

![Image](https://cdn-images-1.medium.com/max/800/1*47eKyJD3avxlyboMieKA_w.png)

### Costs, Benefits and Success

### Action

### Fatality

### Missions and Strategies

### Organizations

#### 8

# Japan Reflections

![Image](https://cdn-images-1.medium.com/max/800/1*sesSZhYyxuVh8caVdHFPNQ.jpeg)

A couple of weeks ago, Kanchana and I visited Japan for the first time. To say "we had a good time" is an understatement. Japan was "Food heaven, Jazz heaven, and (especially relevant to me) Train heaven — all rolled into one".

But beyond this material appreciation, the trip also awakened some spiritual curiosity. I was particularly interested in the following observations.

Much of this seemed connected and embodied in Japanese Zen Buddhism. I was particularly interested in the concept of Wabi Sabi (侘寂) — which I learnt about after the trip from Marcel Theroux's BBC documentary, and this useful blurb by Alain du Botton. Roughly, Wabi and Sabi are being at peace and appreciating Suffering and Impermanence, respectively.

At the back of my mind, I always felt that there was some common thread linking all these ideas. To say the common thread was "Buddhism" felt partly true, but also felt incomplete. I wanted something more specific.

A couple of days ago, it occurred to me that the following explanation is consistent with the observations:

Non-Individualism, Formalism, Minimalism, Quality and Wabi Sabi are all connected to living through contemplation, as opposed to living through thought.

As I thought about this more, the following contrasts occurred to me.

## The Contemplative Life vs. the Thoughtful Life

## Disclaimers

#### 9

# Deep Consumption

There is so much information out there — both online (blogs, videos, articles, e-books, music) and offline (books, discussions, concerts). On the other hand, time is increasingly limited. So much information — so little time. How does one decide what to consume and what not to?

I have thought a bit about this question: Sometimes proactively (usually, to find ways in which I might spend my time more wisely); at other times reactively (often, after I have felt that I've "wasted time" watching, reading, or listening).

This note is a set of "guidelines to self" about what information to consume, and what not to. I am sharing with you either because I would like your feedback about it, or because I feel it might be useful to you.

Before I start, a couple of disclaimers. I propose some "models" on how our brain processes information. I am not a neuroscientist and many of these models are not scientifically conceived. They are mostly metaphors to aid understanding. Also, a lot of these ideas are not completely original. I have been influenced by conversations with friends, and books (most importantly, The Shallows, by Nicholas Carr).

## Goals

Let us start with the "why". Before arguing about "what" information to consume, we need to clarify "why" we consume information.

For me, I feel I consume information for the following reasons:

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

## Credo

If the goal of information consumption is knowledge, creativity, and stimulation, then I believe that deep consumption is clearly preferable to shallow consumption. The "guidelines" I am going to propose hinge on accepting this belief.

## Guidelines to Self

All that was "theory". What does this all mean in practice? I have distilled these thoughts into the following guidelines:

![Image](https://cdn-images-1.medium.com/max/800/1*OXZjezwMY_xkP4VmgwWClA.jpeg)

#### 10

# Who do you side with?

## But not simpler

This week's Economist has an excellent article on how European political issues and topics are tangled and complicated. It gives some good examples of where the simplistic "right-left" classification and other binary over simplifications breakdown:

## Meanwhile in California...

Earlier today, among the elegant citizenry promenading Palo Alto's University Avenue, was a scruffy looking woman, pushing a shopping cart, piled with various grey tinged clothes, papers and baggage, with a big "I love Trump" sign taped to the said cart.

In the same block was a retired educator collecting donations for some drug rehabilitation related charity. In return for a small contribution, he presented me with a bunch of "thank-you" marketing material, including a comical list of poems praising the virtues of a certain Bernie Sanders, and poking fun at the said much-loved Donald Trump. He somewhat bizarrely, prefaced this presentation with a "Do you hate Trump?" question (apparently expecting nothing but full agreement).

Whatever the Economist might pontificate, simplistic "right-left" classifications seemed alive and well, at least in Stanford-educated Palo Alto. One might tolerate some bias among "ordinary people". However, when I looked at the latest Facebook posts of the Representative in Congress for Palo Alto [2], the two senators for California [3] [4], and the President [5], I noticed exactly the same phenomenon.

While there were no funny poems, or declarations of undying love, almost all posts I read had three things in common: 1) they attack the opposing political party; 2) issues are described as black vs. white, non-negotiable issues; and 3) "blame" is posited, not on individuals but on the opposing party as a whole ("Republicans", "Democrats"), or one of the synonyms for the said groups ("Conservatives", "Liberals", "Right", "Left" etc.).

## Who do I side with?

I've been annoyed, irritated and worried by this over simplification for some time. Related, I wrote this note, Frustrations and Fears [6] soon after the 2016 presidential election. It seems impossible to have a reasonable conversation about politics without siding or being sided into one of the two sides. I found this particularly frustrating because, as I wrote in the said note:

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

#### 11

# Black or White?

## Donkeys or Elephants?

![Image](https://cdn-images-1.medium.com/max/800/0*iqpoGybMJS49dfFt)

In the lead-up to the 11/6 Midterm Elections in the US [1], I shared some thoughts on "binary politics" and more the one-sided, partisan nature of political discussions [2] — Either you support the Democratic Party (Donkeys) or you support the Republicans (Elephants), with no middle ground, or room for debate.

Meanwhile in Sri Lanka, we have been witnessing an interesting constitutional drama (also known as #CoupLK and a the "Constitutional Crisis"). The timeline is roughly as follows:

I'm no expert to share my own opinions on the constitution, but I did make the following observations about the political discussion surrounding the drama on Facebook, Twitter and news media.

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

Now, the laws of binary logic state that both "P" and "Not P" cannot be true at the same time. In other words, my eyes cannot be black and not black at the same time. Also, the laws also state that at least one of the two have to be true: That is, either my eyes are black, or they are not black.

What if we break these laws? Then, the following could also be true:

Note, we have moved from binary (2-state) logic, to 4-state logic.

## Two types of Ignorance

But what does "My eyes are black, and my eyes are not black" and "My eyes are not black, nor are my eyes not black" mean?

Consider the following types of ignorance:

Assuming these two types of ignorance, "My eyes are black, and my eyes are not black" is true, because my eyes are indeed black, but they are also dark brown, so they are not black. At the same time, they could be a shade of black which, to you, is not black, and a shade of colour, which is inconsistent with your perception of "not black". Hence, "My eyes are not black, nor are my eyes not black" is also true.

This reasoning can be taken further — to 8 state logic, 16, 32, and so on ad infinitum.

## Beyond Donkeys, Elephants and Lotus Buds

![Image](https://cdn-images-1.medium.com/max/800/0*MNa9VDAKkrvExu8h.jpg)

Now, some of you might have understood me; some of you might have misunderstood me. Some of you might have both understood me and misunderstood me; while some of you might have neither understood me, nor misunderstood me.

Either way, let me conclude with an exercise for the reader. (I have localised the questions for a Sri Lankan audience. Friends in other parts of the world should appropriately localise the questions. For example, in the US, UNP/SLPP should be replaced with Republican Party/Democratic Party.)

Suppose by some magical power you ceased to be ignorant of nuance and overlap. In this blessed state, which of the following would you label as TRUE, and which as FALSE?

Please comment with how many TRUEs you got, and how many FALSEs you got.

## Works Cited

[1] [Online]. Available: https://en.wikipedia.org/wiki/United_States_elections,_2018.

[2] [Online]. Available: https://medium.com/@nuwan.senaratna/who-do-you-side-with-c983109e304f.

[3][Online]. Available: https://www.aljazeera.com/news/2018/10/sri-lanka-president-sacks-prime-minister-appoints-rajapaksa-181026174208405.html.

[4][Online]. Available: http://www.wect.com/2018/11/10/sri-lanka-president-dissolves-parliament-calls-election-2/.

[5][Online]. Available: https://www.bbc.co.uk/news/world-asia-46196979.

[6][Online]. Available: https://www.bloomberg.com/news/articles/2018-11-14/sri-lanka-parliament-passes-no-confidence-vote-against-new-pm.

#### 12

# The History of AI

### (in less than 60 seconds)

![Image](https://cdn-images-1.medium.com/max/800/0*Bi81jXVxWABeNVWQ.png)

### AI 0.0 = Human generated Rules (Before 2000)

Humans codified their knowledge and intuitions into Rules, and programmed machines to implement these rules.

### AI 1.0 = Learning from Data (After 2000)

Progress in computer hardware, and the ability to collect large amounts of data, led to Statistical Machine Learning on Data.

### AI 2.0 = Learning from Data, generated from Simulation (After 2010)

Further progress in hardware, led to fancy simulation software. Simulation led to vast amounts of data, which in turn could be used to do more elaborate statistical machine learning (also running on fancier hardware).

### AI 3.0? (After 2020)

Simulating complex behaviour, including human behaviour?

#### 13

Shashank Bharath: "This" means a more freer distribution, and a more egalitarian distribution of data. One important shift with decentralized apps is that data could be stored, owned or controlled by the original owner. This gives the owner more control on data — and leads to a more equitable distribution. See https://medium.com/@timberners_lee/one-small-step-for-the-web-87f92217d085 for more details.

#### 14

# Web 4.0

![Image](https://cdn-images-1.medium.com/max/800/0*kaJmESRg-8CbWx_R.jpg)

Technology (both Hardware and Software) is full of "version numbers". For example: I use an iPhone 8, running iOS 12.1. I'm writing this blog on a computer running Mac OSX 10.13.6, using TextEdit 1.13. Often, we are on the lookout for new version (and their new version numbers), because they might have "cool" new features, or patches to problems in old versions. Often, we are also reticent to install a new version, because it might not be sufficiently tested, and might have unexpected bugs.

The Internet, or World-Wide-Web (WWW) or simply the "Web" is also a giant collection of hardware and software. It is continuously evolving, and unlike OSX or TextEdit, it has not explicit version numbers or releases. On the other hand, it is possible to look at the Web as a whole, and observe various characteristics that can be compared to what the web was 5 or 10 years ago. It is also possible to identify what characteristics might be desirable for the web, and encourage builders of hardware and software to implement these.

In this article, I share a short list of "characteristics" that might be desirable for the future web (which I call "Web 4.0"). Like iPhones or OSX, I consider these "desirable" because A) they add new functionality to the web, and B) fix bugs in the current version.

However, before that, let us review the previous "versions" of the web.

### Web 1.0, 2.0 and 3.0

The term "Web 1.0" is a "retronym"; it was invented retrospectively contrasting it to "Web 2.0". Web 2.0 enhanced Web 1.0 principally in the following ways [1]:

While there is no universally agreed upon definition of Web 3.0, it is trending in the direction of a "collective intelligence" made up of billions of devices and humans connected in a single intelligence whole [2]. That is, while 2.0 was made up of many independent systems, 3.0 will form a collective whole.

### Web 4.0

I'm going to list my characteristics "comparing and contrasting" it to the current web (which is probably best described as a mix of 1.0, 2.0 and 3.0).

### References

[1] https://en.wikipedia.org/wiki/Web_2.0

[2] https://www.webopedia.com/TERM/W/Web_3_point_0.html

#### 15

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

#### 16

# #CoupLK

### From First Principles

## What is #CoupLK about? What do you think?

90% of opinion and discussion on our (Sri Lanka's) constitutional crisis (a.k.a. #CoupLK) fall into groups A or B — split firmly along partisan lines. There is a small minority who purport C. While the options are true to some extent, not one represents the whole truth.

But then, what is the whole truth about #CoupLK? How should we think about it? What should we do? If you're interested, read on.

## Which hat is the President wearing?

Laws (including the constitution) are paradoxically circular. Citizens elect legislators. Legislators pass laws. Laws govern citizens.

![Image](https://cdn-images-1.medium.com/max/800/1*qnERuuGTgXvY_Tk_q4aI8Q.png)

Since citizens (through their elected representatives) pass laws, citizens are the masters of laws. But since said laws govern the said citizens, the citizens are also servants of the laws. Hence, citizens need to wear two hats: MASTER and SERVANT. To complicate matters, when a citizen is allowed to be MASTER and when they should be SERVANT is also defined in the said laws.

At the core of the #CoupLK is a particularly special citizen, the President, and it is not clear which hat he is wearing, or should be wearing.

## Why be SERVANTs?

For laws to work, all of the following must be true.

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

What are you going to do? Comments welcome :)

#### 17

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

In contrast, many of the worst democracies have had democracy imposed on them — sometimes by force. In such places democracy is unstable, and certainly not in equilibrium.

## Post Democracy

Our current decade is further proof of the causal direction of development, equity and enlightened beliefs and a sense of identity, and democracy. Many countries that self describe as "strong democracies" are battling authoritarian forces. It's difficult to ignore the following observations:

All these points to a weakening in the "causes" of democracy. It also highlights the fallacy of ignoring the fact that democracy is more an complex, emergent effect, than a simple cause.

## Sri Lanka: To Democracy or Not To Democracy?

For the first 2 millennia of our recorded history (~500 BCE to 1500 CE), Sri Lanka was an absolute monarchy. For the next ~450 years it was ruled by European powers who were in turn absolute or constitutional monarchies [7]. We have been a democracy for a relatively insignificant 70 years. And when I say "been a democracy" — I don't imply things have been perfect. Our democracy has been marred by violence, corruption and exclusion.

While, the last couple of elections in Sri Lanka have been relatively free and fair, the politicians elected have been, with a few exceptions, abysmal. This begs the question — "What's wrong with our democracy?" And more significantly, "Is democracy the right way for Sri Lanka?"

Reading so far, you might assume that I'm skeptical about democracy. You might even assume that I'm opposed to democracy, and am directly or indirectly proposing an alternative. If so, you misunderstand me.

Let me summarize my feelings towards democracy as follows:

### Qualities of Democracy

### So what should Sri Lanka do?

As Sri Lankans we should not be overly obsessed by Democracy as a virtue by itself. Instead, we should focus on the causal factors out of which democracy will emerge.

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

#### 18

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

#### 19

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

#### 20

# On Pain and Pleasure

### From Philosophy to Calculus

### Philosophy in a time of influenza

Do you remember the last time you got the flu? I had an attack of flu some months ago.

The first day was bad. I had a temperature. Sore throat. Cough. Dull headache. It was difficult to sleep. Nor did I feel up to reading a book, or listening to something. I had no appetite to speak of. As I said, it felt pretty bad. That was the first day.

But it's the second day I want to talk about. Or more specifically, the evening of the second day. Because on the evening of the second day, I was beginning to feel a bit better.

I was still quite sick and weak. The mercury was not quite back to normal, and I coughed a lot. But I had the first indications that the disease was on its way out. I felt better. And oddly, clearly better than I was before I got sick in the first place — when I was "not sick". I felt pleasure, optimism, gratefulness, and the overwhelming sense that things were going to get better, not just with my health, but with life in general.

Pain and pleasure are like the first and second days of flu; completely relative. You feel pleasure if what you felt before was worse. And you feel pain, if what you felt before was better. Hence, there is a limit to the amount of pain and pleasure you can feel. For after a couple of days, "feeling good" becomes pleasure-less, boring and meaningless, and perhaps even annoying. Conversely, while "feeling bad" might painful and hard to deal with at first, but soon becomes bearable as time goes on.

### Calculus in a time of procrastination

![Image](https://cdn-images-1.medium.com/max/800/1*I1pk6WPDDhZ5MV_Rbv04hQ.jpeg)

[1] https://www.flickr.com/photos/internetarchivebookimages/14596852489/

[2] https://tradingeconomics.com/iraq/gdp-growth-annual

[2] https://tradingeconomics.com/japan/gdp-growth-annual