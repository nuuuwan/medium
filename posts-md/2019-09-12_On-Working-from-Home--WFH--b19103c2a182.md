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