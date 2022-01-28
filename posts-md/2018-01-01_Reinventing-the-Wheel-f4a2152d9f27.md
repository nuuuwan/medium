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