#### Article 308 · March 11, 2021

# Programming Subjectivity

A Metaphor

## An Objective Universe

Suppose you observe a flag flying in the distance. And suppose you ask yourself, "What color is that flag?"

The following snippet of code can represent this act of observation:

```
const flag = Object({  name: 'flag',  color: 'red',  weight: 'light',  texture: 'soft',})
```

```
function observe(x, attributeName) {  return x[attributeName];}
```

```
>> print(observe(flag, 'color'))'red'
```

Your observation would tell you that the flag is red. In this universe, we assume that (at least around the time when the flag was observed), the flag and the flag's properties (like color) are both constant and objective.

## A Subjective Universe

But what if the universe behaved differently? What if the act of observing actually created the flag?

```
function observe(x, attributeName) {  x = Object({    name: 'flag',    color: 'red',    weight: 'light',    texture: 'soft',  })  return x[attributeName];}
```

```
>> print(observe(flag, 'color'))'red'
```

In this subjective universe, observing the flag would yield exactly the same observation as in the objective universe. "What color is the flag?", you ask. "The flag is red", replies the universe. But, if you didn't ask, there would have been no flag.

## A Subjective Universe (v2)

But what if we went further? What if the universe created, not a flag, but a flag that was (even more) objectified to your question?

```
function observe(x, attributeName) {  x = Object({    attributeName: 'red',  })  return x[attributeName];}
```

```
>> print(observe(flag, 'color'))'red'
```

In such a universe, the flag would only have properties that you (the observer) cares about. You care about color — the flag has only color. You care about texture — then, the flag has only texture, and so on.

## A Subjective Universe (v3)

Could we go even further? We could.

```
function observe(x, attributeName, attributeValue) {  x = Object({    attributeName: attributeValue,  })  return x[attributeName];}
```

```
>> print(observe(flag, 'color', 'red'))'red'
```

Why might such a hyper-subjective universe be possible? Consider the following:

What exactly is "red"? It has nothing to do with the nature of the flag. True — the flag's material absorbs all types of light except that which represents red. But even this has nothing to do with the "experience of red".

As far as I can tell, this "experience of red" exists nowhere but in the mind of the observer.

![Image](https://cdn-images-1.medium.com/max/800/1*jILh6RAkW6JYpYpybzuOww.jpeg)