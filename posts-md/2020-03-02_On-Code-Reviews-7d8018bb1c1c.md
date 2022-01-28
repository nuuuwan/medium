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