#### Article 244 · June 19, 2020

# The Data Mafia

### And why we exist

![Image](https://cdn-images-1.medium.com/max/800/1*Ej7PudXet9WP_Uv4A4CKfA.jpeg)

Recently, a colleague accused me of being a "Data Mafioso". When I asked him to clarify what he meant, he said something like this.

"Whatever we say, you ask, ‘What does the data say?'. And when you learn that the data says nothing, you kill our idea."

## Red or Blue?

To make this more concrete, let us consider a (hypothetical) example of an idea.

Suppose you are designing the User Interface (UI) of a website. Suppose you want to decide what colour the "Accept" button should be. The default colour (that everyone seems to use for this type of button is "Blue"). But your designer believes "Red" is a better option.

So you do a "User Study" to figure out what colour you should use. You bring in seven potential users and show them the two options.

Now, suppose five think "Red" is better. Two think "Blue" is better.

Your designer colleague is triumphant. The data from the user study confirms his theory: 71% to 29%.

But does the data actually agree?

## What the data says

We use data to test theories. For example, we use the data from the "User Study" to test the "Red Button is best" theory.

How do we "test"? Data has no mind. It is not a human with subjective opinions. And so has no opinion on Red buttons and Blue buttons. So we can't ask the data "Is the Red Button best?". On the other hand, we can ask it to compare two different theories.

For example, we could ask, "Is the Red Button better than the Blue button?" Or to be more precise, we could ask "Does the User Study confirm the theory that the Red Button is better than the Blue button?"

Data answers this (more specific) question, but answering an even more specific question. "What is the probability that the User Study results occurred by chance?" Now if this probability is high, then we can't conclude that Red is better than Blue. In other words, "the data says nothing".

Now, if a user had an equal 50–50 chance of preferring Red or Blue, the possibility of a User Study with seven people picking Red five times or higher is about 23%.

Is 23% high enough? If we want to be very sure that the theory is correct, we tend to be conservative on what "probability is high" means. In other words, we pick a low limit for "high" — usually 5% or 10%. If we are less picky, we might choose a higher threshold like 20%.

## More Samples

The risk of putting a red button on a UI is probably low. So we could afford to be a bit liberal on how we use data. So while 23% is generally considered "high", we might cut some slack and use it in the UI.

There is a simple way around this. Show the button to a few more users. The more samples, the more sure data is. For example, if we had 14 users, and 10 picked "Red", the chance of a random result is down to about 9%. If we had 21 users, and 15 picked "Red", the random chance is down to 4%.

## Risk

But like I said, the risk of putting a red button is probably low. On the other hand, other situations can be more risky.

By Red-Blue example was inspired by a far more risky experiment. A prominent economist was proposing a particular development program for Sri Lanka. Seven other countries tried the same program. In five, the results were positive. In two, it failed. The economist was going around "pitching" the program's "success rate of over 70%".

I tried to explain that 5/7 was not enough. Pointing out that there is a high (23%) chance that the success thus far could be random. And unlike the red button, the program was costly — in terms of tax-payer money, and the opportunity cost of using that money for something else. Hence, we should have been more careful.

Sadly, the powers-that-be bought the "over 70%" pitch, and Sri Lanka became, not the sixth success case, but the third fail case.

## Theories upon Theories

Unlike Web UIs, where it is relatively cheap to run even millions of experiments, this is not true with large development projects. We can't run a $50M project in 30 countries, just to validate if the project would work. Hence, often we "override" the data with a high-level theory. We say the idea works because some theory says so.

In many cases, this works. For example, we know at what velocity and acceleration an apple falls to the ground. Because we have a higher-level theory. The laws of kinetic motion.

But in some cases, higher-level theories don't work. Because they themselves don't have enough evidence to back them up. You can only "replace data with a theory", if that theory itself is backed by data.

To confuse things further, some high-level theories are backed-up by even higher-level theories. Leading to end-less hierarchies of theories.

## #SkinInTheGame

Life is full of uncertainly. And sometimes we have to make decisions, without data. Not knowing if it would work.

Hence, we could have argued that Sri Lanka had to try the development project, even if the "data wasn't sure". However, when we do take such decisions, we should make sure that the decision makers and experts behind the decision take responsibility.

In ancient Rome, the engineer who designed a bridge had to sleep under it for some length of time. If the bridge collapsed, the engineer was killed. Similarly, experts should face some downside when their decisions turn out to be wrong.

While the Sri Lankan tax-payer is laden with more debt, the economist who proposed, the "Red" project is still a paid adviser to the government. He, sadly, had no skin-in-the-game. We took the punishment for his mistake.

## Concluding Serendipity

When there is a risk, we should trust the data as much as possible. And when data is expensive, we need to make sure that incentives are aligned. And that the appropriate people sleep under appropriate bridges.

On the other hand, when risk is low, we can ignore the data or interpret it liberally.

There is an even more extreme decision we could take. In the strange case of the red button, why did we choose between red and blue? Why not green? Or purple or black? Why did we accept the designer's theory? Real creativity comes from looking for solutions in a completely unconstrained manner. Maybe we should have implemented a button that changes colour randomly. Often the results could be poor. But if the risk is low, we could afford these "mistakes". On the other hand, we might also "stumble upon" a genuinely fantastic colour that no one else thought. Purely by chance.

A true Data Mafioso would understand all these factors. And the reason we (Data Mafiosi) exist is not to make sure data is used all the time. But, instead, to make sure data is used appropriately at the appropriuate time.

To summarise, the true Data Mafioso will make sure the following happens:

* Risky + Data is Expensive ⟶ Use Skin in the Game

* Risky + Data Not Expensive ⟶ Use Data Conservatively

* No Risk + Data Not Expensive ⟶ Use Data Liberally

* No Risk + No (Good) Theories ⟶ Forget Data, Forget Theories, Trust in Serendipity