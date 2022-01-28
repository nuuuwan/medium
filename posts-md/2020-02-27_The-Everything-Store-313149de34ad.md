#### Article 215 · February 27, 2020

# The Everything Store

### Part I: What to Store

[The ideas expressed in this article are not original. This is more of a "thinking aloud" exercise. The Computer Scientific theory behind this article can be found here]

Suppose you had a database. Which could store anything. Any piece of data. Any information. How might we design such a store?

Let's start with the "things" it would store.

## Entities

By entity, I mean "things" that have some unchanging identity. Eternally. We could call them "eternities" even.

What other things would we need to store?

## Relationships

Suppose we were to store a news article in the Everything Store. The article could have an author. An organisation might publish it. The article itself might refer to various people and organisations. And finally, there is the article itself. Including its text.

A "relationship" is a collection of entities, united by some meaning. For example, we could say,

>>> "Author X wrote article Y, and organisation Z published it. Article X also referred to politicians P, Q and R, and ministries M and N.".

Note, we can write meaning in different ways. For example,

>>> "Article Y was written by Author X and published by organisation Y".

## Attributes

Finally, entities have characteristics or "attributes" that are not entities themselves. The "text" of the article, for example.

![Image](https://cdn-images-1.medium.com/max/800/1*AGbdoD6z753AbLRnb0dCKQ.png)