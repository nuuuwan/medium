#### Article 122 · October 1, 2019

# Flags of the World

### And asking machines difficult questions

## Supervised and unsupervised learning

>>> "How many categories of flags are there there in the world?"

You might say,

>>> "Some flags are red, white and blue. Some are yellow, green and red. Some have only one colour. Others have many colors."

But what if we ask a computer this question? An unusual question to ask a machine, because usually, we ask machines other questions. Like,

>>> "Here's a picture of a face. Can you tell me who it is?"

Or

>>> "Here's some data about this person who turned up on a website. What advert should we show them?"

Or

>>> "Here's a video from the front camera. Is that a lorry ahead of us?"

All these questions have one thing in common. The computer learns to answer a question, by training itself on previous examples. Similar questions and correct answers. To train a computer to recognise a face, we would provide it with millions of images of faces, together with a label (E.g. "Albert Einstein"). Hence, when a friend uploads a picture of Albert, Facebook can tag him.

This type of learning based on examples is called supervised learning. Most of Artificial Intelligence consists of supervised learning.

But asking a computer "How many categories of flags are there there in the world?", does not consist of learning based on examples. You might provide the computer with images of flags. But you don't give it any right answers. The computer will have to go off an learn what are the categories of flags for itself. Without human help.

This type of learning, without human help, is known as unsupervised learning.

## K-Means

So I decided to ask my computer the question.

One common unsupervised learning method is clustering. In our example, the computer will go and group similar flags. Each group becomes a type. One simple clustering algorithm is k-means clustering.

The computer starts with the items to cluster. In our example, flags. It goes to Wikipedia, and downloads about 200 flags from various countries and territories.

I decide to make things easier for the machine by asking it to categorise flags only based on colour. Ignoring things like shape of the flag, objects like animals etc. Hence, for each flag, the computer notes what colours exist, and what proportion of each colour.

For example, the Sri Lankan flag consists of about 36% yellow, 32% maroon, 11% orange, 11% green, and various smaller amounts of other colors.

![Image](https://cdn-images-1.medium.com/max/800/1*eHo_sJaWjUQVydfqK0QtTA.png)

Once the flags are ready, the computer runs the k-means algorithm.

We must first specify how many categories the computer should find. Let us say seven categories.

The computer picks seven flags at random, and then finds how the other flags are similar to these flags. Those flags join the groups of the first seven flags.

For each group, we find the "mean flag". A "mean flag" is the flag that you would get if you averaged all the flags together. For example, here is a representation of the Sri Lanka Flag, the British Flag, and their mean:

![Image](https://cdn-images-1.medium.com/max/800/1*JQ6yFYIsW7QQUl2CRBzvIw.png)

The computer then finds how the other flags are similar to these mean flags. With each step, the clustering improves. And on and on. When we are happy with the categories, we stop.

So how did my computer do?

## The Results

### 1. Pan-Arab Colors

The first cluster consisted of White, Black, Green and Red. Also known as the Pan-Arab colours. Including the flags of Jordan, Palestine, Kuwait and the UAE.

The cluster also had a bit of yellow and blue, which combined with red to admit flags like Andora and Moldova.

![Image](https://cdn-images-1.medium.com/max/800/1*cBHmhBmnXIGOSVvqUeHv9g.png)

### 2. Red, White and Blue

The second cluster consisted mostly of Red, White and Blue. Including France, the UK, the USA, and the Netherlands.

![Image](https://cdn-images-1.medium.com/max/800/1*FnVLt5vANGzCC__vSXjZYA.png)

### 3. Pan-African Colors

The third cluster consisted of Red, Yellow and Green, also known as the Pan-African colours. This also included some non-African flags like Sri Lanka.

![Image](https://cdn-images-1.medium.com/max/800/1*ViwP0YXDhgywI0Xg2vkNUg.png)

### 4. Red

The fourth cluster consisted of flags that were dominated by red, including China, Turkey, and Vietnam.

![Image](https://cdn-images-1.medium.com/max/800/1*2ZSyVfIugixHZAOvrzsYPA.png)

### 5. Lighter Blue

The fifth cluster consisted of flags with lighter shades of blue, including Greece and Honduras. It also had a little yellow and green which admitted Sweden and Gabon.

![Image](https://cdn-images-1.medium.com/max/800/1*Dl6_53UZ2pSRlRFI_NOXVw.png)

### 6. Dark Blue and Green

The sixth cluster was dominated by dark blue and green. Including New Zealand and Bangladesh.

![Image](https://cdn-images-1.medium.com/max/800/1*rs5hUjpNlnXCkLUqZa2ZBA.png)

### 7. White

The last cluster was dominated by white. It included the flags of India, Japan, South Korea, Finland and Israel.

![Image](https://cdn-images-1.medium.com/max/800/1*4vmOkxEL28wbr-vPcd4P9g.png)

## Concluding Thoughts

Obviously, my computer had not heard about Pan-African leagues or Red-White-And-Blues. These were my own annotations. But it is uncanny how it picked up these patterns.

On the other hand, these clusters do include some noise that humans would not have included. For example, in addition to the dominant colours, each cluster included some "minority" colours, that introduced some "rogue" flags.

On yet another hand, we could choose to see this as the computers "opinion". It has devised a new type of flag, which humans might not have agreed with, or come up with.