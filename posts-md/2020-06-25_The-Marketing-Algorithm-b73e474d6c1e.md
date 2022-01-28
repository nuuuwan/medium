#### Article 248 · June 25, 2020

# The Marketing Algorithm

### And the Importance of Smart Marketing

Fifteen years ago, some friends of mine built a translation system. That would translate English into Sinhala. They "exposed" the system via an API ("application program interface") so that other people could also use it.

When a journalist asked my friends "whether the system was valuable", they replied that it was "fairly valuable". Especially for those who "wanted a tool to translate English into Sinhala".

The API is still available today (I think). But I doubt anyone uses it. If you want to translate English into Sinhala, it is much easier to use Google Translate.

![Image](https://cdn-images-1.medium.com/max/800/1*zMX19zF_8t5-ruR1ASK4wQ.png)

If you were expecting yet another story of how Google killed a promising startup, sorry. This article is not one of those. To begin with, my friends were not a startup. They all had "day jobs", and the project was just a hobby.

Instead, this article is about "Value". More specially, how people (like my coder friends) routinely underestimate the value of products (like the translation system); Why this mis-underestimation happens; And how to avoid this mistake.

## Reductive Value

All "goods" (i.e. product and services) satisfy needs. The "value" of the good is proportional to this "need", and also relative to all other needs a person has. Often goods don't satisfy needs in isolation.

For example, the product "salt" is commonly used with the products "pepper", "chicken" and "cooker", and service "cook". They combine to satisfy the need of "hunger". In this way, goods don't produce isolated value, but are part of "value chains".

By Reductive Value, I mean "describing the value of a good in terms of its contribution to the value chain". When my friends described their product as "a tool to translate English into Sinhala", they were doing exactly this. There was no reference to other goods or value chains. Nor an explicit reference to needs.

## Expansive Value

About a year after I first learnt about my friends' translation system, I met a man who described himself as an "entrepreneur". When I asked "Mr. Entrepreneur" what he did, he said his latest product was about "connecting Sri Lanka to the internet". At first, I thought he was trying to build some extensive telecommunication system. Or distribute free computers to our rural poor.

When I asked him if that's what he was trying to do, he shook his head, opened is a laptop (enormous by today's standards), and played a fuzzy video.

The video looked like a screen-capture of someone opening a browser, then going to the yahoo news website, and finally opening a New York Times article. Surprisingly, the article was written not in English, but in Sinhala.

Mr. Entrepreneur's strategy for connecting Sri Lanka was a web-browser. That translated all text from English to Sinhala.

[While this might seem a bit of a sham, it does make sense if you think about the numbers. Even today. Only about 10% of Sri Lankans are fluent in English, while over 70% have access to internet broadband.]

The video I was not of a real browser, but an animation of one. Mr Entrepreneur was still looking for a programmer to build his idea. I don't know what happened to him, but I was intrigued by his idea.

Engineering-wise, his product was the same as what my friends had built. But while my friends described their product as a humble "tool", Mr Entrepreneur framed his product as a grand vision for completely changing how the internet is used in Sri Lanka.

What intrigued me most was the difference in framing. Mr Entrepreneur considered a value chain (accessing the internet) where his product was a small (but essential) link. Then went on to expand the description of the value of his product in terms of the overall value of the chain. This is what I meant by "Expansive Value".

## But isn't this cheating?

Mr Entrepreneur had something of the air of a charlatan. With his big talk and fake videos. My friends, on the other hand, were naive software engineers. As honest as they come.

And weren't they more honest to describe their product in terms of precisely what it does? As opposed to something much larger? That depends. On what the point of the description is.

Honest and objective descriptions are all good. But at the end of the day, goods satisfy needs. And the description should describe the need, not just the good. My friends' description made no explicit reference to needs. Conversely, Mr Entrepreneur's "expansion" was not dishonest. Instead, he was doing what was necessary. Framing the good in terms of essential needs.

## Dumb Marketing and Markerters

In the Technology field, we tend to respect a solution more than we respect problems. We tend to appreciate "goods" (especially if they are complex and esoteric) more than we respective descriptions of needs that the same goods might satisfy.

Hence, how my friends behaved was utterly normal. They had built a solution and expected the requisite respect. What need the solution satisfied was someone else's business.

In Tech, these "someone elses" tends to be "marketing people" and other low-life. Undeserving of respect. Because they don't have to do difficult things. Like engineering.

This pre-judgement has become a self-fulfilling prophecy. Marketing departments are mostly communication departments for "translating engineer-speak" into language that "ordinary people understand". In other words, they are conduits for communicating "Reductive Value".

As a result, marketing departments tend to be underfunded, and comprise with dull and uncreative people. A vicious cycle that perpetuate the myth that marketing and marketers are dumb.

## Smart Marketing and The Marketing Algorithm

Instead, Marketers in Tech should instead be looking to maximise the "Expansive Value" of what is built. Or even better, what should be built.

If maximising Reductive value is hard, maximising Expansive value is even harder. It requires understanding the complex economics of value chains and a keen understanding of human behaviour and psychology. It consists of identifying every single value chain where a product might be a link and determine what value chain is most valuable.

This sort of "Smart Marketing" is what marketing should be.

Let me conclude by reframing the difference between reductive value and expansive value in a form techies would understand. Enter "The Marketing Algorithm".

```
def get_reductive_value(good):
```

```
"""This is what engineers maximise"""
```

```
return "value of the good in isolation"
```

```
def get_expansive_value(good):
```

```
"""This is what marketers maximise"""
```

```
max_value = 0
```

```
for value_chain in all values chains where good is a link:
```

```
max_value = max(
```

```
incremental_value of good in value_chain,
```

```
max_value       )
```

```
return max_value
```

## Acknowledgements

In his excellent book, Alchemy, Rory Sutherland describes "Expansive Value" as magic. Finding it is indeed a more "magical" process than merely engineering Reductive value. Mr Sutherland's ideas have significantly influenced this article.

![Image](https://cdn-images-1.medium.com/max/800/1*qWVfe61Ocvv7QdnoJhYSuQ.jpeg)