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