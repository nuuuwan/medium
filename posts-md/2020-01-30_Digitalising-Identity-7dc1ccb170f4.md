#### Article 210 · January 30, 2020

### Digitalising Identity (Part 1)

# How much of my private data is public?

### And what is my "data exposure"

We all share a lot of our data with the outside world. Not just on social media. But also with Banks, Hospitals, Phone Operators and the Government. In Sri Lanka, the "process of sharing" is still often manual. When we open a bank account, we often fill in paper forms.

But digitalisation will likely replace these manual processes in the next few years. Making many processes more efficient and accurate. And benefit consumers in all sorts of ways. But there are also risks. Particularly around privacy and data exposure.

This article is the first in a series about "Digitalising Identity". Written from a Sri Lankan perspective.

In this article, I address one of the most fundamental questions about Digital Identity: What is my "data exposure"? Or other words, how do you answer the question "How much of my private data is public?"

## Example Data: Sri Lankan National Identity Card

![Image](https://cdn-images-1.medium.com/max/800/1*D5mhSAj3KU8g3AQE6jezEQ.png)

Consider the data on your the front face of your Sri Lankan National Identity Card. It contains the following fields of data.:

* 12 digit NIC Number

* Full Name

* Sex

* Date of Birth

[We will ignore signature and face photo, until a later article]

How much information is here? Let's consider each field one by one.

### Sex (and Information Content)

In computer science, we have a notion of "information content". Which we can use to measure the "amount of information" in some piece of data. "Information content" is the smallest number of bits needed to store some data. Equivalently, it is the least number of "binary questions" that might infer the data. A binary question is a question with only two possible answers.

For example, "Sex" takes two values "MALE" or "FEMALE". Requiring a single bit of storage. Say "0" for "FEMALE" and "1" for "MALE". Using the "question intuition": To reconstruct the data, you only need to ask one question. Something like "Are you FEMALE or MALE? " or "Are you FEMALE?"

Note, in practice, we might use more bits to store the data. For example, we could store "Sex" as six Unicode characters (which would take 96 bits). But "information content" refers to the "smallest". Which is just one bit.

### Date of Birth

What is the information content of "Date of Birth"?

If we use a MySQL DATETIME data type to store "Date of Birth" we could need up to 24 bits of data. However, this is not the "smallest" amount of data. Assuming that we are only interested in people who were born within a window of about 200 years, "Date of Birth" can only take about 73,050 distinct values.

What is the information content of 73,050 distinct values? We can answer this question by asking "What is the least number of binary questions that might infer this data?"

The list of binary questions would be something like this:

* Is your DOB in the first half of the 200 years or the second half?

* If you answer "second", we split that half into two halves and ask the same question.

* And so on.

* In the end, we will end up with just two possible birthdays.

The mathematicians among you will notice that the number of questions is about log2(73,050) or (rounding up) 17 questions. Hence, "Date of Birth" needs about 17 bits.

### NIC Number

>>> 1970 510 1234 5

The Sri Lankan NIC number consists of four parts:

* First four digits: Year of Birth (e.g. 1970)

* Next four digits: Day number in Year of Birth (e.g. 10 if you were born on January 10th) + 500 if you are female. Hence, a female born on January 10th would have "510". A make would have "010".

* Next four digits: A serial number

* Last digit: a checksum

What is the information content of the NIC Number?

You would have noticed that the information contained in the first seven digits is the same as the "Date of Birth" and "Sex" combined. Hence, it is 17 + 1 = 18.

The four-digit serial number can take any value, and hence has 10,000 unique values. Thus, if has log2(10,000) or 14 bits of data.

The final checksum derives from the other 11 digits. And hence, it doesn't contain any new information of its own.

Hence, the NIC Number has 18 + 14 = 32 bits of data.

### Full Name

What is the total number of unique "Full Names"?

It is difficult to say exactly. But probably a number in the order of the size of our population. Or ~22,000,000. Hence, "Full Name" contains about log2(22,000,000) or 25 bits of information.

[In practice, information systems rarely store "Full Name". And instead store a combination of "First Name", "Middle Names" or "Middle Initials" or "Initials", and "Last Name". For simplicity, we'll ignore this fact for now.]

### Complete NIC

Hence, what is the total amount of information in the NIC?

Since, "Date of Birth" and "Sex" are contained in "NIC Number", the total information is 32 (NIC Number) + 25 (Full Name) = 57 bits.

![Image](https://cdn-images-1.medium.com/max/800/1*HjD-LON_8XX5dPCujUzy-w.png)

## Case I: Bank

Suppose you want to open a Bank Account. And suppose the Bank needs your "Full Name" and "Date of Birth".

[In practice, Sri Lankan Banks need all the NIC information. Plus tonnes of other details. But let us assume this scenario for now.]

Let's also assume that your only private data are the 57 bits of information on your NIC. For the sake of these cases.

How much information have you "given away" to your Bank? 25 (Full Name) + 17 (Date of Birth) = 42 bits. Hence, 42/57 or 74% of your private data is "publicly exposed".

![Image](https://cdn-images-1.medium.com/max/800/1*QKUu7O5XNe3BuejUoNl9gA.png)

## Case II: Minimalist Bank

Suppose Sri Lanka has comprehensive and enforced data protection and privacy laws. Suppose these laws make sure that institutions (like Banks) only ask customers for a minimal set of information. The minimum they need to do their job.

For example, suppose that "Date of Birth" is only used to verify that the customer is 18 years or older. Hence, the Bank is not allowed to ask for "Date of Birth". Only "Are you over the age of 18?"

Since "Are you over the age of 18?" is a binary question, this contains 1 bit of information.

[Note, this "intuitive binary question" approach, is an approximation. "Are you over the age of 18?" actually needs less than one bit. But we'll ignore this technicality. You can learn more at Entropy.]

Hence, you only need to give the bank 25 (Full Name) + 1 (Are you over the age of 18?) = 26 bits of data. Instead of 42 bits. Now, your data exposure is 26/57 or 46%.

![Image](https://cdn-images-1.medium.com/max/800/1*t0MwOPaE0aQwwImOCQNNQQ.png)

## Case III: Hospital

Suppose you need to visit a doctor, and the Hospital need your "Date of Birth" and "Sex". This would contain 17 (Date of Birth) + 1 (Sex) = 18 bits of data. 18/57 = 32%.

![Image](https://cdn-images-1.medium.com/max/800/1*oFBSerOi8u2dKTTxuYoHNw.png)

Now, suppose you also opened a (non-minimalist) bank account (like Case I). What is your total data exposure? Across both Bank and Hospital?

Before we answer that question, why would you care?

Suppose you are of the Mormon religion. And suppose your Bank knows this. And suppose the Hospital has a racist policy of charging Mormons double. However, since the Hospital doesn't have your "Full Name", it doesn't know your religion. As far as the Bank and the Hospital are concerned, you are "two people". Each can't connect your two accounts.

But what if a teller at the Bank (who knows your name) is married to an accountant at the Hospital. They might pass information between each other. And your privacy is blown.

How might we represent this in our "data exposure" metric?

## Average Data Exposure

Let's assume that the Bank and the Hospital are the only data collecting organisations in Sri Lanka.

And let's assume that they are equally important. We could compute your "average data exposure" as a weighted average of your exposures. Or 74% × 50% + 32% × 50% = 53%. In the case where they can't share data.

Now, in the case where the teller and the accountant are sharing your data with each other, each has 25 (Full Name) + 17 (Date of Birth) + 1 (Sex) = 43 bits. Or 43/57 = 75%. Since, both parties have all this data, your "average data exposure" is 75% × 50% + 75% × 50% = 75%.

Many techniques can minimise "data exposure" when confronted with multiple (possibly colluding) data collection organisations. Including "differential privacy".

## Summary and Future Articles

In this article, we discussed the computer-scientific concept of "Information Content". And, based on this, derived a "data exposure" metric. We extended this to an "average data exposure" metric, to consider multiple data collecting organisations.

We also discussed "minimalism" or how data collecting organisations should only collect the minimal data needed to "do their job". "Minimalism" and many other concepts we discussed (and will discuss in future), depend on data protection and privacy laws.

We also, explained how "data exposure" can explode when data collecting organisations collude to (possibly illegally) share data.

In future articles, I hope to address the following questions:

* How do we design minimal data sharing schemes?

* How does data exposure relate to identity and authentication?

* How do we prevent "data exposure" explosions, when confronted by colluding data collecting entities?

* How do we implement all of this in a digital system?

Please comment if you have ideas on more interesting questions.