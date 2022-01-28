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