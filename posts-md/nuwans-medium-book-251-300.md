# Book 6

#### Articles 251 to 300

#### Article 251 · July 6, 2020

RE: On the allocation of 160 seats by population, on which year's population was this based on (am wondering if the analysis of the current numbers are skewed by IDPs)

2012 Census.

#### Article 252 · July 6, 2020

### 2020 Sri Lanka General Elections

# The Split Effect

### A Hypothetical Experiment

A friend of mine claimed that the UNP + SJB split would actually be beneficial. And that the split would win more seats, than if they contested the 2020 Sri Lankan General Election under a single party. My friend's reasoning was something like this: "Many would-be UNP-voters would not vote UNP, because Ranil is leader. Similarly, many would not vote UNP because of Sajith. With the split ticket, the Anti-Rs would vote SJB. And the Anti-Ss would vote UNP."

![Image](https://cdn-images-1.medium.com/max/800/1*TCR8QSjIV1zO8UWWNe-B8A.png)

Many in my Twitter audience (a highly biased and statistically insignificant sample) seem to agree.

>>> 

There might be truth to these beliefs. However, there is another factor that might put a spanner-in-the-works: Our (not so) proportional representation system itself.

In (Not so) Proportional Representation, I discussed how our proportional representation system is "not completely proportional". How "Bonus Seats", "The 5% limit" and "Rounding Luck" favour some parties more than others. These factors might bend the result in favour or against the UNP + SJB.

But which is it "in favour" or "against"?

In this article, I attempt to answer this question.

## Methodology

Our last general election was in 2015. The UNP came top with 106 seats, while the UPFA got 95.

I consider a hypothetical result: if the UNP contested 2015 on a UNP + SJB split. We assume that the total UNP votes were split equally between the UNP and the SJB. Note, this is an assumption — which might not hold in practice. Also, the equal or 50–50 split also an arbitrary assumption. In practice, the split might be different, especially across districts.

## The "Results"

In theory, if the system was completely proportional, there should be no difference. In practice, there is a significant difference.

![Image](https://cdn-images-1.medium.com/max/800/1*T74PRIoz6fZq_iVrxAZKrQ.png)

In the UNP + SJB contested 2015 split, the UNP would win 48 seats, and the SJB would win 45 seats. For a total of 93. 13 seats less, compared to no split. The hypothetical split effectively "flips" the election in favour of the UPFA.

[Note: Why did the UNP get three more seats than the SJB, if we split equally? That's because of rounding errors. In a few cases, the UNP and the SJB need to share an odd number of seats. In these cases, we assigned all the seats to the UNP. In practice, two seat-eligible parties getting the same number of votes is rare.]

What explains the loss? All the factors which we mentioned above.

### Bonus Seats (-11 Seats)

In 2015, the UNP got the most number of votes in the Colombo, Gampaha, Kandy, Matale, Nuwara-Eliya, Digamadulla, Trincomalee, Puttalam, Polonnaruwa, Badulla, and the Kegalle Electoral Districts.

On a hypothetical split, they would not get the most number of votes in these districts and hence lose their bonus seat. The alternative district winner (in 2015, mostly the UPFA) would benefit from the UNP's bonus seat losses.

### Rounding Luck (-1 Seats)

On a split, the UNP would lose one seat in each of Matara, Batticaloa, Digamadulla because of rounding effects. However, the UNP would also gain one seat in Trincomalee and the National List.

In general, "Rounding Luck" should mostly "cancel out".

### 5% Limit (-1 Seats)

In Jaffna, the UNP got one seat with 6.67% of the vote. On a split, the UNP and SJB would get about 3.33% each, or below the 5% threshold, a party must get to be eligible for seats. Hence, neither would win a single seat.

## [UPDATE 7/6] Addendum: The Converse

We see that the UNP + SJB looses about 13 seats by contesting seperately, if they get the same total votes. What about the converse question? How many additional votes must the get to get the same number of seats? That "bump" is around 7%.

## Concluding Caveats

This article is not a prediction. It is purely an exercise to demonstrate how our proportional representation system behaves when a party splits.

Also, we considered a 50–50 split. Which is the worst-case scenario, because it maximizes the "Bonus Seats effect". In practice, the split might be more asymmetric.

With CoViD-19, comic infighting within all parties, and many other nuances, 2020 is likely to be different from all previous elections.

Caveat emptor!

#### Article 253 · July 20, 2020

### 2020 Sri Lankan Parliamentary Election

# Real-Time Projections (#GenElecSL2020)

### "Predicting" the Election in Real-Time

With the hardships of CoViD19, many seem to have lost interest in #GenElecSL2020. It would be interesting to see if turnout exceeds the previous lows of 61.26% (in 2010) and 63.60% (1989). But as with many things with little data, and no precedent, predictions are almost impossible. Hence, I'm not going to attempt predicting turnout, nor the final result.

Instead, this article is like the Election Projections article I wrote around #PresPollSL2019. Where I ask the question:

"Can we use early results to project and predict the final result? And if so, how accurate would such a projection be?"

## The Experiment

To find out, I simulated #GenElecSL2015. As with my previous article,

* I assumed that election results report in order of result size. Starting with smaller results like postal votes. Ending with larger polling divisions like Homagama, Kaduwela, and Nuwara Eliya-Maskeliya.

* For each set of reported results, I built a regression model. That predicted the outcome based on these reported results. The model trained on the previous six general elections (between 1989 and 2010).

* I validated the results by computing error bounds.

However, the similarities end here. Presidential elections are simple. The "final result" is a "winning candidate". Selected based on who got the most votes islandwide. General elections are far more complicated. And our model needs to consider this.

## Complexities of General Elections

A presidential election is, effectively, one, islandwide election. A general election is a collection of many elections.

An "election" is held for each electoral district. Parties gaining at least 5% of the total district vote qualify for seats. A certain number of seats are pre-allocated to each district. These divide among the qualifying parties, proportional to their votes. Of the 225 seats in parliament, 196 are so allocated.

The remaining 29 for the "National List". These divided among parties, proportional to their total islandwide votes.

Hence, the "final result" of a general election is not a single winner, but an allocation of seats. Far more complex.

Every Sri Lankan presidential election has been a "two-horse race". Between candidates from the two main parties. Some might say, some have even been "one-horse races". No "third candidate" has won more than 4.63% of the popular vote.

Hence, predicting a presidential election is easy. Merely predict the votes each major party candidate would get.

General Elections are far more complicated. While the two major parties still get most of the seats, other parties also get significant numbers. Parties also field many candidates, who might not necessarily be permanently loyal to the party. As it is common for politicians to "jump". Multiple parties form complex coalitions, without precedent.

Hence, when it comes to predicting general elections, the "concept" of a "party" is of little value. The election profile of the same "party" in two elections could be very different.

## The Model

Our General Election projection model takes these complexities into account.

With presidential elections, we trained a model as follows. To predict how many votes a party would get in a yet-unreleased polling division. Based on the polling divisions released. Each party had is own model.

In contrast, with general elections, we can't assume "party" as a factor. Hence, our model party agnostic. Each party shares the same model. If "party" does have some significant effect, our model does not capture this.

## The Results for 2015

Let's look at the model's predictions at results in intervals of 40.

![Image](https://cdn-images-1.medium.com/max/800/1*_SWyVyM-9vYEnK65mLrJxA.png)

At 40, the projected result is very similar to the final result for the UNP and the UPFA. But the error bars are very wide.

![Image](https://cdn-images-1.medium.com/max/800/1*Fz_HMz7gm267k4Ef93jlwg.png)

At 80, the error bars narrow somewhat, but are still very wide.

![Image](https://cdn-images-1.medium.com/max/800/1*aza4DHbSIhD0HPc-GDzTcg.png)

At 120, the error bars narrow further, but not enough to call a winner.

![Image](https://cdn-images-1.medium.com/max/800/1*dtlP_xLCGXFw3QRkLb6f4Q.png)

The error narrowing continues into 160. But not winner call as yet.

And finally, the final result.

![Image](https://cdn-images-1.medium.com/max/800/1*qSk-6UI5doZHDvpTEWpoTw.png)

Here's a graph of the seat predictions for the UNP and UPFA, as each result came in. Low and high error bars in thiner line.

![Image](https://cdn-images-1.medium.com/max/800/1*fPUlA-LN2NWV5j0yul15aA.png)

## The Results for 2010

2010 was a far more "one-sided" general election. And many were asking the question if the UPFA would get a two-thirds majority. Many are asking the same question about the SLPP this time around.

Sadly, while it was clear, early that the UPFA would win a majority, the "two-thirds" question remained unanswered right up to the end.

![Image](https://cdn-images-1.medium.com/max/800/1*5mPAEHSM5hDuC1O1PJJIVg.png)

## Concluding Warnings

When training data is scarce and problems complex, prediction is, not only difficult but often inaccurate and weak. This was my constant warning in my presidential election articles.

General elections have about the same amount of data as presidential elections (counting only the Proportional Representation Era). However, as we noted, they are several orders of magnitude more complex.

Hence, I must sound my warning even louder.

#### Article 254 · August 4, 2020

### 2020 Sri Lankan Parliamentary Election

# Understanding Parliamentary Elections

### Notes on Articles 96, 98, 99 and 99A of the Sri Lankan Constitution

"Will the SLPP get Two-Thirds?" is the "Big Question" of the 2020 Sri Lankan Parliamentary Election. I don't hope to answer this question, because I don't know the answer.

On the other hand, if you are interested in this question and other questions about #GenElecSL2020, understanding how elections work is key. Particularly, how seats are assigned.

Articles 96, 98, 99 and 99A of the Sri Lankan Constitution, collectively provide all the information you need to understand parliamentary elections in Sri Lanka. This article is based on my own notes of these articles, together with some illustrative examples and complementary data. Hope they would be useful to you too.

[Disclaimer: I'm no lawyer, nor constitutional expert. My only qualification for writing this article is that I can (to a point) read and write. Hence, take my notes with a pinch of salt].

## Article 96. Electoral Districts (EDs)

1. Sri Lanka must divide into between 20 and 25 Electoral Districts (EDs). A Delimitation Commission defines the districts, their names and their boundaries.

Currently, Sri Lanka has 22 EDs.

![Image](https://cdn-images-1.medium.com/max/800/1*r_183FOayh-vW7sTP97zHA.png)

2. An entire province could be one ED. Or divided into two or more electoral districts.

Currently, no province is a single ED. The Western, Central, Southern, and Eastern provinces divide into three EDs each. The Northern, North-Central, North-Western, Uva and Sabaragamuwa provinces divide into two each.

3. The boundaries of EDs respect the boundaries of Administrative Districts (ADs). Hence, either a) an ED is the same as an AD; or c) an ED is a combination of two or more ADs; or c) an AD is a combination of two ore more EDs.

Sri Lanka has 22 EDs and 25 ADs. Currently, the Jaffna ED is a combination of the Jaffna and Kilinochchi ADs. The Vanni ED is a combination of the Mannar, Vavuniya and Mullaitivu ADs.

All the other 20 EDs are the same as an AD. All except one, have the same name as the corresponding AD. For example, the "Colombo Electoral District" is the same as the "Colombo Administrative District". The one exception is the Digamadulla ED, which is the same as the Ampara AD.

Sri Lanka has no AD which consists of multiple EDs.

4. The Delimitation commission assigns four seats to each province. And divides these among the EDs.

In this way, Sri Lanka's nine provinces get 36 seats. The current division among EDs is as follows:

![Image](https://cdn-images-1.medium.com/max/800/1*oxDBgV2z6U02-FRe0N2h7g.png)

5. Delimitation Commission makes decisions by majority. If there is no majority, the Commission's Chairperson decides.

6. The Delimitation Commission's Chairperson communicates decisions to the President.

## Article 98. Number of members returned by the several electoral districts and their apportionment among such electoral districts.

1. 196 Seats divide among the Electoral Districts (EDs).

2. Of the 196, 36 divide as described in 96.4. [i.e. four per province, and divide amongst the EDs in each province].

3. Paragraphs 98.4, 98.5, 98.6, 98.7 describe how the remaining 160 [i.e. 196 minus 36] seats are divided.

4. The "Qualifying Number" is defined as follows:

```
"Qualifying Number" =   "Total Number of Registered Voters in entire Country"    / 160" ROUNDED DOWN
```

For example, there are 16,263,885 registered voters for the 2020 General Election. This gives a qualifying number of 101,649.

5. Each ED is assigned "Total Number of Registered Voters in ED / Qualifying Number — rounded down" seats. [Let's call them "Whole Seats"]

For example, Galle has 867,709 registered voters. Hence, it's Whole Seats can be computed as follows:

```
Registered Voters / Qualifying Number= 867,709 / 101,649= 8.536
```

```
Whole Seats = 8Remainder = 0.536
```

6. Any balance seats assign in order of EDs with the largest fractional remainder of "Total Number of Registered Voters in ED / Qualifying Number". [Let's call these Remainder Seats]

In 2020, 149 seats were assigned as Whole Seats, leaving 11. These were assigned to the EDs with the highest fractional remainders.

The whole seats, remainder seats, the seats from Article 99, the seats from Article 96.4 and the total number of seats for the ED, as as follows:

![Image](https://cdn-images-1.medium.com/max/800/1*9w_f_vj2NnBD8q1OWOQu8g.png)

This method of allocating seats to districts is known as the Hare Quota Largest Remainder Method. As we shall see later, this is also how seats allocate to parties in elections.

7. If there is a tie, i.e. if two or more EDs have the same fractional remainder, seats are assigned by lot.

8. The Election Commission publishes the above information in a Gazette.

![Image](https://cdn-images-1.medium.com/max/800/1*GM11SycSqpblWVaxbpQPTg.png)

9. The "Number of Registered Voters" is computed from the register of electors at the time of the relevant election.

## Article 99. Proportional Representation (PR)

1. Each Electoral District (ED) has a number of seats, as published in 98.8.

2. Each voter votes for a party or independent group (IG). And also indicates a preference for up to three candidates.

3. Each party/IG submits one nomination paper. Each party/IG may nominate as many candidates equal to the number of seats in the ED plus three.

For example, in 2020 Colombo has 19 seats. Hence, a party/IG contesting Colombo may nominate up to 22 candidates. Similarly, Trincomalee has 4 seats. Hence, parties/IGs contesting there may nominate upto 7 candidates.

4. Each registered voter is entitled to one vote. Even if their names appear on an electoral register in more than one district.

5. Candidates elect from an ED, in order of preference votes.

6a. Parties/IGs with less than 5% of the total votes in the ED disqualify from getting seats for the ED.

For example, in 2015, the JVP received 4.27% of the votes in Kurunegala, and hence were disqualified from getting seats. The 15 seats in Kurunegala were divided amongst the only two parties that exceeded 5%: The UPFA (49.29%, 8 seats) and the UNP (45.87%, 7 Seats).

In the same 2015 election, the JVP received 6.74% of the votes in Colombo, thus qualifying for seats.

6b. For the computation of seats, all votes for disqualified parties/IGs are excluded. The remainder is known as the "Relevant number of votes":

```
"Relevant number of votes" =   "Total votes in the ED for all parties/IGs"     — "Total votes in the ED for parties/IGs disqualified"
```

In 2015 in Colombo, only the UNP, UPFA and JVP qualified for seats:

![Image](https://cdn-images-1.medium.com/max/800/1*0lTvxCL8ee29DBW9KAOxeA.png)

The Relevant Number of Votes was 1,196,197. 11,752 votes from parties that failed to reach the 5% threshold, were excluded.

7. The "Resulting Number" of a party/IG in an ED, is defined as follows:

```
"Resulting Number" =   "Relevant Number of Votes"     / (Total Seats for ED minus One)" ROUNDED UP
```

(Note, the "minus one" is set aside for the bonus seat.)

For 2015 Colombo, the Resulting Number was:

```
"Resulting Number" = 1,196,197 / (19 - 1)= 66455
```

8. Each Party/IG is assigned "(Total Seats for ED minus One) / Resulting Number of Party/IG — rounded down" seats. [Whole Seats]

9. The balance seats assign in order of EDs with the largest fractional remainder of "(Total Seats for ED minus One) / Resulting Number of Party/IG." [Remainder Seats]

As I mentioned earlier, this method is known as Hare Quota Largest Remainder Method.

10. The party/IG with the highest number of votes gets an extra "bonus" seat.

The whole seats, remainder seats, bonus seat, and total seats by party for Colombo in 2015 is as follows:

![Image](https://cdn-images-1.medium.com/max/800/1*VlnzPwbXpfhJKb0yxTCbqg.png)

11. If there is a tie, i.e. if two or more Parties/IGs have the same fractional remainder, seats are assigned by lot.

12. In the above calculation, "Rejected Votes" are excluded.

13. If a candidate's seat becomes vacant, the candidate with the next highest number of preference votes is elected.

## Article 99A. Election of Members of Parliament on the basis of the total number of votes polled at a General Election

* After 196 seats are allocated based on ED, the remaining 29 seats [which together make up Sri Lanka's 225 member parliament], are allocated proportional to total votes obtained nationally. Also, known as the "National List". The allocation method is as described in Paragraphs 98.4, 98.5, 98.6 and 98.7.

For example, the Votes by party, Total Votes, Qualifying Number, Whole seats, Remainder seats, and Total National list seats for the 2015 Parlimentary Election are as follows:

![Image](https://cdn-images-1.medium.com/max/800/1*rOzOqg6zfNxoVVQHNlqCVw.png)

* Each party/IG submits a list of candidates who might elect to these seats.

The submissions for 2020 are here.

![Image](https://cdn-images-1.medium.com/max/800/1*X9PUGA7HCdrP7GKB2MfWhQ.png)

#### Article 255 · August 8, 2020

### Things that CS Courses Don't Teach You

# Bad, Good and Great Programmers

### Phrase-bookers, Pastichers, and Novelists

## The Phrase-Booker

I usually begin an onsite-coding-interview with an easy-difficulty question. Good Coders take a few minutes at most to answer this question. I then ask a medium-difficulty question, and if the candidate gets it right, a hard question.

Then, why do I ask an easy question? To filter out the bad coders. If a coder flunks one of my easy questions, we can end the interview, and save everyone time. On some rare occasions, I do ask a second easy question. For example, when a candidate gives an interesting, but the wrong answer to an easy question. But, as I said, these are rare.

...

One candidate who flunked an easy question asked me why I ask questions like that. When, if in "real-life" if they had to find an answer, they could Google it?

Writing code is like speaking a language. A way of communicating ideas. To both machines and humans. As a tourist might ask "How do I get to the railway station?", the following snippet of code asks a computer, "What is the square root of two?"

```
math.sqrt(2)
```

Now, as you might survive on a Phrase-book while touring a foreign country, one could find answers to easy coding questions by Googling (like finding the square root). And that would be fine if the point of the easy question was to "get the right answer".

Instead, the point of the coding question is to check other things. To see how the coder constructs code. To see how they connect it with different concepts. To see if they can combine it with other pieces of code that they've written in the past.

![Image](https://cdn-images-1.medium.com/max/800/1*lBXQEN_mAkPWQUWQczS0gw.jpeg)

## The Pasticher

"Pastiche" is a work of art that imitates another work of art. It might be complex and elaborate. But it is not original.

A Pasticher is a better coder than a Phrase-Booker. They don't have to Google the answer to an easy (or even medium-difficulty) coding question because they already know the answer. They already know all the data structures and all the algorithms. All the design patterns and programming styles. All the programming languages and technologies.

But then, you might ask, what is wrong with a Pasticher?

Not much. The ideal pasticher that I describe is very useful. Many a technology company would love to hire them.

But they have one flaw. While they are great at Pastiche, they are poor at originality. Real creativity, where they create something new. The pasticher is like the professor of literature, who is unable, nonetheless, to write an original work of their own.

The Phrase-Booker can't solve problems (without Google). The Pasticher can only solve the problems that they know. They can't solve the problems that they don't know.

Now, this might be fine for many software jobs, where most problems are known problems. But if you are to build something original, then you need something better: The Novelist.

![Image](https://cdn-images-1.medium.com/max/800/1*0ZPWC8j42PFjP07XAhKsZQ.jpeg)

## The Novelist

The hard thing about hard-difficulty coding problems is not that they are hard. They are not much harder than medium questions. A good hard question is one that could have many answers. Some mundane and standard. But some ingenious and creative.

The Pasticher gives one of the standard answers to a hard question. It might be right in theory, but wrong in practice. Because the goal of a hard programming question is to test novelty and creativity. Not correctness and standard-ness.

A good pasticher usually earns a hire at a coding interview. But they are reasonably common. A Novelist, on the other hand, is rare. And a novel and imaginative answer to a hard question (which is also the "right" answer), earns a "strong hire" in my book.

We know how to become a Pasticher. It is a matter of learning things, like algorithms and design patterns. But how does one "learn" to be a Novelist?

Here's my step-by-step approach:

* It helps to be a Pasticher first. Just as some of the most celebrated novelists are well-read and familiar with other novelists, it helps to build a solid base in programming theory. In other words, try to be a good programmer before you decide to be a great one. If you don't end-up being a Novelist, you'll at least be a Professor of Literature.

* Don't try to be a Novelist directly. Try to approach the problem obliquely. For example, try to learn about the nature of programming and philosophy of programming without worrying too much about programming itself. Study programming languages "comparatively". I.e. the similarities and differences of different programming languages.

* They say the Novel (and not the Novelist) writes the Novel. Similarly, with truly creative programs, the Program writes the Program. Hence, try and make programming a subconscious skill. This requires a lot of repetitions and practice — many hours spent at the keyboard. Try and acquire as many synaptic connections in your brain by working on different programming problems. Don't just do programming for work or university courses. Start some programming hobbies. Contribute to some open source projects. [Aside, an "Yes" to the question "Do you have any side projects?" is an excellent interview question. But be sure to verify any answers. A lot of interview candidates are good at faking].

* Make sure you have dedicated time to code. In a traditional workweek of 40 yours, there are ten slots 4 hours long. Say, one before lunch and one after lunch on each working day. This works for me because I'm a "morning person". It might be afternoon and evening, or even, evening and night, if you're a night-owl. Make sure you have as many slots completely free — I.e. no meetings and no distractions. If you have, say 6–7 free 4-hour slots per week, you can be very productive. If you are an engineering manager, inspect your report's calendars to see how much dedicated time they have.

* Finally, being a Novelist is a creative process. You need energy and rest to be creative. Make sure you exercise and have enough sleep. I find my "programming creativity" severely drops when I don't have enough sleep. For the same reason, I'm not a fan of software engineers doing "all-nighters". They might be sufficient for solving known problems, but if you want a coder to be creative (i.e. solve unknown problems), make sure they get to sleep.

![Image](https://cdn-images-1.medium.com/max/800/1*0OVoliTL5CU3rZ16INvPnA.jpeg)

#### Article 256 · August 8, 2020

# Valhalla

### On heaven, hell and the afterlife

![Image](https://cdn-images-1.medium.com/max/800/1*HB4Fu996pEg3BorlG1_zuw.jpeg)

In the Netflix TV Show, Vikings, the old warrior Tostig pleads with Earl Lothbrok. "Please let me fight", he says [in not so few words].

Why battle? Because he is alive. Fought many battles. Lost many comrades. Flirted with death many a time. But Tostig is still alive. And he wants to die. In battle.

But, why die in battle? Because of Valhalla.

When Viking Warriors die, Odin, God of War and Death, invites them to feast with him. In the "Hall of the Slain", or "Valhalla".

Warriors eat with their comrades in arms. And drink. And then afterwards fight. Each other. To the death.

After death, the dead warriors reappear. In Valhalla — the Hall of the Slain. To eat, drink, flight, die and reappear again. For the cycle to continue.

...

This is the "ideal afterlife" or "heaven" for the Viking warrior. Very different from the heaven found in other Western theology. Like the ones with gentle angels with white wings, playing harps, and supping on milk and honey (an excellent laxative, according to Mohamed Ali).

On the one hand, I, myself, am not a fan of the harps and honey heaven. The idea of playing dominos with Mother Theresa or Saint Benedict of Nursia for the rest of eternity, is not quite my scene.

On the other hand, being a card-carrying coward and pacifist, I'll pick milk and dominos. Over drunk murderous warriors. Anytime.

On a third hand, there is something I like about the idea of Valhalla.

...

Bravery in battle, and angels with wings are a contradiction.

If you told a soldier that if he dies in battle, he'll end-up playing a harp, A) he might not believe you. Or worse B) he might refuse to fight — given the utterly boring consequences (i.e. dominos etc).

The Valhalla-pitch is both more convincing and less contradictory.

...

Related, aficionados of the Buddhist Sutra will notice a striking parallel in the Yodhajiva Sutra. Between the "Hell of the Slain" and Valhalla.

#### Article 257 · August 9, 2020

### 2020 Sri Lankan Parliamentary Election

# Did the Greens stay Home?

### What the data says

## Did the Greens stay Home?

The 2019 Presidential Election had 13.2M valid votes. That number dropped to 11.6M in the 2020 General election.

About 1.6M fewer valid ballots.

Some claimed that this was due to many UNP/SJB supporters staying home without voting. Others argued that they did vote, but many spoiled their ballots. Resulting in the SLPPs near-2/3 landslide.

True? False? What does the data say?

Read on to find out.

## Valid Votes vs Green Support

Did the Greens Stay Home?

If so, we would expect a more significant reduction in the number of valid votes in UNP/SJB strongholds compared to SLPP ones.

Let us investigate this claim first.

For each polling division (and postal/displaced votes), we plot the % change in valid votes from 2019 to 2020, against the % of votes the NDF got in 2019. We plot the 2019 NDF wins in green, and the 2019 SLPP wins in red.

>>> E.g. The valid votes in the Chilaw polling division dropped from 93,885 in 2019, to 75,415 in 2020. Or a % change in valid votes of -19.7%. In 2019 the NDF received 40.0% of the vote, to the SLPP's 54.6%. Hence, a red plot.

![Image](https://cdn-images-1.medium.com/max/800/1*fhp5GzsEn1MfQEu3WItRHg.png)

We see the opposite of what we would expect if the "Green Stayed Home". The most considerable reductions in valid votes are in polling divisions that the SLPP won in 2019. Our trend line (noisy, but significant) indicates an increase in valid votes, as the NDF vote in 2019 increased.

Of course, this only indicates that there were (relatively) more valid votes in NDF polling divisions. And fewer in SLPP polling divisions. It says nothing about specific voters. It could be that SLPP supporters in NDF divisions voted more. And UNP/SJP supporters in SLPP divisions voted less.

But nor can we claim that the Greens stayed home. More likely the opposite.

## Rejected Votes vs Green Supporters

The other claim was the Greens did go and vote (our data does agree with this). But they spoiled their votes.

If this were the case, we would see more rejected votes in NDF polling divisions. Let us investigate this second possibility.

For each polling division (and postal/displaced votes), we plot the % rejected votes in 2020, against the % of votes the NDF got in 2019. As before, we plot the 2019 NDF wins in green, and the 2019 SLPP wins in red.

![Image](https://cdn-images-1.medium.com/max/800/1*ZuYmiAqJlEfu50EjQdHvyg.png)

Unlike, before we do see a positive trend. The % rejected votes in 2020 increase with NDF support in 2019. Unfortunately, this trend is not statistically significant, as there is too much variation in the % of rejected votes. Particularly among smaller NDF divisions.

This graph is similar to one comparing NDF support in 2019 to rejected votes in 2015.

![Image](https://cdn-images-1.medium.com/max/800/1*-VwFVbnDkV3ZUm2QwUJ7EA.png)

Hence, there is no evidence to support the ballot pooping theory either.

## Conclusions and Take-Aways

On the one hand, caveat emptor. With 24-carota aurum knobs on.

The methods described in this article are not the best ways of answering our questions. A more in-depth and more detailed study, ideally, some combination of exit polling and voter polling in general, would give more significant results.

On the other hand, our results do indicate that some "popular intuitions" (e.g. "The Greens stayed home" or "The Greens spoiled ballots") might be flawed. Or even contradict the data.

Hence, if you take away one thing from this article:

Don't blindly accept your intuitions. Or those of your friends and neighbours. Or what you might read on WhatsApp. The truth might prove you wrong.

...

You can find the data used in this analysis at https://github.com/nuuuwan/public_data/blob/master/gen_elec_sl_2020/gen_elec_sl_2020.analysis_unp_home.csv. Originally extracted from http://elections.gov.lk.

#### Article 258 · August 9, 2020

### Data Science 101

# Making Data Talk

### 9 Dos and Don'ts Data Analysis

This article is based on a talk I delivered at Verite Research, a few weeks before the 2019 Sri Lankan Presidential Election.

...

Data Analysis is an interrogation. The data analyst is the interrogator, and the data is the interrogated.

![Image](https://cdn-images-1.medium.com/max/800/1*KJJtjCQTiXnpwmzbALu3CA.png)

The interrogator has a bunch of tools. Some legal. Some illegal. Some ethical. Some not so ethical.

This article is about using those tools. Effectively. And ethically.

## 1. Do ask Questions

![Image](https://cdn-images-1.medium.com/max/800/1*L8-WmEKH2hJ6hMxbRXV1Ng.png)

There is no point in interrogating someone, if you have no questions to ask. If you're silent, the data will be silent.

So you have to have questions. Good questions. Interesting questions.

...

I started one of my articles by asking the question, "How many voters are floating voters?" [A floating voter is a voter who is not bound to a certain party. At an election, they could vote for any party.]

At the beginning, I didn't know how to answer this question. But even if you can't answer your question, you might be able to answer a different question.

So while I didn't know "How many voters were floating voters", I did find a way of estimating "How many voters were base voters". [A base voter is the opposite of a floating voter. Voters who always vote for the same party.]

This Dorling Cartogram represents voters who'll always vote UNP. And how they are distributed across polling divisions. The size of the circle is proportional to the number of base voters.

![Image](https://cdn-images-1.medium.com/max/800/1*6xUO_fjw36v5jXFrc1-pOA.png)

In Sinhala we have a colorful phrase "කැපුවත් කොළ" ("Kepuvat Kola"). Voters who support the UNP so much their blood is green. This is the data analytics representation of කැපුවත් කොළ.

...

Once you have an intermediate answer, you can apply some theory to get the answer you want.

I figured that the number of floating voters is what you get when you subtract all base voters from all the voters.

And so, we get an approximate answer to our question, "How many voters are floating voters?"

![Image](https://cdn-images-1.medium.com/max/800/1*TnuCgOjKcaLLLu40SlMLsQ.png)

...

If you have an interesting question, you can (usually) find an interesting way to find an answer. The important thing is to ask questions.

## 2. Do Reflect on Data

![Image](https://cdn-images-1.medium.com/max/800/1*WfG5tPoitqXxFd6_39iABg.png)

When there is an interrogation in movies, there's always a "mirror scene". Where the police watch the prisoner through a one-way mirror.

And usually the police see some interesting things. Because the prisoner can't see them. And instead sees themselves. And tend to do interesting things.

Can we do the same mirror trick with data? Can we put data into a room and watch it? From behind a one-way mirror?

The answer is, we can.

And the way to make data "reflect", is to see what new conclusions it implies.

...

For example, we can take our floating voter data, and see how it reflects on the 2015 election.

![Image](https://cdn-images-1.medium.com/max/800/1*yaMjBnhSqDngSzniu07EFw.png)

This cartogram represents how the two main political parties performed among floating voters. And as expected, we see that the NDF dominated the floating vote.

...

We get an even more interesting reflection from 2005. Again the NDF dominates the floating vote, but not enough to win the election.

![Image](https://cdn-images-1.medium.com/max/800/1*37erqn3KwVmyfxWC-1DqVQ.png)

Many people talk about the LTTE boycott in the North, and how it affected the final result. But a less talked about point is how the NDF failed to win the floating vote in places like Colombo, Galle, Matara and Gampaha.

All those white circles represent floating voters, who didn't vote NDF, or just stayed home.

## 3. Do understand that Data is stranger

Too often, we think we understand the data. When in fact we don't. Sometimes data is strange. Or even. Stranger.

![Image](https://cdn-images-1.medium.com/max/800/1*pS93JWvcFIS2R1Bk2i7fwQ.png)

...

This is a map of the 50 United States of America and the District of Columbia. And a map of another presidential election.

![Image](https://cdn-images-1.medium.com/max/800/1*i5j3epTWaQhnn0i000x-4A.png)

The Blue states always vote for the Democrat Presidential candidate. The Red vote Republican. The other states are swing states. They vote for one candidate or the other.

The purple states are an interesting type of swing state. Known as Bellwether states. They not only swing, but they tend to swing in the right direction. They almost always vote for the candidate that wins the election.

In any data analysis, it is essential to realize that not all data is the same. For example, not all Polling Divisions are the same. Some might be Bellwether polling divisions.

...

I tried to answer this question and came up with this map. The eight purple polling divisions always voted for the winning presidential candidate.

![Image](https://cdn-images-1.medium.com/max/800/1*_D_-3hqykx-oAu3MnioS_w.png)

...

There are other ways in which data is also different. For example, Turnout can be very different across polling divisions. And this could be significant for elections.

![Image](https://cdn-images-1.medium.com/max/800/1*xql6TeVInFUNa_NRMiGkgw.png)

## 4. Don't let the data get the better of you

After I shared maps of floating voters and bellwether polling divisions, many people concluded that campaigns should focus on either the bellwether areas. Or the areas with the highest density of floating voters.

This shows some fallacies in thinking.

Bellwethers are bellwethers not because they influence the national results in some way. It's because their voter distributions happen to match the national distribution. The relationship is a correlation, not causation. So if a campaign targets a voter in Mawathagama , you might end up getting more votes in Mawathagama. But that won't "cause" you to get more votes Islandwide.

...

The problem with focussing on areas dense with floating voters is that causes you to lose out on other floating voters. The reality is that floating votes are everywhere. And concentrating on just some areas might win you polling divisions. But loose you the election.

...

In this controversial scene from Basic Instincts, Catherine Tramell not only taunts and intimidates her interregators, she ends up sending them in a completely wrong direction.

![Image](https://cdn-images-1.medium.com/max/800/1*v9awDlk5rIdW-RrNChnwWg.png)

Don't let the data get the better of you.

## 5. Don't torture data

I disappointed many by not predicting the result of next month's election. To exasperate these people, even more, I wanted to prove that it was hard to predict the outcome even after the results have been partially released.

To do this, I built a projection model. Which tries to predict the final result of the election using both previous election results. And the released results in the current election.

This graph shows the projected results for the 2015 election. The X-axis represents polling divisions as their results are released. The Y-axis represents the projected votes for each party. The red line is NDF. The blue line is UPFA.

![Image](https://cdn-images-1.medium.com/max/800/1*9cE-x3UPK8XVKMXUND0Eow.png)

Now, if you go by this projection, you'd assume that one party or the other is going to win the election. For most of this graph, it looks like red is going to win (as it did). But for some parts it might look like Blue is going to win.

But this is a wrong conclusion.

...

There are two types of interrogations. In one type, the interrogator wants to learn the truth. In the other type, the interrogator wants to force a confession.

![Image](https://cdn-images-1.medium.com/max/800/1*fnPX7YESx5M498Nm8ggUtw.png)

The problem with data is that with minimal torture, you can get it to say anything you want. So, if you want to learn the truth, the interrogation has to be sensitive and intelligent.

Sadly most data analyses fall into the forced confession category. The analyst has some specific outcome in mind, and they torture the data to call this outcome.

...

Let's look at my projection again. In this second diagram, you see the real state of the data. You see not one red line and one blue line. But three read lines and three blue lines.

![Image](https://cdn-images-1.medium.com/max/800/1*eL2XXrm9XwEFRUvEYWN7EQ.png)

Let's zoom in for more detail.

#### Article 259 · August 10, 2020

### 2020 Sri Lankan Parliamentary Elections

# So close, yet so far

### What if they got a few more votes...

Many expected Sunil Handunnetti of the JJB to win a seat in Matara. In fact, he did come tantalizingly close. If the JJB won just 4,212 more votes in Matara, they would have won a seat. And SH might have been "in".

But there were other examples. The JBB itself came much closer to winning seats in Kalutara and Hambantota, than it did in Matara.

In this article, I list some "so close, yet so far" cases. Where with a few more votes, more seats would have been won.

[For clarity, I only look at cases with less than 10,000 votes, or 15% of what the votes the party actually won.]

## TMVP (1 close calls)

In the National List, the TMVP would get an extra seat, at the expense of the OPPP (increasing their total to 1), with 67 or + 0.6% more votes.

## EPDP (1 close calls)

In the National List, the EPDP would get an extra seat, at the expense of the OPPP (increasing their total to 1), with 6,295 or +10.7% more votes.

## SLFP (1 close calls)

In the National List, the SLFP would get an extra seat, at the expense of the OPPP (increasing their total to 1), with 1,180 or + 2.3% more votes.

## UPA (1 close calls)

In Batticaloa, the UPA would get an extra seat, at the expense of the SLPP (increasing their total to 1), with 2,370 or + 8.1% more votes.

## SDPT (1 close calls)

In Vanni, the SDPT would get an extra seat, at the expense of the EPDP (increasing their total to 1), with 1,246 or +12.9% more votes.

## SJB (2 close calls)

In Kalutara, the SJB would get an extra seat, at the expense of the SLPP (increasing their total to 3), with 591 or + 0.8% more votes.

In Gampaha, the SJB would get an extra seat, at the expense of the JJB (increasing their total to 5), with 8,186 or + 3.4% more votes.

## JJB (3 close calls)

In Kalutara, the JJB would get an extra seat, at the expense of the SLPP (increasing their total to 1), with 1,662 or + 5.5% more votes.

In Hambantota, the JJB would get an extra seat, at the expense of the SLPP (increasing their total to 1), with 4,112 or +13.6% more votes.

In Matara, the JJB would get an extra seat, at the expense of the SLPP (increasing their total to 1), with 4,214 or +11.8% more votes.

## SLPP (4 close calls)

In Vanni, the SLPP would get an extra seat, at the expense of the EPDP (increasing their total to 2), with 1,390 or + 3.8% more votes.

In Nuwara-Eliya, the SLPP would get an extra seat, at the expense of the SJB (increasing their total to 6), with 7,223 or + 3.6% more votes.

In Badulla, the SLPP would get an extra seat, at the expense of the SJB (increasing their total to 7), with 7,897 or + 3.1% more votes.

In Gampaha, the SLPP would get an extra seat, at the expense of the JJB (increasing their total to 14), with 8,186 or + 1.5% more votes.

![Image](https://cdn-images-1.medium.com/max/800/1*syyrbCgvAzZiewBDVfyHZA.png)

#### Article 260 · August 26, 2020

### Tourism in Sri Lanka

# Every Hotel in Sri Lanka

### Visualising Tourism

Data is a strange beast. How it looks depends on how you look at it. If you look at it from a different angle, or even in a different color, it might look completely different.

For example, I thought I knew something about hotels in Sri Lanka. But when I took some data and plotted it, I came to some new conclusions.

...

Here is a map of every hotel in Sri Lanka. Each circle represents a hotel, rest-house or tourist accomodation. The area of the circle is proportional to the number of rooms. The color of the circle represents the type of hotel.

![Image](https://cdn-images-1.medium.com/max/800/1*09oTZGH9zxXNke98WNBfaA.png)

Here's a list of "insights" that occureed to me. They are not particularly novel. But I thought them "interesting".

### 1. Most hotels are on the South-West Coast

To be honest, I already knew this fact. Qualitatively, that is. But quantitative, I didn't expect the fact to be as skewed as it is.

Also, many would argue that Sri Lanka's best beaches are on the East coast. Sadly, tourist infrastructure in this part of the country is dwarfed by the other coast. Excluding Kandy, ancient capitals like Anuradhapura and Polonnaruwa also seem to have less infrastructure than expected.

Another example of කොළඹට කිරි?

### 2. Most hotels are in clusters

* The South-West can be clustered around towns like Kalpitiya, Negombo, Colombo, Panadura, Bentota, Hikkaduwa, Galle, Tangalle etc.

* Kandy, Nuwara-Eliya and Ella in the central hill

* Trincomalee, Batticaloa, and Potuvil (including Arugam Bay) on the East Coast

* Matale/Dambulla, Anuradhapura, Thamankaduwa (Polonnaruwa)

* Jaffna

* Various other small clusters

![Image](https://cdn-images-1.medium.com/max/800/1*0z8M45o0MnwDl0Gs1Xxn8w.png)

Many of the smaller clusters have few "Classified Hotels", and those that have them have a relatively smaller number of rooms.

### 3. Hotels Accommodation is proportional to population and wealth

Unsurprisingly, most hotels are in relatively populous and affluent areas. Compare the above maps to this map of poverty in Sri Lanka:

![Image](https://cdn-images-1.medium.com/max/800/1*ou8GFd307dwj0zAiyOh1yA.png)

The "causality" might run both ways: Hotels might make the local population wealthier. A wealthier local population might go on to build more hotel rooms.

Either way, mightn't more tourism lift up the economic lot of (say) the Eastern Province?

...

Caveat: The underlying data might need some updating. Take the suggestions below as "suggestions" and not "concrete proposals".

For details about data source and visualisation techniques see: https://observablehq.com/@nuuuwan/sl-tourist-accomodation]

#### Article 261 · August 27, 2020

### 2020 Sri Lankan Parliamentary Election

# How the JJB might have won 10 seats

### Lessons for next time

For many JJB supporters, the 2020 General Election was a disappointment. Winning only three seats, their disappointment was (probably) only second to the UNP (one seat).

The dissapointment might have been compounded by the fact that they came very close to winning more seats. In So close, yet so far (where I describe how with a few more votes, various parties might have won more seats), the JJB represented three of my "Top 10 so close misses".

Some might consider this "bad luck" — a misfortune. Others, however, might consider this "carelessness". I count myself in the second camp. Here's why: With a few more votes in a relative small selection of areas, they could have more than tripled their tally to 10 seats.

"But why flog a dead horse?", you might ask. "The election is over".

And you're partly right. There won't be another parlimentary election for some time. Then, why am I writing this article? For three reasons:

* Any party wishing to win any seats at the next parliamentary election, must begin preparing now. In this sense, JJB included, it's never too early to start.

* A party with ten seats in parliament has a lot more clout than one with three. Hence, if a party had a realistic chance of winning ten seats (and as we will see, the JJB had a realistic chance), they should take such opportunities very seriously.

* Even for larger parties, this exercise will be useful in determining which areas to focus on more, and which area less so.

### 3 Seats (actual 2020 Result)

Let's recap. The JJB won three seats. One each in Colombo and Gampaha, and one on the National List.

![Image](https://cdn-images-1.medium.com/max/800/1*0MnleWTwLbrlBjFaFQj4EA.png)

The bulk of their votes was in the Western and Southern provinces. With a few spikes in urban centers.

![Image](https://cdn-images-1.medium.com/max/800/1*9XdQaAJwFzXd6HlQ2UI2Tw.png)

### 4 Seats

![Image](https://cdn-images-1.medium.com/max/800/1*YdpokZ7QY-VPXOBbzCL3Yw.png)

The JJB's closest miss was in Kalutara, where they won 33,434 votes. This translated into 4.77% of the total vote. And hence, the JJB were disqualified from winning a seat on the 5% rule.

With just 1,700* more votes (or +5% of what they already got), they would have qualified for seats on the 5% rule, and won a seat.

* See Appendix: Methodology

### 5 Seats

![Image](https://cdn-images-1.medium.com/max/800/1*Z393JS-4ibkyeGtib6W_NQ.png)

Matara was the next closest miss. The JJB won 37,136 votes or 7.76% (well above the 5% limit).

Unfortunately, with just 7 seats allocated to the district (one of which is reserved for the winning party), 7.76% was not sufficient to win a single seat. This number was revised down from the 2015 General Election that had 8 seats allocated to Matara. In an 8-seat-Matara, the JJB would have won a seat.

However, even with 7 seats for Matara, just 4,300 more votes (+12%), the JJB would have won a seat. And Sunil Handunetti might have sat in Parliament.

### 6 Seats

![Image](https://cdn-images-1.medium.com/max/800/1*m9dyT57tkAeQ-VnekWtNjA.png)

The JJB's 6th seat would have come from Hambantota, where they won 31,362 votes, or 8.39%. Like Matara, Hambantota had only 7 seats.

With 4,200 votes (+13%, very similar to Matara), the JJB would have won a seat in Hambantota. And I wonder who the Handunetti of Hambantota would have been...

### 7 Seats

![Image](https://cdn-images-1.medium.com/max/800/1*WJntRMbDRUl3-AgB4ZRwdA.png)

Now things get a bit more difficult. But hardly impossible.

In the Badulla District, the JJB got 19,308 votes or 3.87%. 6,000 more votes (+31% of 19,308) or a total of 25,308 votes, would have got them over the 5% line, and won them a seat.

Now you might argue that +31% is a tall order. In 2001, the JVP did win 26,820 votes in Badulla, easily over the 25,308 they needed to win a seat in 2020.

Never has the JJB or any of its past reincarnations, won a seat in Badulla. However, in 2020 the seats allocated for Badulla increased from 8 to 9. And hence, Badulla was definetely "in play" for the JJB. Perhaps they didn't take it seriously.

### 8 Seats

![Image](https://cdn-images-1.medium.com/max/800/1*PthTvl8NwJGQz5g91Yer5Q.png)

The 8th seat would have come from Kurunegala, where the JJB won 36,290 votes, or 3.74%.

13,000 (+36%) more votes, would have won them a seat.

In percentage terms, 13,000 more votes would have got the JJB to around 5% of the votes. While they missed this target in most of the Kurunegala district, they did hit it in the Kurunegala Polling Division.

### 9 Seats

![Image](https://cdn-images-1.medium.com/max/800/1*8IdsbDCqV2rkxV4VT20kuA.png)

The 9th seat would have come from Anuradhapura, where the JJB won 24,492 votes, or 4.83%.

Another 9,000 votes (+37%) would have got them a seat.

Like the Kurunegala Polling Division, the JJB did relatively well in the more urban Anuradhapura East Polling Division. If they matched this performance in the rest of the district, a seat would have been guaranteed.

### 10 Seats

If the JJB succeeded in getting the extra seats in Kalutara, Matara, Hambantota, Badulla, Kurunegala, and Anuradhapura, they would also have got at least 38,200 more votes (1,700 + 4,300 + ... etc) islandwide.

This was well over the 22,600 extra votes nationally (or about 5% of the 445,958 votes the JJB actually won islandwide), they needed to win a second national list seat.

Hence, 10 seats!

## Concluding Thoughts

On the one hand, to be fair, not all the seats above are equal. While Kalutara, Matara and Hambantota were probably lost, Badulla, Kurunegala and Anuradhapura, clearly had to be won. And with a very strong showing at that.

On the other hand, both percentages and absolute votes to be won were not unreasonable numbers. Definitely within reach.

...

## Appendix: Honourable Mentions

* 11 Seats: Galle. A seat with another 12,100 votes (+40%)

* 12 Seats: Colombo. A second seat with another 28,300 votes (+42%)

* 13 Seats: Gampaha. A second seat with another 41,800 votes (+68%)

## Appendix: Methodology

There are two ways in which a party can get more votes: 1) "get out the vote" from their voters, who would have otherwise stayed home; 2) "steal" votes from other parties. In both cases, the votes of the said party would go up. In the former case, the votes other parties would stay fixed. While in the latter case votes would go down.

I assume the former case. It makes for easier analysis, because we don't have to assume how many votes the said party "stole" from other parties. Often, the "theft" is asymmetric. Regardless, for a smaller party like the JJB, the two cases lead to similar results.

* For simplicity, in this analysis, I've rounded-up the "more votes" to the nearest 100 votes. The actual number could be lower.

[You can run my "simulations" here: https://observablehq.com/@nuuuwan/how-the-jjb-might-have-won-10-seats]

#### Article 262 · August 28, 2020

### 2020 Sri Lankan Parliamentary Election

# Variations on Proportional Representation

### Some hypothetical scenarios

In Understanding Parliamentary Elections, I explained how Sri Lanka's Proportional Representation based electoral system works.

In particular, I discussed how our "proportional" system is not quite proportional, because of the following factors:

* Article 96 of the constitution assigned four seats to each of the nine provinces. These, in turn, were distributed amongst districts by the Delimitation Commission. Since, all provinces (big and small — by voter population) got the same number of seats, the smaller provinces got more seats relative to their size. Even within provinces, allocation of seats was not proportional to the voter population, further exaggerating the asymmetry.

* A Bonus Seat was allocated to the party getting the most number of seats in a district. The allocation happened if the party coming first got even one vote more than the party coming second.

* Parties qualified for seats at the Electoral District level, only if they got a minimum of 5% of the valid votes of that district. This 5% rule was often a disadvantage to smaller parties.

* Finally, differences in turnout meant that total seats a party received were not proportional to total votes. A party that got more votes in a district with higher turnout received relatively fewer seats.

In this article, I present some hypothetical scenarios, on what the seat allocation in the 2020 Sri Lankan Parliamentary Election would have been if the above "disproportionalities" did not exist.

## Actual 2020 Result

Let's begin with the actual 2020 result.

![Image](https://cdn-images-1.medium.com/max/800/1*mF4aeRl29tOdpDqaSJIv6w.png)

## 2020, ignoring Article 96

If we ignore Article 96 and assign seats to a district in proportion to their voter population, we get the following allocation.

![Image](https://cdn-images-1.medium.com/max/800/1*2sABnVKfegecxqlODVhc1A.png)

The new allocation favours bigger districts (like Gampaha) and disfavours smaller ones (like Vanni). With the new allocation, the 2020 result would have looked like this:

![Image](https://cdn-images-1.medium.com/max/800/1*Zj2gMWv5D4UPf3ZGY7A0gg.png)

Since the SLPP and JJB did relative better in larger districts, especially in the "South", they gain 4 and 1 (Matara) seats respectively, mostly at the expense of the SJB (-2) and the ITAK (-2).

## 2020, ignoring Article 96 + the Bonus Seat

When we remove the Bonus Seat privilege for the winning party, the SLPP loses six seats. Mostly to the advantage of the SJB that came "second" in many districts, which gains six seats.

![Image](https://cdn-images-1.medium.com/max/800/1*uRqo6b4JCKxvZ4XPTPKM_Q.png)

## 2020, ignoring Article 96 + the Bonus Seat + the 5% Rule

When we relax the 5% rule, the JJB gains four seats (Kalutara, Kandy, Galle and Kurunegala). The UNP also gains two seats (Colombo and Gampaha).

The SLPP loses six seats, and the SJB loses two seats.

![Image](https://cdn-images-1.medium.com/max/800/1*QlV7EeUI4qzTXrGdhHpRvg.png)

## 2020, with perfect proportionality at the national level

Finally, we look at how seats would have been allocation with "perfect proportionality". That is, if the seats parties got were exactly (save rounding error) proportional to the votes they received islandwide.

![Image](https://cdn-images-1.medium.com/max/800/1*7VUB0kCdiYzdT9bEyQIktA.png)

The allocation is very similar to the "2020, ignoring Article 96 + the Bonus Seat + the 5% Rule" with minor changes due to turnout. The SLPP and SJB lose two seats each. The UNP gains two seats, while the JJB and ITAK gain one seat each.

## Bonus: 2020, with a 12.5%

The 1978 Constitution that originally defined proportional representation stipulated a 12.5% threshold for parties to qualify for Electoral Districts seats. This was subsequently lowered to 5%, apparently at the request of smaller parties.

In this final "Bonus Scenario" we look at the what 2020 result would have been if we replace the 5% rule with the original 12.5% rule.

![Image](https://cdn-images-1.medium.com/max/800/1*H4oVAIREHVwXAu5uMtKcQA.png)

The chief loser in this scenario is the JJB, which loses its seats from Colombo and Gampaha.

#### Article 263 · September 1, 2020

### Notes on Buddhist Philosophy

# Dependent Origination

Important: Please read the Disclaimer at the foot of this article

...

### Uncertainty (Anicca)

The "truth" that things change.

This is the "axiom of Buddhist Philosphy". The only thing take as "a given". Every other concept follows from this axiom.

### Ignorance (Avijja)

The belief that (some) things don't change.

### Formations (Sankhara) or "Things"

Things composed or formed of other things.

There can be no "things" without ignorance. A "thing" achieves its "thingness" from certainty. For a "thing" to be "a thing", that quality ("thingness") which make it "the thing" should remain unchanged.

At the same time, there can be no ignorance, without things. To believe in certainty, one has to believe in "the certainty of some thing". Without that thing, certainty has no meaning.

### Consciousness (Vinnana)

A flow of things believed to be unchanging, changing.

As long as the set of things believed to be constant stay constant, all things appear to be constant and fixed. However, the moment when (inevitably) something changes, all things appear to move from one state, to a new state. Creating a flow.

### Dependent Origination (Pratityasamutpada)

When two or more concepts depend on the existence of all others for their own existence. Where one cannot exist without all the others.

For example, things and ignorance dependently originate.

This is superficially similar, but different from the concept of "causality". When we say "A causes B" (e.g. The grandmother causes the grandson), the A many exist without B (as many women might not have grandsons). But when we say "A and B are dependently originated", A (or B) cannot exist without B (or A).

Also, in some sense, dependently originated concepts might be said to be logically equivalent.

### Dissatisfaction (Dukkha)

The feeling of unsatisfactoriness/disappointment/dissatisfaction, when things believed to be certain, turn out to be uncertain.

...

## Disclaimer

Many concepts of Buddhist Philosophy transcend language.

Hence, on the one hand, "language aides" (like notes, glossaries and dictionaries) are superfluous for proper understanding and "internalisation" of these concepts.

On the other hand, it is challenging to study most topics (Buddhist Philosophy included) without some books and some conversation. Both of which require language.

On the third hand, especially with Buddhist Philosophy, what one "understands" through language might be misleading. Or even blatantly wrong. Hence, language and language aides, like this set of notes, must be approached with caution. At best, they are vague sign-posts. And not destinations.

#### Article 264 · September 9, 2020

# Searching for "Sex" in Sri Lanka

### Using Google Trends

The Daily Mirror reported,

>>> "Ethiopia topped the list among the 10 nations that searched for the word ‘sex' the most on Google in the second quarter of 2020, whilst Sri Lanka was placed second."

The trend is not new. As the Daily Mirror said,

>>> "Sri Lanka topped the list in Google searches for the word ‘sex' for five consecutive years from 2012 to 2016."

Various commentators have interpreted these results in various ways. Some possibly flawed. In this article, I try to understand how Google Trends works and debunk some myths surrounding searching for "Sex" in Sri Lanka.

## Google Trends: A Brief Tutorial

Suppose you got to Google Trends, and search for the word "Sex" from "2004-Present" "Wordwide".

![Image](https://cdn-images-1.medium.com/max/800/1*n_quaI_qlTHFp63wnyCJBw.png)

You will see two graphs.

### Interest over Time

The first graph indicates the "Interest Over Time" for the search term. The "Interest" (on the Y-axis) is an a value from 0 to 100. The value is 100 at the point of time (X-axis) when the given search term (e.g. "sex") was at its highest in terms of the "percentage of searches".

![Image](https://cdn-images-1.medium.com/max/800/1*DXUMkqJ3O2KDNmW3WuF86g.png)

For "sex" this high point was in July 2017. Where we can see that the index was "100".

![Image](https://cdn-images-1.medium.com/max/800/1*QkgDl2I-W1TyLy5EWz0RJg.png)

The interest values for all other points of time are relative to this value. For example, currently (September 2020) the interest is 82. This means that currently the proportion of searches that search for sex is about 82% of what it was in July 2017.

![Image](https://cdn-images-1.medium.com/max/800/1*0h5y8_6lhpuulO_BvqhYzw.png)

Note, we don't know what this actual proportion is. We only know the proportion (say in September 2020) relative to the high point (July 2017). If 10% of searches in July 2017 were for "sex", then the proportion in September 2020 was about 8.2%.

Similarly, we also don't know the absolute number. We can't say that there were fewer searches for sex in September 2020 worldwide, because the total number of searches could have increased. For example, if the total number of searches in July 2017 was 10M (this is a guesstimate, I don't know the exact number), and assuming that 10% of searches were for sex, we have 1M searches for sex. If the number of total searches in September 2020 increased to 20M, then we have about 1.64M searches for sex in September 2020. Or more than July 2017.

### Interest by Region

The second graph indicates "Interest by Region". For the region you selected ("Worldwide"), you see the results broken down by sub-regions of that regions ("Country").

![Image](https://cdn-images-1.medium.com/max/800/1*Q89ZICed5SSb5dhjn69QMw.png)

Each country has an "Interest" value. Again ranging from 0 to 100. 100 is assigned to the Country with the highest proportion of searches for the search term. For "sex" this is Ethiopia.

Note, just as we did not know the exact proportion of "sex" searches" or the absolute number of "sex searches" in July 2017, we don't know the proportions or absolute numbers of "sex searches" for Ethiopia. All we know is that it has the highest proportion across the world. This proportion could be very large or very small. We just don't know.

Again, just as the "interest" values for other points of time (e.g. September 2020) were relative to the high point (July 2017), the "interest" values for other countries are relative to Ethiopia. For example, the proportion of web searches that are for "sex" in Sri Lanka, are about 91% of that of Ethiopia. So, if the proportion in Ethiopia is 10%, then Sri Lanka is 9.1%. If it is 0.1%, Sri Lanka is 0.91%. But we don't know what the proportions actually are. Nor do we know the absolute numbers.

Also, note, the above compares the highpoint of Ethiopia, to the highpoint of Sri Lanka. If we change the time window (say from "2004-present) to "last 12 months", the high-points change, and the results also change.

![Image](https://cdn-images-1.medium.com/max/800/1*H0E36Mu-GGlpfh-xuLjs6A.png)

### Search within Sri Lanka

Just as we searched world-wide, we can also search for trends within a country, like Sri Lanka.

![Image](https://cdn-images-1.medium.com/max/800/1*xqd_b9PlTGZsaSo1o_vbSg.png)

We intepret the results just as we did for "Worldwide".

![Image](https://cdn-images-1.medium.com/max/800/1*hSwGx3HIfTWCWQ2_mrNlOQ.png)

Similar to the world as a whole, the highpoint in time for searching for "sex" in Sri Lanka was July 2017.

In "Interest by subregion", just as "Worldwide" broke into countries, "Sri Lanka" is broken down into provinces.

![Image](https://cdn-images-1.medium.com/max/800/1*ielZh_kItn6oKlBhq7ctDg.png)

"North Central Province" has the highest proportion of "sex" searches. Followed by the "Northern Province" etc.

### Analysing Multiple Search Terms

Google Trends also supports searching for multiple search terms. For example, suppose you search for "Facebook", "Sex", "XXX" and "Porn".

![Image](https://cdn-images-1.medium.com/max/800/1*qynbF81Ng3rJKdADkeQPfg.png)

Similar to before, the "interest" value is 100 for the search term with the highest proportion at some point of time. This was in Aug 2013, for the search term "Facebook".

![Image](https://cdn-images-1.medium.com/max/800/1*A-ka6rkAbxjkCJmytAh38Q.png)

## Debunking Potential Myths

[Note: All the claims are assumed to be for the "last 12 months", unless otherwise indicated]

### 1. Sri Lanka has more searches for "sex" than any other country, except Ethiopia.

Google's "Interest" metric is proportional to the "proportion of searches" for "sex". Not the absolute number. If we want a compare countries by absolute number of searches, we should normalise the interest value, by the number of internet users (which I assume is proportional to the number of total Google Searches).

Once, we do this normalisation, we see that Sri Lanka drops from second place to 11th place. Hence, the claim is FALSE.

Matching our intuitions, the countries at the top have large populations.

![Image](https://cdn-images-1.medium.com/max/800/1*d_caQBBmS6PTp4zl9vSd5A.png)

11th is still quite high. Particularly given that Sri Lanka has the 64th largest internet user population. But that doen't make the "most searches" claim true.

### 2. 91% of Google Searches in Sri Lanka are for "sex"

If you read the Google Trends Tutorial, you'll understand why this is blatantly FALSE.

![Image](https://cdn-images-1.medium.com/max/800/1*H0E36Mu-GGlpfh-xuLjs6A.png)

### 3. Sri Lanka has a highest proportion of searches for "sex" than any other country, except Ethiopia.

The claim is superficially true. Google's "Interest" value is proportion to the proportion of searches for "sex". Hence, superficially, the claim is TRUE.

However, using the word "sex" as a indicator for "sex" is narrowly English-centric. Other languages have other words for sex.

![Image](https://cdn-images-1.medium.com/max/800/1*Rx2swzR8O7FTwhojcWYyfA.png)

Analyzing for "sex" excludes many countries. Including those that speak Spanish and Portugues (both translate as "sexo"), Russian ("секс"), and Chinese ("性別").

![Image](https://cdn-images-1.medium.com/max/800/1*kZLwxJ3lUaRAy9eFdQ4VkA.png)

Also, as you might have noticed, the Chinese word for "sex" does not appear on the map for China. This is because, Google Search is not used in Mainland China. The country with the most number of Internet Users. These users have other search engines, that they might use to search for "sex".

![Image](https://cdn-images-1.medium.com/max/800/1*6JRtpNj63wS9QKSDMdFsrQ.png)

There are also hints that searching for "sex" is correlated with a poor knowledge of the English language. For example, internet users looking for pornography in Native-English-Speaking countries, tend to search for "porn" — not "sex".

![Image](https://cdn-images-1.medium.com/max/800/1*pkvnGYxemFygmk6GvxCOzQ.png)

Hence, while Sri Lanka clearly has a high proportion of searches for "sex", concluding that Sri Lanka has the highest proportion is, at best, PROBLEMATIC.

### 4. "Sex" is the most searched for term in Sri Lanka.

To correctly answer this question using Google Trends, we would need to compare "sex" to every possible search term.

For example, if we compare "sex" to "Facebook", and "free", we see that until around 2009, "free" was the most popular term (not absolutely, but relative to "sex" and "Facebook"). Then, until about 2015 it was "Facebook". And since then "sex". It is true that, currently, "sex" is more searched for, than "Facebook" and "free". But that doesn't mean that there is no other word that is more popular.

![Image](https://cdn-images-1.medium.com/max/800/1*INWIENFVKCB7jumum6gHVA.png)

Hence, on ""Sex" is the most searched for term in Sri Lanka.", our conclusion should be DON'T KNOW.

## Concluding Thoughts

Regardless of what I've said above, Sri Lanka does have an abnormally high number of searches for sex. Why might that be?

One theory is that a disproportionate number of Sri Lankan internet users are young males. Who are the target audience of most pornagraphic sites. Who, for various cultural and social regions have restricted access to "offline" sex. And who have little education on sex in general, and "sex on the internet" in particular.

There is some (weak) evidence to support this.

For example, the interest in "sex" across Provinces in Sri Lanka, are (weakly) correlated with the proportion of the population aged 20–29.

![Image](https://cdn-images-1.medium.com/max/800/1*1_9JxfDep6plCzMO0CU3MA.png)

Note, this "evidence" is, at best, weak. And needs more analysis. It would have been useful if Google Trends broke down its "interest" values by age and gender. Sadly it doesn't.

...

PS: If you have any other claims/myths on this topic, which you'd like me to analyse, please comment.

#### Article 265 · September 11, 2020

### The Constitution of Sri Lanka

# Digitizing the Sri Lankan Constitution

### A Request for Comments & Feedback

There has been a lot of conversation and debate around the 19th and 20th amendments to the Sri Lankan constitution. I was keen to learn more — both about these amendments and the history of our constitution and amendments in general.

If you want to read our constitution, you can download a softcopy from the Parliament Website, which is what I did.

![Image](https://cdn-images-1.medium.com/max/800/1*dOXt7bOMgLfGb_DKfmosyA.png)

Unfortunately, the softcopy is a PDF. Technically"digitized" and good enough for a human to read. But not good enough for many other things.

For example, it is difficult to answer questions like the following:

* What articles amended in the "19th"?

* What articles were in the first 1978 draft of the constitution?

* What chapters have amended the most?

* What would a "diff" of the post-19th amendment version and the post-16th amendment version look like?

Hence, I thought of "translating" the constitution into a more "data processible" and analysis friendly form. This article describes my design. Comments and feedback are most welcome.

This Github Project project contains a draft version of the data. It has been generated through automated machine scraping and has errors that must be human-reviewed and corrected. It is solely meant as an illustrative example.

## The Design

### Versions of the Constitution

Each amended version of the constitution will have a folder (e.g. amendment_019 will contain the constitution after the 19th amendment).

![Image](https://cdn-images-1.medium.com/max/800/1*4sqzsGP9vBuwzcAJoyU7rQ.png)

A markdown file within each version foldler, will contain the version's preamble.

![Image](https://cdn-images-1.medium.com/max/800/1*bfpGWBG8rXW5tiish1tT6g.png)

### Chapters

A dedicated folder will store each chapter.

![Image](https://cdn-images-1.medium.com/max/800/1*rCndw4ozxDn1xqZ-JIrMJw.png)

### Articles

Within this chapter folder, each article will have a markdown file.

![Image](https://cdn-images-1.medium.com/max/800/1*cEJltTl_sN6AWHDlf1W9fg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*2ZVai4qSOQWDsKgvseCytw.png)

* The margin note will appear in italics at the top of the file.

* The numbered heading as the top-level header.

* The paragraphs, sub-paragraphs, sub-sub-paragraphs etc. as outlined numbered list entries.

```
*Languages of administration.*# 22.1. Sinhala and Tamil shall be the languages of administration through out Sri Lanka and Sinhala shall be the language of administration and be used for the maintenance of public records and the transaction of all business by public institutions of all the provinces of Sri Lanka other than the Northern and Eastern Provinces where Tamil shall be so used.Provided that the President may, having regard to the proportion which the Sinhala or Tamil linguistic minority population in any unit comprising a division of an Assistant Government Agent, bears to the total population of that area, direct that both Sinhala and Tamil or a language other than the language used as the language of administration in the province in which such area may be situated, be used as the language of administration for such area.2. In any area where Sinhala is used as the language of administration a person other than an official acting in his official capacity, shall be entitled:    a. to receive communications from, and to communicate and transact business with, any official in his official capacity, in either Tamil or English;    b. if the law recognizes his right to inspect or to obtain copies of or extracts from any official register, record, publication or other document, to obtain a copy of, or an extract from such register, record, publication or other document, or a translation thereof, as the case may be, in either Tamil or English;
```

#### Article 266 · September 11, 2020

Sanjiva, what you propose is what first occurred to me. And the CSist in me still wants to do this.

However, I was worried that a non-tech person might not be able to find a specific version by going through Git commit history. So I thought of a compromise where you start with 1978. Clone it and add amendment 1 as a diff. And so on. I thought having a separate file for each version might work better with non-techies.

A third approach might be to do what you propose, and just have the version files somewhere else for the non-technies.

Either way, given this early stage there's time to try one or all of these.

#### Article 267 · September 11, 2020

Yes. Schedules and Appendices should be added. + Various other meta data about amendments like dates. Will merge these in.

#### Article 268 · September 13, 2020

# King Devanampiyatissa's Number Theory

### A historical fiction

![Image](https://cdn-images-1.medium.com/max/800/1*4JNOFuxP9A1VXTqMa9wPiw.jpeg)

"How old are you, O King?", said the Arahat. "42 years, next full moon, Sir", replied the King.

"42", mused the Arahat. And then asked, "What sort of number is that?""It is an even integer, Sir", replied the King.

"And are there others besides that?""Sir, yes, Sir", said the King. "There are many, indeed an infinite number, of even integers".

"And besides those?", questioned the Arahat."There are odd intergers, Sir", said the King.

"And besides all these integers even and odd?""Well, Sir", said the King, "There are other rational numbers, that are not integers. Like 2/3. Which, incidentally, is the majority my PM has in Parliament, Sir"

"My namesake", said the Arahat, ruefully. "Yes. I've heard of that one. And besides?""My PM?...Oh, you mean rational numbers. Yes, there are other numbers, Sir".

"Such as?""Well, irrational numbers, Sir. Like the length in spans of the diagonal of a square, where each side is one span. That number is a little less than one and one-half spans. But cannot be expressed as a simple fraction. Indeed, I can prove it. A simple matter of contradiction..."

"Yes, yes", said the Arahat, hastily. "Don't let that fellow Pythogoras hear you. He might drown you as he did Hippasus."

"And besides all these, O King?", continued the Arahat. "Well, Sir", said the King. "There might be numbers that have not been invented as yet. The square root of a negative number, for instance."

"Yes, O King", said the Arahat. "I've also thought about those. But for brevity, and without any loss of generality, let's ignore these and leave them for some future discussion and, perhaps, generation. Any other numbers that have been invented?" "You mean, besides other even integers, odd integers, rational numbers and irrational numbers, Sir?", replied the King.

"Yes, O King", said the Arahat. "Why yes, Sir.", said the King. "There is 42, Sir. My age next full moon".

"Thou has shown great wit, O ruler of men!", said the Arahat. "Why, thank you, Sir!", said the King.

#### Article 269 · September 14, 2020

Haha, thanks!

#### Article 270 · October 3, 2020

### Geography of Sri Lanka

# Top 10 "Biggest" Rivers in Sri Lanka

### It depends on what "biggest" means...

Do you know what the Top 10 "Biggest" Rivers in Sri Lanka?

## 1D

We've all learnt that the Mahaweli Ganga is the longest river in Sri Lanka. Some of us might also know that the next longest is the Aruvi Aru (a.k.a. Malwathu Oya). Kala Oya comes next. Kelani Ganga and so on.

![Image](https://cdn-images-1.medium.com/max/800/1*KULARf6N02wUdDOnsdqZGA.png)

However this definition of "biggest" (i.e. "longest") is literally one-dimentional. There are more dimensions we can look at.

## 2D

If we rank rivers according to their catchment areas (i.e. the land area from where they get water), we get a different Top 10.

As in the 1D case, the length of the bars in the chart, are proportional to the length of the river. The area is proportional to the catchment area.

![Image](https://cdn-images-1.medium.com/max/800/1*t6if3RwKvlkiLH44I4kckw.png)

The Top 3 remain the same. Kalu Ganga (an unsually wide river with a dense system of branches) jumps from 10th to 4th place. Maha Oya leaves the Top 10, making way for Gal Oya.

## 3D

We can also look at the volume of water collected by the river. Or in other words, the volume of rain precipitated into the river. Leading to another Top 10.

As in the 1D case, the length of the bars in the chart, are proportional to the length of the river. As in the 2D case, the bottom area is proportional to the catchment area. The volume of the bar is proportional to the precipitation volume.

![Image](https://cdn-images-1.medium.com/max/800/1*hBh4hjkc4hvJMTrIfUCoog.png)

Wet zone rivers go up in the ranking, at the expense of Dry zone rivers. Mahaweli is still 1st. But Kalu and Walawe take 2nd and 3rd place.

...

Data and Code: https://observablehq.com/@nuuuwan/sl-rivers

#### Article 271 · October 6, 2020

### Covid19 Pandemic

# Are Sri Lankans Careful about CoViD19?

### A partial answer with the help of Facebook Mobility Data

Yesterday, I asked my twitter-sphere the following question:

![Image](https://cdn-images-1.medium.com/max/800/1*QnGMjW3G0uzt90pzrrjDsw.png)

I was surprised by this answer. I expected a "reduction" in alertness from September to October, given the relative calmness around CoViD cases.

Of course, this type of poll is, at best, a very rough estimate. At worst, it can bias by all sorts of factors.

Is there a better way to answer the alertness question? Perhaps, one with data?

## Mobility as Proxy for Carefulness

One proxy for "alertness" might be travel or mobility. If people are "more alert", they might be more likely to stay at home. Or restrict travel to short, essential trips.

But, how do we know if people stayed home?

## Facebook Data as a Proxy for Mobility

An interesting dataset that partially answers this question are the mobility data sets released by Facebook.

These datasets estimate the proportion of people who stayed within their region, based on Facebook use.

For Sri Lanka, an anonymised data set is available at a Divisional Secretariat Division (DSD) granularity. Here's an example DSD:

![Image](https://cdn-images-1.medium.com/max/800/1*ZiJXSFuljEH9hanZ_GCrSQ.png)

The Y-Axis records the % of people in the DSD (Colombo) who remained within an area approximately 600m by 600m. At "peak-lockdown" this was about 54% in the DSD. Before lockdown it was about 13%, and seems to have stabilzed at about 18% in September and October.

## Some Results

Here are mobility graphs for a selection of DSDs.

### Colombo and Suburbs

![Image](https://cdn-images-1.medium.com/max/800/1*ZiJXSFuljEH9hanZ_GCrSQ.png)

![Image](https://cdn-images-1.medium.com/max/800/1*e_E-CezZ_IQHfhYTPI3EIw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*D9jYth9OAXsituKx1wHdzw.png)

![Image](https://cdn-images-1.medium.com/max/800/1*iAhhIULdioW3GK5ijoMnxg.png)

There seems to be little difference between September 1st and October 1st. In fact, after lockdown eased, mobility increased only slightly.

There is a small uptick in immobilituy in October, and is probably due to the Minuwangoda outbreak. It would be interesting to monitor this trend.

### Galle, Kandy, and Jaffna

![Image](https://cdn-images-1.medium.com/max/800/1*D9JLwZBU7zxAYWqsNAhf_A.png)

![Image](https://cdn-images-1.medium.com/max/800/1*dUG_s16ylQlb2oDcVVMfWg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*z0QeR2CpIsr38KFRGVBOCA.png)

Except for a little more noise (possibly due to a smaller amount of data), Galle, Kandy, and Jaffna, are very similar to Colombo.

...

You can look at more data at https://observablehq.com/@nuuuwan/sl-lockdown-facebook-movement-data.

## Concluding Caveats

As I already said, Mobility is, at best, a partial signal for carefulness. Also, Facebook's estimates for location might not be completely accurate. Especially for sparsely populated areas. Hence, take these results with a pinch of salt.

#### Article 272 · October 8, 2020

### Transport in Sri Lanka

# Is the Colombo Light Rail worth it?

### A very "back-of-the-envelope analysis"

There's a lot of discussion and debate about the recently cancelled, Japanese funded, Colombo Light Rail (CLR) Project. Opponents say that "it is not cost-effective". Proponents have other thoughts.

![Image](https://cdn-images-1.medium.com/max/800/1*ytn1aHi6Zxl_FI4205c5ew.jpeg)

Who's right? To form an opinion of my own, I did some back-of-the-envelope calculations.

[See also https://medium.com/on-economics/road-metrics-aef58a17f097 for more details on metrics.]

## Latency and Speed

The first stage of the CLR spans 15 stations from Pettah to Malabe. A distance of about 15km. With a top speed of about 80km/h, the CLR promised to complete the entire length in about 30min (average speed 30km/h).

While it is possible to drive from Pettah to Malabe in about 30min in no traffic (e.g. at 2 am), at peak traffic, the journey can last three times that (90min). By bus, it can be 2 hours or more.

Hence, it is clear that the CLR would have been faster. Especially during peak traffic.

## Bandwidth

"Bandwidth" is a measure of the number of people travelling per unit time.

A CLR train has a maximum capacity of about 800 people. Assuming that 15 trains could have run per hour* (or one every 4 minutes), the CLR would have a bandwidth of 3.3 people per second.

A 10m long bus, with a maximum capacity of 60 people, with a bottleneck speed of 5km/h, has a bandwidth of about 8.3 people per second.

A sedan with five passengers has a bandwidth of about 1.4 people per second. However, even at peak-traffic most cars in Sri Lanka have about 2 passengers on average. Hence, bandwidth is about 0.6 people per second.

Hence, on bandwidth, busses are still more efficient than CLR.

[* I don't have the exact figure. Also, see discussion on Cost]

## Comfort

Like many private cars, the CLR will be Air Conditioned. But also like many busses, when at maximum capacity, many passengers might be standing and cramped together.

## Cost per Trip

For simplicity, I only look at upfront costs. I'd assume that upfront costs and ongoing costs are proportional.

The first stage of the CLR will cost about $2.2B or Rs. 407B. Spreading this across 25 years, and ignoring inflation/interest, this would be about Rs. 16B per year. Assuming an average of 250 working days per year*, that's Rs. 65M per day.

Assuming that the CLR runs for 8 hours per day**, at 15 trains per hour***, and 800 passenger trips per train, it completes about 96,000 Trips/Day. Hence, the CLR would (very roughly) cost Rs. 678 /Trip.

In comparison, a Rs. 10M Bus, with a 5-year lifespan, and 240 Trips/Day, would cost about Rs. 33 / Trip.

A private car, costing Rs. 6M, with a 5-year lifespan, with 4 trips per day (2 passengers, to and from work) would cost Rs. 1200/Trip.

If the same car were used as a Taxi, with 30 trips a day, that cost would drop to Rs.160/Trip. Carpooling would be somewhere in between.

[* Assuming 250 working days is equivalent to 365 working and weekend days combined]

[** The train would probably run for about 16 hours per day. I assume it is equivalent to 8 hours at maximum capacity]

[*** I don't know if the $2.2B estimate budgets for this many trains. It might be lower, in which case the CLR would be more expensive than I estimate.]

## Pollution

On the one hand, the CLR would be electric, and hence, compared to petrol cars and diesel buses, would have no urban pollution. On the other hand, Sri Lanka's electricity generation has increasingly depended on coal, the most polluting form of fuel.

Hence, all options pollute, but CLR and Busses probably pollute less per Trip.

## Summary and Concluding Thoughts

As I said, this is very much a "back-of-the-envelope" computation. Hence, season with the obligatory pinch of salt.

In summary, this is how cars, busses and the CLR compared across different dimensions.

![Image](https://cdn-images-1.medium.com/max/800/1*D5iQL5XJAt368HzSRPiQRg.png)

My (personal) conclusions are as follows:

* Pollution: No transport option will be environmentally ideal until Sri Lanka can move away from coal.

* Cost/Trip: Busses are the most cost-effective option. CLR and Cars are expensive.

* Comfort: The gap between Busses and Cars can be narrowed by having more ACed busses, and policies around crowding and safety, E.g. Female only busses.

* Bandwidth: Busses are best

* Latency and Speed: The only dimension where the CLR wins convincingly. However, I wonder what would happen if a significant proportion of traffic moves from cars and other private vehicles to busses? That might significantly reduce latency.

Overall, CLR is probably not worth it. The most low-hanging-fruit for Sri Lanka seems to lie in improving Bus Transport. Hence, I think what Sri Lanka needs is, not a Light Rail Plan (CLR or otherwise), but a Bus 2.0 Plan. We need to get people out of cars and into the busses.

#### Article 273 · October 8, 2020

### Transport

# Road Metrics

### From Latency to Bandwith

## Simple Road Segments

Consider a hypothetical segment of road. Suppose this segment is short enough that all the vehicles on it move at the same speed.

Suppose we wanted to "measure" the "state" of this road, using various metrics. What metrics might we care about?

### Distance and Speed

The most "well-known" metric about roads is probably distance. Or the length of the road segment. The other "well-known" metric is "speed". Or the distance travelled in a unit time.

For example, if some road segment is 100m, and it takes 10s for a vehicle to move from one end to the other, the "speed" on this segment is "10 meters per second" or 10m/s. Or in more familiar units, 36 km/h.

### Latency

We also care about how much time it takes to get from A to B. For the example road segment, this time or "latency" is 10s.

### Bandwidth and Density

The "bandwidth" of a road is the number of people that can travel through in a unit time. Bandwidth depends on both speed, and how densely people can pack into the vehicle travelling on that road.

For example, a large, 10m-long bus carrying 50 people, carries 5 people/m. A 5m-long sedan, carrying 5 people, carries only 1 person/m.

If the bus were travelling at 10m/s, its bandwidth would be 50 people/s. The sedan would have a bandwidth of 10 people/s.

The number of lanes on the road, also influence bandwidth. For example, if the road had two lanes, each with a bus travelling at 10m/s, its bandwidth would be 100 people/s.

## Complex Routes

In practice, road journeys happen on multiple road segments that form a complex road network. However, the metrics we care about are much the same.

How do the metrics for road segments, "aggregate" to form metrics for road networks?

### Distance and Latency

The Distance or Latency of a route is the sum of the distances or latencies of each of its component road segments.

For example, if a route consists of two segments, the first 100m long, and the second 200m long, and with latencies of 10s and 12.5s respectively, the aggregate distance is 300s, while the aggregate latency is 22.5 seconds.

### Speed

The speed of the route is the sum distance divided by sum latency.

In the previous example, each segment had speeds of 10m/s and 16m/s, respectively. The aggregate speed of the route is 300m / 22.5s or 13.33m/s.

### Maximum Bandwidth

The maximum bandwidth of a route is the bandwidth of the segment with the lowest bandwidth.

In our previous example, suppose the first segment was a single-lane road, while the second segment was a three-lane highway. Also, suppose that traffic on both segments was restricted to 10m-busses. The first would have a maximum bandwidth of 50 people/s, while the second would have a maximum bandwidth of 187.5 people/s.

Now the combined route would still have a maximum bandwidth of only 50 people/s, because it would not be possible to traffic more on the first segment, regardless of the extra capacity of the second.

![Image](https://cdn-images-1.medium.com/max/800/1*tAWPmys0DJxVFKMn38usSw.jpeg)

#### Article 274 · October 12, 2020

"A 10m long bus, with a maximum capacity of 60 people, with a bottleneck speed of 5km/h, has a bandwidth of about 8.3 people per second."

More details in https://medium.com/on-economics/road-metrics-aef58a17f097

#### Article 275 · October 12, 2020

# Happiness is a little bird

I gaze into the eyes of a little birdThat I hold gently in the palms of my hands.It is flightless, helpless...I smile at it, and I see my face smiling back through its tiny eyes.I am happy. And I am happier that its little face mirrors my happiness.

Afternoon, after afternoon we spendSupposedly in each other's companyEach hour passes with each smile...Each smile with each hour...The smiles are all mine. Little bird is beginning to flap its wings...I am happy. And am happier still for what I imagine are its little smiles...

Slowly it is evening. Dusk is golden brownDark creatures are returning home to nest.Oddly the cool winds of nostalgia feel strangely warm.I imagine that I am happy. Happier still, that I have let my little bird free.It has flown away.

Now it is night. The stars don't shine. For it is a night of clouds. A cloud of nights. Dreamless dreams full of masquerading imaginings. Imaginings of happiness. Happiness folded tightly in imagination. Now I am alone. Longing for warmth. Longing for a disconnection from reality.Longing to hold that little flightless bird in my hands again. Alas. Little bird has flown away.

...

Originally published on Facebook, April 2010

#### Article 276 · October 12, 2020

# London Sunrise

By the window. I,

As the mists of a winter morn caress the sun,

Contemplate silence.

Through the ear lids of a glass

A new day.

Now.

Born.

"Is grey a color? Worthy of such enchantment?",

The mistral teases.

O'er tiles and trees I smile at nature's incense.

"Oh, I am content."

Sipping rose hip tea.

Tasting the dancing sunlight.

By the window. I...

...

Originally published on Facebook, February 2018.

#### Article 277 · October 12, 2020

# Our War

War began not suddenly, but yet suddenlyIt was expected, yet it was unexpectedSickening and bringing out all the hate in the worldIt raged while it raged. But not afterFor as soon as it began it ended(An Anticlimax)I think we both wanted it (the war) to last — but it was not to beEven though we were poised...

Guns were all a ready to fire, ammunition loaded, crowds shouting for blood..But nothing really happenedA few fake skirmishes.That was all.Looking back, really nothing.

Nothing at all.

But then againIt was a sort of war, wasn't it?It did happen, didn't it?It must have. For...we still feel it, don't we?

I feel peacefulness now. Not peace, but peacefulness — void of peace.

How I sometimes long for war...Just so that we could do it all again.

...

Originally published on Facebook, March 2007

#### Article 278 · October 12, 2020

# Perfect Music

The scent on its shiny surface,Black and white(an enchanting, yet tranquil dress).Through the window,its polished lid reflectsrestful shades that sieve(like a breeze sifting moonlight)a serene mosaic. Calm. It is drizzling.Softly.Like a quiet friend leaving you alone.And yet- not.Piano. Not quite winter.Still, autumn has retired.New rain.Syrupy, soft.Music. Sprinkling through the elmand the oak,the hornbeam and the London plane,Nestling snugly in the crisp, scented leavesAnd then leaping softlyPattering drops on Turtle pondAnd the old castle This, I don't see through the windowOnly in my mind's.Part of my world.Like the warm comfort of a soft blanket on a November morning A green, gentleness across Fifth Avenue.It wraps me. The fall is shut(like the mouth of a sleeping black swan).But drops of music pitter-patter on my mind.Not quite jazz.Not Reverie.La prélude belle petite?NonBut still perfect. Wanting nothing moreJust perfect

...

Originally published on Facebook, January 2011

#### Article 279 · October 12, 2020

RE: "How come you didnt use the same math for the bandwidth of the train ? Say the train carries 800 people, 80 kmph and the train length is 100m. Then you get a bandwidth of 177 per second. "

CORRECT

...

RE: "And even logically a train moving 800 people at once at 80kmph, and a bus moving 60 people at 5kmph should have a lower bandwidth than the train. Confused !"

You are comparing one bus to one train. I'm comparing a system of busses to a system of trains. That's the difference.

The maximum bandwidth of a single train is much more than that of a system of trains.

#### Article 280 · October 12, 2020

# Random events around Colombo

Whiffs of water droplets, Splashing on leaves, Warmed by a mid-afternoon of sunshine, A grandfather tending plants in a quaint little garden,Adorned by shadows of dark green.A young couple amble into a Kottu place,

Greeted by its own percussive beacon,("A tempo" is my stride)An avocado-white vine with lavish verdures, It sashays up a jac-fruit tree,A sari draped across a sultry, sandalwood torso. Windows with sunburned, mahogany edges, Peeking out of whitened fences. Recently clipped grass, sumptuous and fragrant.A sea relaxing behind a craggy skyline.The crispy-sweet, scent of fresh hoppers.A sun (not quite set), Sleepy crows hovering across it.Ancient buildings serious, noble and dignified, Keeping guard, uninterrupted for 150 years,Witness more than just a few Random events around Colombo.

...

Originally published on Facebook, January 2014.

#### Article 281 · October 12, 2020

# Someone else

Is this you who I see? Or is it someone else? Or is it someone else that I saw in you?

Is this confusion? Or is it that I "was" confused? Confused that you were someone else, when you were still actually you?

Am I who I think I am? Or am I someone else? Or am I just not the one I thought I was?

Am I? For I see that you are still who you are But that you are still someone else.

I am someone else.

...

Originally published on Facebook, April 2007

#### Article 282 · October 12, 2020

# The Solutionist

And so the piper played his pipe,While all the rats did chase the tones,As people watched, the fruits were ripe,On trees that housed those swarms of dronesDid chase the tones, and end as bones...

And as the creatures headlong fellTo icy waters, currents coldThe men at work would dig the wellInto which the cat dropped, brave and boldCurrents cold and fears untold...

And so the solutionist posed his query,Answer this and you will know,The question is the one to bury,Ask it now. Unlike beforeYou will know,and so much more...

...

Originally published on Facebook, May 2010

#### Article 283 · October 13, 2020

# Drinking Water in Sri Lanka

### And the Reliance on Bowsers

Recently, a friend and I were discussing a charitable project to improve the quality of drinking water, in a remote part of Nothern Sri Lanka. The project involved building tube-wells. Without which people need to walk for miles, or rely on bowsers to collect water. The benefit of such projects is immense. They improve, not only the health, but entire economies.

However, one problem these projects face is "discovery". Namely, discovering who needs help.

I wondered if this "discovery problem" could be solved with data. Immediately, I thought of the 2012 Sri Lankan Census which asked a question on the Source of Drinking Water of Households. One question asked if the household's principle source of drinking water was bowsers. I wondered if "We depend on bowsers" would be a good proxy for "We need a better drinking water solution". And hence, if these households might be a good starting point for drinking water projects, including charitable ones.

Hence, in this article, I do a drill-down of households in various parts of the country depend on bowsers for drinking water.

## Data and Analysis

The Trincomalee district has the highest number of households using bowswers (4,425), followed by Puttallam(3,961) and Jaffna (3,142). As a proportion of households, bowsers are most prevalent in Mannar (11.6%), followed by Trincomalee (4.6%) and Kilinochchi (2.9%).

![Image](https://cdn-images-1.medium.com/max/800/1*_335gAGnDvDXllRRSEEbbQ.png)

Next, let's look at Trincomalee, Puttallam and Jaffna in more detail.

## Trincomalee

Most bowser use in Trincomalee is concentrated in the Kantale DSD (21.5% of Households) and the Mutur DSD.

![Image](https://cdn-images-1.medium.com/max/800/1*LMLztzHsGPCdFLwzW-yOYA.png)

Within Kanthale bowser usage is concentrated in the Jayanthipura, Wanela West, Wanela East and Pansalgodella GNDs.

![Image](https://cdn-images-1.medium.com/max/800/1*nUWpVvkBqema-gno8Bws7Q.png)

In Mutur, bowser usage is clustered around Muttur West, Jayanagar, and Periyapalam.

![Image](https://cdn-images-1.medium.com/max/800/1*GWlPmxVOuCf0ZGc8laZ8Yg.png)

## Puttalam

Most bowser use in Puttalam is concentrated in the Mundel DSD (14.2% of Households).

![Image](https://cdn-images-1.medium.com/max/800/1*ILlOb0gsDYisMP6wSfeQBw.png)

Within Mundel bowser usage is concentrated in the Andimunai, Udappuwa, Udappuwa and Pulichchakulama GNDs.

![Image](https://cdn-images-1.medium.com/max/800/1*lwRBqXOIzSy8kD2Ct5X4fg.png)

## Jaffna

Most bowser use in Jaffna is concentrated in the Karainagar DSD (39.8% of Households) and Island South (Velanai) DSD.

![Image](https://cdn-images-1.medium.com/max/800/1*A3b4Vwydi0La7mhLaVbFRQ.png)

Within Velanai bowser usage is concentrated on the Punkudutivu island.

![Image](https://cdn-images-1.medium.com/max/800/1*NPODTCph9cuAcTfaU1Cr8w.png)

Bowser usage seems to be evenly spread across Karainagar Island.

![Image](https://cdn-images-1.medium.com/max/800/1*LYdefAbCaudE6w4ce58t7A.png)

## Conclusions

In summary, let's look at the GNDs with the largest number of households that depend on bowsers. We missed some in the above analysis, because we did a top-down drill-down. Eluthur and Thalvupadu, which are in Mannar. Haragama is in Kandy District.

![Image](https://cdn-images-1.medium.com/max/800/1*efg-_C0KmQyq9FDunsRC3Q.png)

Also, there might be no "one-size fits all" solution that would work for all these GNDs. Some might need pipes, others wells. For still others bowsers might be the best solution.

Nevertheless, this list might be a good starting point. Further research should provide the details.

...

More Details can be found in https://observablehq.com/@nuuuwan/drinking-water-in-sri-lanka

#### Article 284 · October 14, 2020

### CoVid19 in Sri Lanka

# Spikes, Active Cases, Predictions and the Future

### Some approximate thoughts

## Spikes

Three spikes dominate the brief history of CoViD19 in Sri Lanka: The "Navy" spike in June. The spike associated with the Kandakadu Drug Rehabilitation Centre, and the latest spike associated with Brandix in Minuwangoda.

![Image](https://cdn-images-1.medium.com/max/800/1*Sqmgv5b1-wAywAPm27J2-A.png)

Each spike was about double the height of the previous. While this might be a coincidence, it is still worrying. Emotionally, if not rationally.

## Active Cases

While the spikes and the associated "total confirmed cases" have got a lot of media attention, the number that matters is the number of active cases. Our "ability to cope", in terms of hospital staff, beds and ventilators, depends on this latter statistics.

![Image](https://cdn-images-1.medium.com/max/800/1*zvQI51c3Md31IUOzbazGvQ.png)

Any spike in new confirmed cases causes a spike in the number of active cases. But as these people recover (or in a few cases die), the number of active cases drop.

## Predictions

The number of active cases at a point of time is the number of confirmed cases minus the number of recoveries and deaths.

The number of recoveries is relatively easy to predict since it seems to follow the number of confirmed cases 21 days ago, reasonably closely — matching our intuition that people recover in about three weeks.

![Image](https://cdn-images-1.medium.com/max/800/1*cLP3wvpNpQALSGBLbhx5AA.png)

The number of deaths from CoVid10 in Sri Lanka has been mercifully, so far, low compared to other countries. We could also reasonably assume that the "death rate" would stay reasonably stable. Hence, like the number of recovered cases, we could fairly accurately predict the number of deaths based on the recent history of confirmed cases.

The tricky variable is the number of new confirmed cases. This number is hard to predict in general, just as it is hard to predict spikes in particular.

## The Future

Any prediction for the future would depend on our ability to predict new confirmed cases — obviously, difficult. Hence, I'm not going to make any predictions. Instead, I'll make some observations based on a single, hypothetical scenario.

We've had about 100 cases per day, during the last three days (October 10, 11 and 12). There is no reason to assume that this trend will continue. But if we do assume that this trend continues for the next 100 days, the number of confirmed and active cases will be as follows:

![Image](https://cdn-images-1.medium.com/max/800/1*uhWpeoymW_INFC_GW4dJ5A.png)

At this rate, we would reach nearly 15,000 total confirmed cases in the next 100 days. But, as explained above, the more important metric is active cases.

The number of active cases would peak at around 3,500. Then active cases would "flatten out" at approximately 2100 cases. This is the number of new cases (100) time the days for each cases to recover (21). This computation is crucial because it gives us a sense of the relationship between active cases and new cases.

The latter calculation also gives us a sense of how many "new cases per day we could cope with". This number is the number of "active cases we could cope with" divided by 21. For example, if our maximum capacity for active cases was 2100, we cannot deal with more than 100 new cases per day.

However, before the "flattening out" there will be a peak of active cases. This is when our health care systems will be stressed the most. And what we should worry most about.

#### Article 285 · October 20, 2020

# Good Ideas for University Projects

### The Why and the How

![Image](https://cdn-images-1.medium.com/max/800/1*_lMv8kzGkUyV4z9ouzk3ng.jpeg)

Many university students ask me about university projects, especially on ideas and probable topics. This article is a summary of what I (usually) end-up telling them.

## Why University Projects

For most people, University Projects are a mere requirement. It's something they "have to do" to get their undergraduate or post-graduate degree. But there are many other reasons for doing University Projects and doing them well.

### Solving problems you care about

The two most common questions I get about ML and AI, are "What are the most important technologies?" and "What courses should I take?" My answer to both these questions is the same: "Forget about technology and courses to start with. Instead, find a problem that you care about. Then, see how you might apply technology or knowledge gained from courses to solve that problem".

University Projects are an excellent medium for solving problems that you care about. And beyond merely satisfying your course requirements, that's an excellent reason for completing a project.

### Building Visibility

If you are planning on pursuing "higher studies" beyond your bachelors or masters, your adviser would probably advise you to "publish a few papers" based on your university project. This is indeed a good reason, as often the project and any resulting papers will feature prominently in a post-graduate university application.

Beyond this academic visibility, projects are also a useful means of professional and industrial visibility. When I'm scanning through resumes to hire software engineers or data scientists, a good university project will boost the candidate to the top of my priority list. University projects carry a lot more weight than (say) high GPAs; they are far more relevant to the real-world.

### Converting into a bigger thing

Many real-world businesses have been born out of university projects. The most famous example is probably Google. Not only did Brin and Page become multi-billionaires, but so did several of their advisors at Stanford, and some of their batchmates.

A "bigger-thing" might not necessarily be monetary. For example, you could convert your university project into an open-source project. While it might not turn you into a Billionaire, it could still potentially benefit thousands or even millions people.

### Winning awards

There are many competitions for university projects, and the winners get a lot of publicity, monetary or other rewards, and often both.

## How to come up with good university project ideas?

The previous "Why" section meant to be a "generator" for this "How" section. Each "Why" serves as a mechanism to generate "Hows".

Ask yourself the following questions:

* What real-world problems do I care about? How might I "formulate it" as a university project?

* What are some interesting research papers? What are similar topics?

* What might be a potentially exciting business idea? Can a university project be a basis for testing such an idea?

* What are some interesting open-source projects related to my academic interests?

* What are some good competitions for university projects? What topics won in the past?

#### Article 286 · October 27, 2020

# Frustrations and Fears

### After the 2016 US Presidential Election

[Originally published on Facebook in November 2016]

I've lived in the US since 2007. As a non-citizen I've not had the opportunity to vote. However, I have been keenly following many political episodes, including the election of America's first "50% White+ 50% Black" President, and, more recently, its first, apparently, "Orange" one.

There are many aspects of engagement with US politics, which I've found frustrating and scary. Election 2016 has emphasized these frustrations and fears, and that's what this note is about.

## The Purplish States of America

![Image](https://cdn-images-1.medium.com/max/800/1*Xom8npB13rXu6057h-S3oA.jpeg)

The vast majority of my friends and acquaintances in the San Francisco Bay Area (where I live) identify as Democratic Party aligned Liberals (Blues). They've constantly and publicly identified with this alignment (e.g. #imwithher). Their social media communications highlight the positives of the Blue Team, and the negatives of the Red Team. They deal in certainties. Truths they hold to be self evident.

Republican Party aligned Conservatives seem exactly the same; with the exception of rooting for the Red team instead.

I've struggled to exclusively identify with a particular party. This is because, once I list all the issues, I agree with the Blue team on some, with the Red team on others, and neither on still others. On most issues, I'm more aligned with the Blues, but there are others which I'm more aligned with the Reds. In this sense, I'm neither Blue, nor Red, but Purple; even if its a Bluer shade of Purple.

Most of us are various shades of Purple. But why is it hard for us to say so openly? Why do we need to pretend we are the purest shade of Blue or Red? Democrats, please can you list Republican policies you agree more with? And Republicans vice versa?

## Jesus for President

![Image](https://cdn-images-1.medium.com/max/800/1*4eOwddxXC857SpPy6DLFrQ.jpeg)

When I have a strong one-sided opinion, I try very hard to force myself to argue the case for the other side. This is hard, and often I fail. But this is a good practice, because our natural biases get in the way of good judgement.

These last couple of months, I heard about everything that was wrong about the Red Candidate, from the Blue team, and everything that was wrong about the Blue Candidate, from the Read team. I wish this was the other way around.

I would have trusted the judgement of Ms. Clinton's supporters (especially those around me) a lot more, had they articulated Ms. Clinton's short-comings more clearly and openly. All political candidates must have some short-comings. When his/her supporters don't say what these are, I can only conclude that they are either ignorant, or they have something to hide.

The democratic process depends on people being informed and acting on that information. I, for one, had significant concerns about Ms. Clinton's suitability, both as a Presidential candidate, and as a President (I don't want to go into these, because that's not what this note is about). But among fellow Bluer shades of Purple, I was in the minority, when it came to being open about these concerns.

## Bigots casting stones at other Bigots

It is very hard for individual humans to hate other individual humans, once they get to know each other. The process of getting to know another person is the process of realizing that we are the same. On the other hand, it is very easy to hate labels: Mexicans, Muslims, Bigots, Misogynists, Homophobes, NRA-members etc etc, because it's easier not to identify with them; and it's easier to see the people cloaked in these labels as sub-human or inhuman.

I've been alarmed at the amount of political discourse which happens through labels. How many of us personally know a bigot? And if we think we do, have we ever sat down with the said bigot and tried to understand its views? Even if we conclude that the said bigot is seriously mentally disturbed and in need of therapy (or a lethal injection), can we extrapolate that large numbers of our fellow humans are exactly and uncontroversially the same?

A bigot is "a person who is intolerant toward those holding different opinions". There is often very little difference between a bigot and someone who casts stones at others calling them bigots. People, please look in the mirror.

Most people who voted for Mr. Trump are decent Americans. They are not bigots. For many of them the world has advanced and left them behind. They yearn for some past greatness, which an Orange faced, misogynist promises them. They did what they did because the rest of the world was too busy calling them bigots, rather that seeing their plight and helping them out.

![Image](https://cdn-images-1.medium.com/max/800/0*2_s7CQE5awTB0YxS)

## Conquer we must

I've grown to love the USA. It's been my home for most of the last 9 years. I feel for the US a lot of the matriotism I feel for Sri Lanka (my country of birth and citizenship). Ideas like "All men are created equal, that they are endowed by their Creator with certain unalienable Rights, that among these are Life, Liberty and the pursuit of Happiness" must be protected and promoted. But I genuinely fear for them.

I fear Blue Bigots as much as I fear that of Red ones. I fear personality cults of perfect leaders and perfect misleaders. I fear branding our fellow humans as inhuman. I fear all these things, but I'm most afraid that nothing will be done about them. We can't let nothing be done. Conquer we must, when our cause it is just.

![Image](https://cdn-images-1.medium.com/max/800/0*hw2igAYxKFSYWIh0)

#### Article 287 · October 27, 2020

Loosely related https://www.hpb.health.gov.lk/media/pdf/revised-timeline.pdf

#### Article 288 · October 27, 2020

The closest thing we have to a Central Website is https://www.hpb.health.gov.lk/en. It has quite a lot of useful information.

It might be useful to compare HPB to the "Ideal" and recommend what should be added to HPB (which might be easilly done).

#### Article 289 · October 27, 2020

https://www.hpb.health.gov.lk/media/pdf/revised-timeline.pdf

#### Article 290 · October 30, 2020

### Transport in Sri Lanka

# Bus 2.0

### What would it take to get me out of a car and into a bus?

I live not 2-minutes from one of the busiest bus routes in Colombo. Yet, I rarely travel by bus. A car (private or Taxi) is my usual mode of transport.

And there are many car-holics like me. As of 2018, for every bus in Sri Lanka, there were almost eight cars. The problem is that cars, compared to busses, are far less efficient at using road space. A Tata LP 913 has about 3.5x more seats per area than a Toyota Prius. This misuse of road space is one of the top reasons for traffic congestion in Sri Lanka in general and Colombo in particular.

What if we can convince these people (like me) to get out of cars and into busses? What if we could design a new bus system that these people would be happy to adopt?

In this article, I discuss a hypothetical bus system: Bus 2.0. The sort of system I'd be happy to use.

![Image](https://cdn-images-1.medium.com/max/800/1*BxKasbSzk5jTaaQ3_mUddw.png)

## Comfort

### Air Conditioning

The top reason I don't travel by bus is because of Air Conditioning. Or, more accurately, because of the lack of it. In a city with 90°F Temperatures and 90% Humidity, turning up to a meeting drenched in sweat is not an option. Hence, I revert to PickMe or Uber.

### Crowd Free

A seat or a comfortable standing space, without foreign elbows is a must have for me. Regulation around "maximum passenger limits" would enable this.

## Safety

### Harassment-free Busses

Busses in Sri Lanka are notorious for "Bus Perves", who physically and verbally abuse, especially female passengers, particularly at times when busses are crowded. Pickpockets and other thieves are also not uncommon.

Again "Maximum passenger limits" preventing over-crowding, would be a partial solution. Another might be to install security cameras on busses and use the footage to prosecute and shame miscreants.

### Bus Stops

Many passenger accidents occur when busses are picking-up or dropping-off passengers; often because busses don't stop at designated bus-stops, and instead stop (say) on the middle of the road. Or, even worse, not stop at all.

As before, mandating and enforcing regulations on basic safety will solve this problem. Even with no rules or enforcement, Bus 2.0 could use these safety guidelines as a mechanism to differentiate itself from Bus 1.0, and hence build a customer base and brand.

## "The App"

### Payments

People are far more likely to buy and use a product if they pay for it using cashless payment methods.

A "Bus 2.0 App" that would enable payments would be simple to build, especially given that most rider and drivers will own a smartphone.

### Tracking Stops

Beyond payments, a bus could easily provide other services. For example, it could warn the passenger that their destination is near, and alert the driver to stop; the modern version of the "bell" found on some busses.

## Joint Ventures

### Niche Transport & Tourism

In parallel to a "public transport" alternative, Bus 2.0 could also serve niches like office transport and school transport, by possibly going into joint-ventures with organizations or schools.

Another option is to use the system as a "Tourist Bus" system, particularly since many tourists sites around Colombo and its suburbs lie along existing bus routes.

### Ride-Sharing Apps

Existing ride-sharing networks like PickMe and Uber could add Bus 2.0. Just as you pick a Tuk or a car, you could choose a Bus.

## Advertising and Publicity

As with most products, a little marketing could go a long way.

Bus 2.0 could market itself as "an environmentally friendly alternative to cars", or "the most comfortable way to see Colombo" or "the safest way to travel" etc.

## Playing Devil's Advocate

### Cost

"But wait!" you ask. "Won't AC busses with security cameras and passenger limits be expensive?"

Pricewise, we are not competing with the fares of existing busses. A journey that costs Rs.50 by regular bus (let's call it Bus 1.0) might cost Rs. 1000 by car. Hence, a reasonable price for Bus 2.0 is probably in the range of Rs. 100 to 400 for this ride, and won't need to compete at Rs.50.

This differential would give some "breathing space" cost-wise.

### The Bus Mafia

"Sri Lanka's Bus 1.0 is controlled by a (relatively) small collection of politically well-connected businessmen. Won't they oppose Bus 2.0?"

At least at the beginning, Bus 2.0 would look like Tourist or Office Bus services, which already operate fairly independently. Hence, at least initially, Bus 2.0 would not compete with the interests of Bus 1.0.

### More for the Rich

"Why build another transport option for people who already have cars? Particularly when we could significantly improve Bus 1.0?"

True. Bus 1.0 is hardly optimal. However, solving the problems of Bus 1.0 and Bus 2.0 are neither mutually exclusive nor zero-sum. Also, unlike Bus 1.0, which might need a government subsidy, Bus 2.0 can be self-funded.

## Concluding Thoughts on Next Steps

So what happens next?

While Bus 2.0 might sound like "one grand plan", it is a collection of much smaller plans; implementable independently and in parallel. Anyone interested in one of the parts could start working on that part(as I might do myself) knowing that they are contributing to the whole.

Bus 2.0 could also be, not a system, but a "Standard" for building systems. The implementation left to individual transport providers.

#### Article 291 · November 16, 2020

# LRSM Programme Notes

I compiled these program notes as part of my Licentiate of the Royal Schools of Music, London in Performance (LRSM), which I obtained in 2003.

## J.S.Bach (1685–1750)

### Prelude and Fugue in C sharp major, №3 from ‘The Well Tempered Clavier', Book 1

Johann Sebastian Bach and his music form one of the most important chapters in musical history. Generations of composers have looked back to Bach's music in a search for that ideal that made his music "so right". His 48 preludes and fugues are stunning explorations into the individual character and colour of each chromatic key. They have influenced and shaped the styles of practically every great composer, from Beethoven to Chopin. The latter paid homage to Bach with his own 24 preludes.

The first book of ‘The Well Tempered Clavier' was completed around 1722, while Bach was musical director to Prince Leopold of Anhalt Cothen. Like his inventions the work was partly written for the instruction of his children (four of whom became eminent composers themselves). However, its principal intention was to exhibit the merits of the, then novel, tuning practice of equal temperament. Although early performances would almost certainly have been on the clavichord or harpsichord, the term "Clavier" did not refer to any explicit keyboard instrument. It is interesting how well the modern pianoforte (a "Clavier" Bach never heard himself) corresponds to the idiom of ‘The Well Tempered Clavier'.

The toccata like prelude is built upon a series of explorations through C sharp major. The opening phrase is a harmonic progression through the tonic key — rising and falling as if to feel it entirely. This is sequentially repeated in the dominant, the supertonic minor and the relative minor. If this opening section explores the harmonic qualities and relations of C sharp major, the next section scrutinizes the melodic and textural possibilities of a chromatic keyboard. The hands engage in a contrapuntal ‘question and answer' session while traversing the keys. In the final section, Bach revels in rhythmic complexity, balancing upon the black keys.

The fugue is in three voices, entering in descending order with the nimbly rhythmic subject. It is uniquely non-technical — it has no stretti, nor does it contain common fugal devices such as augmentation, diminution, inversion and pedal point. Bach relies solely on shape, form and some very original keyboard writing to create what is an amazingly lively, even dramatic piece. As in the prelude, Bach uses sequences to create movement and tension, especially in the episodes between the utterances of the subject. He also uses voices in Bradenburgian instrumental roles: a flute in the soprano, above a tenor cello, for example. Interestingly, the form of the fugue bares a surprising similarity to sonata form. The final section is almost a recapitulation of the exposition, while the unusually long episode that precedes it is uncannily developmental.

## Beethoven (1770–1827)

### Sonata in F minor (‘Appassionata'), Op. 57

Allegro assai Andante con moto Allegro ma non troppo

Ludwig van Beethoven's 32 piano sonatas epitomize a personal voyage, both musical and spiritual. They revolutionized pianoforte repertoire by demonstrating its orchestral power. They also reveal the boundless flexibility with which Beethoven expanded the sonata as a musical structure. Being highly representative of Beethoven's own turbulent character and existence, and spanning a period of 26 years, they symbolize, what is for many people, the autobiography of the greatest composer ever.

Op. 57, set in the dark key of F minor, grew out of the most tempestual episode of Beethoven's life. It depicts the violent inner struggle with which Beethoven confronted his crippling deafness and recall the many moments of utter despair that frustrated his epic search for inner peace. The sonata was published in 1807 (sketches date back as late as 1803) and was dedicated to Beethoven's friend and patron, Count Franz von Brunswick. The title ‘Appassionata' was the invention of the publisher Kranz, who later published a transcription of the original masterpiece for four-hands.

The first movement Allegro assai opens with a short characteristic theme based on the tonic triad. The doubling of the melody two octaves apart reveals Beethoven's almost prophetic insight into the sonorities of the piano. This also creates a sinister intensity that is only heightened by the innocuous trill and the silence that follows. The ‘quick- quick- quick — slow' motive that follows is strikingly similar to the immortal ‘fate' motive of Beethoven's Fifth Symphony (first performed an year after Op. 57 was published). The lyrical theme of the second subject beautifully extracts the piano's almost orchestral sonorities and idiomatically anticipates Beethoven's later melodic writing. Interestingly, this is based on an inversion of the sinister opening theme -forecasting the idée fixe of Berlioz and the leitmotiv of Wagner. Revolutionary as it may seem, Beethoven did use a similar device in his very first sonata (Op. 2 №1), coincidentally in the same F minor. The recapitulation begins with repeated quavers on the dominant below the opening theme, not unlike the opening of Schubert's song Erlking. Like Goethe's poem of the supernatural, upon which the song is based, the effect is indeed menacing. The over 50 bar long coda, is almost a second development. A dramatic rally of kaleidoscopic arpeggios lead to the Piu allegro section, that for the first time quotes the lyrical second subject theme in an agitated minor. Pressing syncopated chords follow in conclusion, before dying away suddenly. The first movement is the perfect example for the manner in which Beethoven fused drama into a classical form, while flawlessly preserving its almost Mozartian contour.

Sheltered between the two stormy Allegros is the Andante with its variations. It is highly spiritual and organic, rising from simple origins to plane heavenly proportions. The theme, a simple harmonic progression, set in a solemn, low register, conveys both harmonic and melodic overtones. It resembles soft wind instruments softly singing out a peacefully nocturnal air. The three variations induce a process of rhythmic division. The first variation contemplates in a simple walk like meditation, with the left hand following the right hand half a beat later. In the second, the left hand sings a cello like melody below peaceful semi-quaver broken chords in the right. The third variation cascades in demi-semi-quavers and builds to a divine high before leading to an echoing recollection of the theme, scattered between two registers. After almost dying away, the final Allegro ma non troppo is embarked upon, furiously.

Beginning with a succession of diminished sevenths and characterized by violent agitation throughout, the Allegro ma non troppo is arguably the most impassioned movement in the ‘Appassionata'. It is almost completely based on a single theme of a gyrating, cyclonic nature, and consequently pursues a single mood from start to finish. It is heard in various transforms: between melodic echoes, as a principal melody and in canonic counterpoint. The rising and falling nature of the storm manifests in scalic passages, sequential fragments and revolving octaves. The superhuman determination that was so distinctive of Beethoven's character manifests throughout, but particularly in the frenzied coda with its stubborn repetition and repetitive perfect cadences.

## Chopin (1810–1849)

### Etude in E major, Op.10 №3 Etude in G flat major (‘Black Keys'), Op.10 №5

To Frederic Chopin, the pianoforte was more than a musical instrument. A vehicle for expressing his most inner feelings and thoughts, it was as much an ear as it was a voice. Born into an age when the virtuoso was king and the piano his sword, Chopin succeeded in unifying virtuosity with individuality and poetism to an extent few have since emulated. Being principally technical works and yet perfect examples of the pianistic miniature that Chopin perfected so well, his 27 etudes are perhaps some of the best examples of this unity. Each emphasizes some particular aspect of pianoforte technique and are as innovative as they are instructive.

The 12 etudes of Op.10 were completed in 1833. Unlike many volumes of ‘finger exercises' that were abundantly available in Chopin's day, they belonged more to the concert hall than to the classroom. A more flamboyant composer such as Liszt would have certainly titled Op.10 as Etudes de concert (Concert Studies). Interestingly, the set was indeed dedicated to Franz Liszt, who described them as ‘Marvellous'. Chopin returned the compliment by wishing that he could execute them as Liszt did.

Finished in mid 1833, the Etude in E major was among the last etudes of Op.10 to be completed. Its opening section is a study of cantabile, legato and shape. Arch like and irregular in phrase structure, the bar by bar building of melody is narrative and adds to its story like lyricism. The opening theme was one of Chopin's personal favourites. He once confessed, "Never have I written a more beautiful melody.". On another occasion, when his pupil Gutman was studying it, the master is said to have clasped his hands and cried passionately, "O, my fatherland!". The more animated middle section is a study of sixths and trichords. It relies on texture and shape, rather than harmony for character. It is also surprisingly futuristic, even to the extent of foreseeing the dissonant colours of Wagner. It is also a reflection on Bach, with its long-range resolutions and dissonant counterpoint.

The Etude in G flat major, appropriately nicknamed the ‘Black Keys' or the ‘Black Note Etude', emphasizes balancing the right hand on the black keys. Completed around 1830, it was one of the first in the set to be completed. Like many of Chopin's bravura works, it possesses a novel flow, punctuated by the novel fingering technique that the composer pioneered, or at least revived. It personifies brilliance in every possible way — from its bouncing opening, right through to the pentatonic descent at the end. It is full of cross rhythms and dialogues evocative of the Italian opera that Chopin delighted in. The hands have individual and contrasting characters that help create the momentum and colour, characterized in the vivace marking. Like №3, many aspects of №5, especially its moto perpetua (perpetual movement) and harmonic style, seem to have been influenced by Bach's keyboard writing. Unlike №3, №5 was not one of Chopin's personal favourites. He thought it ‘The least interesting of the set..'. It is, however, one of his most popular works. Essentially as it is elegant, witty and as Von Bulow aptly described it, ‘A Salon Piece'.

## Ginastera (1916–1983)

### Danza del gaucho matrero from Danzas Argentinas

Inspired by nationalistic trends and his native Argentine folklore, Alberto Ginastera is arguably one of the true great nationalistic composers. The Danzas Argentinas composed in 1937, when the composer was 21, effectively communicates this. The three dances, Danza del viejo boyero, Danza de la moza donosa and Danza del gaucho matrero, set in the Argentine Pampas, depict the spirit of three pastoral characters: an oxen herder, a melancholy country maiden and a renegade cowboy, respectively.

Danza del gaucho matrero, like many of Ginastera's toccata like dances, is based on the Malambo, a rapid, energetic gaucho dance in compound-duple time. Its highly programmatic nature is characterized by some very colourful pianistic effects. For example, in the opening, Ginastera uses chromaticism and parallel effects to create a vivid picture of pounding hooves punctuated with metallic pulses. Soon after, he uses irregular chord clusters to mimic wild gunshots. He then depicts frenzied leaps with glissandos. Many aspects of gaucho dance manifest in the shape of percussive foot tapping and guitar effects. Ginastera's parallel major triad melodies also bear a striking resemblance to panpipe tunes that lay at the core of Amerindian music. (Coincidentally, gauchos were of mixed ancestry — European and native Amerindian)

Like many 20th Century composers, Ginastera was strongly influenced by many of the modern ‘isms' that characterized the music of the period. The serialistic sequences in, especially the dramatically climaxing sections, paint a vibrant picture of the violent surroundings of the gaucho matrero. Bitonality, expressionism and time signature changes, themselves once considered sacrilegious, enhance the rebellious nature of the dance. The extreme and sudden dynamics, not least the savage fortissississimo that concludes the dance, firmly imprint in the listener's mind the truly renegade spirit, that Ginastera wishes to portray.

#### Article 292 · November 16, 2020

### Politics in Sri Lanka

# The Sri Lanka Ghost Party 👻

### A Thought Experiment

Recently, I saw a 2020 Election Map of the US, with each state coloured by its winning presidential candidate, assuming that "I didn't vote" was also a candidate.

![Image](https://cdn-images-1.medium.com/max/800/1*1PSsa34--z57s54oz8UbjA.png)

This led me to ask the following question:

If "didn't vote + rejected votes" was a single political party (let's call it the "Sri Lanka Ghost Party"), how many seats would it have won at #GenElecSL2020 ?

In this article, I hope to answer this question, and also how many seats the Ghost Party would win in previous elections.

## 2020

Let's recall the actual result of the 2020 General Election. The SLPP won 145 seats; just shy of a ⅔ majority.

![Image](https://cdn-images-1.medium.com/max/800/1*gPiepH5MacWXJs-lOMIT8w.png)

The turnout in 2020 island-wide was ~76%. Of the 16,263,885 registered voters, 12,343,302 cast votes. In other words, 3,920,583 voters didn't cast their ballots. Of the votes cast, 744,373 or ~6% were rejected.

Now suppose we assign the 744,373 rejected votes and the 3,920,583 "I didn't vote"-votes, to an imaginary "Sri Lanka Ghost Party" (👻 or "GP"). How many seats would this party win?

![Image](https://cdn-images-1.medium.com/max/800/1*FGepiunS3RILUgoIdpOehg.png)

The Ghost Party would end up winning 67 seats or just under 30% of the seats in Parliament. The SLPP's vote tally would go down from 145 to 104; still a plurality, but no majority. The SJB's would drop from 54 to 41. Hence, the Ghost Party would have the second-highest number of seats in Parliament, next to the SLPP.

How would these results look like by Electoral District?

![Image](https://cdn-images-1.medium.com/max/800/1*oj5lHRXTqO8CUUVvzgIHig.png)

In five districts (Jaffna, Vanni, Batticaloa, Digamadulla, and Puttalam), the GP would have the highest number of seats.

Are 67 seats too high? Too low? How does it compare to history?

## 2015

While turnout and rejected votes in 2015 wasn't much different to 2020 (78%, 4.4%), there was a stronger and closer content between the two major parties. In this election, hence, the GP is in third place. It still wins a similar number of seats (65) to 2020.

![Image](https://cdn-images-1.medium.com/max/800/1*IW1G3-xzG4_X3x55qomM7A.png)

As we shall see, 2015 is an anomaly, in that it is the only General Election year where the Ghost Party is in third place.

## 2010 and 1989

Similar to 2020, the UPFA won a near ⅔ majority in 2010, with 144 seats. Unlike 2020, however, turnout was significantly lower (61% compared to 76%). Rejected votes were also higher at 7% (compared to 6%).

In our hypothetical scenario, the GP wins 111 seats, ahead of the UPFA (76 seats) and the UNP (32 seats). It wins first place in all districts, except Gampaha, Hambantota and Digamadulla.

![Image](https://cdn-images-1.medium.com/max/800/1*VWJsLhh5kXh_Pta51fNNCw.png)

This 111 seats is not unlike 1989, where the GP wins 96 seats. Like 2010, turnout was low (64%) and rejected votes (6%) similar. Unlike 2010, the UNP would win more districts in 1989 than the UPFA in 2010.

![Image](https://cdn-images-1.medium.com/max/800/1*6zNO7SBx1zcC7drgxDI-IQ.png)

## 2005, 2001 and 1994

In 2005, the Ghost Party would come second with 65 seats. Like 2020. Turnout was similar to 2020 at 76% and rejected votes around 5%.

![Image](https://cdn-images-1.medium.com/max/800/1*Wmz1Z5Pi4G_U7-zok9FzZQ.png)

2001 and 1994 would be similar.

![Image](https://cdn-images-1.medium.com/max/800/1*ZLzKpce2VeO5elwcXoFSbg.png)

![Image](https://cdn-images-1.medium.com/max/800/1*hO_VxO81vsBq98Jqa4gX1w.png)

[Apologies for not including 2000. I don't have accurate data in rejected votes.]

## Concluding Thoughts

The "Ghost Party" is not real, and the above "analysis" is a thought experiment. Nevertheless, is there something we can learn from this?

A few things:

* Given normal turnout (mid-to-high seventies percentage-wise), the Ghost Party would win about 65 seats. Similar to what it would win in 2020. A fairly "normal" pattern.

* Ghost Party seats are, in theory, up-for-grabs. Real political parties should think hard on how to win these, especially in districts where the Ghost Party seems strong.

* Sri Lanka has a comparatively high turnout compared to many other countries. Hence, "the hunt for Ghost Party's votes" might not be that easy.

* Of the last 7 General Elections (excluding 2000 — for which I'm missing some data), the Ghost Party came first in two(1989, 2010), second in four (1994, 2001, 2004, and 2020) and third in one (2015). When the Ghost Party comes second (which is the most common outcome), most of the "floating vote" either votes for the party coming first, or stays home (i.e. "votes" for the Ghost Party), implying that political parties should pay more attention to floating voters.

Happy Hunting! Or should I say, Haunting?

...

## Appendix: Code

You can find the code used to generate the above analysis and visualizations here: https://observablehq.com/@nuuuwan/if-rejected-votes-and-i-didnt-vote-were-a-party

#### Article 293 · November 23, 2020

# Three Stories about QA

### On Software Quality Assurance

## I

"Oh, we don't have to do any testing", replied the developer, almost smugly.

"QA does all our testing", his PM added helpfully. "Our rockstar developers just need to write code fast."

"Who designs the test plan for QA", I ask.

"I do", says the PM.

"Can't the developers write the test plan?" I ask.

"No", says the PM. "Tests plans have a lot of business logic and customer requirements. We don't bother developers with too many details."

"But isn't code full of business logic and customer requirements?", I ask.

"Yes", says the PM hesitantly. "But we spec-it-out so that developers can code it up easily."

I ask to see a test plan, and the PM shares a Word document with about 500 manual test workflows. I show a few workflows to the developer.

"Which part of the code are these tests testing?", I ask the developer.

"That's the Seller page. These code modules and functions."

"Can you open the seller page and test this workflow?"

I expected the developer to open the Seller page on his web-browser. Instead, he opens a terminal and runs a script. Before our eyes, and as if by magic, the script automatically tests the workflow.

"Why did you write the script?" I ask the developer.

"Oh, it makes it easy to test bugs", he replies.

"So you do write tests?", I ask.

"I don't have scripts for all the code", he replies. "Just a few."

"Would it be easy to write automatic tests for all your code?" I ask.

"In theory, yes", he replies.

"But not in practice?" I ask.

"No. That's QA's job".

"But what if you did write more of these test scripts?", I persist.

"Well, reflected the developer. "My code would be much cleaner. And we won't need to spend so much time back-and-forth with QA".

"But your PM would still have to write the plans, right?", I ask.

"Not really. If you understand the business logic well enough to write code, you can also write tests".

## II

"Why do QA engineers get paid less than Developers?" I ask. "After all, don't you all have the same university qualifications? Like degrees in Computer Science?"

"Actually", replied the senior QA engineer, "The pay here is quite good for QAs. We get paid a lot more than other companies."

"Why do you get paid more?" I ask.

"The hours can be tough", she replies. "Particularly during releases and deadlines. Sometimes we are up all night testing."

"Also", she adds doubtfully, "The work can be quite boring."

"Why", I ask.

"Running test after test after test. Manually" she explains. "It can be a pain".

"Could you do it differently?" I ask.

"Well", she replied, "there are a lot of bugs that are not in the test plan."

"How do you know?" I ask.

"Well, when you use the product for a long time like we do, you get a sense of where things might be wrong", says she.

"Do you report these to the PMs and developers?" I ask.

"Sometimes", she replies. "Though usually, we are so busy testing the test plan, there is no time".

"What if you had more time?"

"Yes — we'd test outside the test plan. It is more interesting and creative, and also more useful. Test plans are repetitive. Stupid actually."

"But why don't you have more time?" I ask.

"We don't have a lot of budget for QA. So we only budget for the time needed to finish the test plans."

"Why did you decide to become a QA?", I ask.

"Well — I interviewed for both QA and Developer roles. The interviewer said I'd be better for QA, so I become a QA."

"Ah ok. You probably messed-up the coding question?", I queried.

"There was no coding question. The PM and the CEO said they needed QA people, and I'd be good for the job."

## III

"When we were small, we didn't have a QA team. We shipped a lot of bugs, but since we didn't too many customers, it wasn't a big deal.

"Then we got bigger, and things changed. High-value customers expect more, especially from an enterprise product. Every enterprise product has QA, so we decided to build a QA team. As a sort of extra defensive layer".

"So, what does this defensive layer, defend you against?", I ask the CEO.

"Bugs, of course", he replies.

"Since developers write the bugs, QA defends the company against bad developers, right?"

"Sort of", replies the CEO doubtfully.

"I was looking at one of your manual test plans", I continue. "It looks automated tests can replace most of the manual tests."

"So, you want us to hire you to write the automated tests?", the CEO grins.

"Hardly", I reply

"Then who?", the CEO asks. "You know these consulting companies that design test plans are really expensive. We don't have that kind of money."

"Your own developers care perfectly, capable of writing automated test plans."

"Are they capable?" he asks.

"You don't think so?" I reply

"Well, won't the test plans have a lot of business logic and customer requirements?", he asks.

"Did you look at your test plans?" I ask.

"No — I leave that to my PMs", he replies.

"No", I reply. "‘business logic' and ‘customer requirements', as you put it, won't be a problem to your developers. The can write the automated tests."

"But then what happens to the QA team?, the CEO asks. "What do we do with them?"

"Well, some of them might be excellent developers", I reply.

"And we get rid of the others?", the CEO replies.

"No", I answer. "You're QA team could stay as it is, just fine. Maybe even grow a bit bigger".

"But", the CEO looks at me confused. "What would they do?"

"Well", I say, "They could do what you wanted them to do in the first place. Be your defensive layer."

"But what would they do? If the developers are already writing all the tests?" he asks.

"They could do their own testing. And also check on whether the developers are doing their job."

"But who will tell them what to test?"

"No one. QA already knows what to do. They can understand the code and read the manuals and figure things out."

"But will they catch new bugs?"

"Oh, yes. QA will catch stuff your PM never thought to put in his Test Plan."

"Interesting", replies the CEO, beginning to see some light.

"And they don't need to test only during product launch deadlines. QA can investigate the product all the time. And during normal hours. Without having to stay up all night when something is about to launch."

"And can we pay them less?", the CEO asks.

"You should pay them more.", I reply. "That is if you want this defensive layer to work."

"It is not working now", the CEO muses. For the first time, philosophically.

## Concluding Morals

* Automated QA: Much of what QA does now can and must be automated. Developers should be responsible for this.

* Creative QA: QA can move away from mechanical and boring QA (which automated tests can replace), to creative and interesting QA. QA will transform into a task that requires human intelligence, as opposed to brute-force labour.

* Asynchronous QA: In the old world, QA is the last link in the feature development chain. As a result, products can't ship without hectic, last-minute testing by QA. In the new world with Automated and Creative QA, QA can be parallel and asynchronous to development.

![Image](https://cdn-images-1.medium.com/max/800/1*RaB_WCXV3fOUMRpAqKri7g.jpeg)

#### Article 294 · November 29, 2020

### The Constitution of Sri Lanka

# The One Page Constitution

### A Thought Experiment

Most nations have constitutions that are hundreds of pages long. For example, the 2015 Revision of the Sri Lankan Constitution (up to and including the 19th amendment) contains 242 pages.

![Image](https://cdn-images-1.medium.com/max/800/1*bgxwVwMYzGLlceJVs7PXUA.png)

But what if we could write a constitution that fitted on a single page? One that could be read in a couple of minutes?

This article is a (possibly foolhardy and naive) attempt at such a "One Page Constitution" for Sri Lanka. I've erred on the side of being "novel and imaginative" and my "one-pager" has obvious weaknesses and gaps.

But then this is a thought experiment intended to be thought-provoking, while not necessarily practical.

...

## The Constitution of the Democratic Socialist Republic of Sri Lanka

### Article 1: Moderation of Power

* Bill Of Fundamental Rights, will ensure the most basic freedoms and rights of people (citizens and non-citizens) within the country, including freedom of speech, religion, press, and assembly, and freedom from cruel punishment etc.

* Legislature and "Representatives": Parliament will consist of a lower house and upper house, and will be responsible for only legislation, not execution. The Lower house, will be elected by the people, and will design and vote on laws. The Upper house, appointed by the lower house, with guaranteed membership for women, religious and ethnic minorities, and technocrats, will have veto power on all laws. Appointments to both houses are for four-year terms, and have a retirement age of 75.

* Judiciary: Nominated by Parliament, with a retirement age of 75.

* Executive: The posts of Executive President and Prime Minister are abolished. See Technocratic Executive below.

### Article 2: Stability of Laws

* Consistency: No law or its execution may contradict another law. Laws must be mutually consistent. E.g. No religion may trespass on a person's freedom of religion.

* Amendments: Amendment to this constitution would require the approval of 75% of both Lower and Upper houses.

### Article 3: Simplicity of Representation

* Lower house Representatives will be elected by First-past-the-post voting, from polling divisions ("Constituencies"), ensuring that each citizen knows exactly who their representative is.

* Local and Provisional Governments are abolished. The Lower House Representatives will also be responsible for local and provincial matters of their constituencies.

* Parliamentary Terms will begin on the first working day of January of years divisible by 4 (2000, 2004, 2008 etc.). Elections will be held on the first Saturday of December the previous year.

### Article 4: Efficiency of Execution

* Technocratic Executive: The executive will be headed and staffed by career technocrats. Parliament will pass legislation that determines budgets, policy, accountability and goals for the executive.

* Decentralization: Every service supplied by the State (Health, Education, Utilities, Transport, Police etc.), will be administered at the smallest practicable unit. E.g. Local Roads and Schools can be administered at the Constituency level; Coast Guard at the National Level.

* English will be the official language.

### Article 5: Identity of The Nation

* The Head of State will be a Non-Executive President, appointed by Parliament, embodying values considered most Sri Lankan, for life or until retirement.

* National Symbols (Anthems, Flags, Holidays) will amalgamate components from all identity groups. E.g. There won't be a Sinhala National Anthem or a Tamil National Anthem, but instead a Sri Lankan National Anthem, with both Sinhala and Tamil (as well as other) components.

#### Article 295 · December 1, 2020

### Startups in Sri Lanka

# Sri Lanka's Startup Ecosystem — 2020 December

### A Visualization

Can we visualise every Startup in Sri Lanka in a single picture? Read on to find out.

## The Data Source

Startup SL is a platform run by ICTA (Information and Communication Technology Agency of Sri Lanka) that claims to help startups to get access to accreditation, finance, partnerships and markets. It lists 335 startups, along with some interesting information about them, including category, funding stage and startup stage, along with the founders' contact details.

In this article, I visualize these startups in various ways, in an attempt to get a summary view of Sri Lanka's Startup Ecosystem.

### Important Caveats

* The listing on Startup SL might not be exhaustive. There are interesting and valuable startups, known to me, that are not listed here.

* Much of the information is self-reported by the startups. Some of it, particularly regarding funding, looks suspect.

## The Big Picture

In this "StartupScape", I group 335 startups by category (as reported on Startup SL). Each Startup assigns itself to up to three (out of 43 possible) categories. Hence some startups appear in multiple boxes.

![Image](https://cdn-images-1.medium.com/max/800/1*Xxtp49cUZ5wrL1UusX49aw.png)

This Big Picture is dominated by IT Products and Services, followed by E-Commerce, Mobile Apps, Education and Digital Marketing. This pattern continues as we look at finer cuts of startups.

## Startups by "Startup" Stage

### Ideation

Not all startups, even within the same category, are the same. The earliest startups consist of a set of founders (or sometimes even a single founder) brainstorming an idea. They believe that the idea might have potential. We call this the "Ideation" stage.

### Traction

Once the founders have had time to test their idea, and it gains some traction, the Startup enters the "Traction" stage.

If we exclude the 74 startups in "Ideation", our StartupScape (with 261 remaining startups) looks like this.

![Image](https://cdn-images-1.medium.com/max/800/1*CxlSAMYdAYJOiwcE4lNDyw.png)

### Break-Even

"Break-Even" is when a business total revenue is approximately equal to its costs. Hence, it makes neither profit nor loss — an important milestone for any startup because it proves that its net value is at least neutral.

Startup SL has 131 startups at Break-Even or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*AHQp7MxsqCVz10WlGIYSzA.png)

### Profit

Once revenues start exceeding costs, startups enter a "Profit" stage. Startup SL has 76 startups at Break-Even or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*av8lhmDRzRVkIj5UWyDfeQ.png)

[Note, this information is self-reported by the startups. I can't guarantee that these startups are profitable.]

### Scaling

Startups usually use the term "growing" to describe that they are trying to do what they are doing a bit better. Hence, growth is generally considered additive. "Scaling" on the other hand is multiplicative.

Startup SL has 37 startups at Scaling or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*R30GedZ5Yc95AOR2QGchBw.png)

### Steady

Finally, a startup reaches a "steady-state" where it more-or-less starts to do the same thing. By this stage, a startup is probably no-longer a startup. It is also debated if "stable" is a good state for any business, as it should be looking to innovate. Nevertheless, "Stable" is the final startup stage in Startup SL's classification.

Startup SL has eight startups at Stable.

![Image](https://cdn-images-1.medium.com/max/800/1*pCYSgiXvRawx22xif56bFw.png)

## Startups by Funding Stage

### Pre-Seed

Funding can be used to categorize a startup's evolution. Founders initially fund most startups, and possibly their close family, friends and other supporters. This type of funding is known as "Pre-seed" funding. Pre-seed funding is often unofficial, and some funders don't take a share of the companies equity.

### Seed

"Seed" funding is the first round of "official" funding, where the funders take an equity stake in the company.

Startup SL has 152 startups at Seed or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*DJYTKHoKZ31HDZuSTuLTlA.png)

### Angel

The term "Angel investor" or "Angel" refers to a professional investor who tends to invest in risky ventures like early stage startups.

Startup SL has 83 startups at Angel or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*SaWKteKUkn9r32XAHVGfNw.png)

### Series A

Startups seek "Series A" funding once they have proved their idea, gained some traction, and have a longer-term plan for profitability. However, this is an arbitrary definition — and we will see later if this holds for Startup SL's list.

Startup SL has 47 startups at Series A or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*tALT-n0EIYRLSCxgpeZeYg.png)

### Series B

In a "Series B", startups seek even more profitability and larger scale. In addition to the investment, investors often help Startup with expanding markets and new partnerships. Again, this definition is somewhat arbitrary. An alternative description of "Series B" could be "The round after Series A". In this way, there could be "Series C", "Series D", and even beyond (though Startup SL's classification ends with "B").

Startup SL has 22 startups at Series A or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*xJH4KBj-CGc_i68BvAO_3Q.png)

### Venture Capital

The term "Venture Capital" funding tends to overlap with all the post-pre-seed stages. However, it is usually different in that "Venture Capital" funding tends to come from Venture Capital firms, as opposed to individual investors.

Startup SL has 20 startups at Venture Capital or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*LPORauRIPNhRCS9x8TN4Xw.png)

### Mezzanine

Mezzanine financing usually consists of a combination of investments and loans and often precedes an Initial Public Offering. Often startups have specific projects they want to spend the funds on, often with the goal in optimizing their public offering value.

Startup SL has eight startups at Venture Capital or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*Zk7d_Zixo9HCjbUorz9wTQ.png)

### Initial Public Offering

At an Initial Public Offering, the Startup's shares are offered for sale in a Public Stock Market. And hence, it has access to funding from the public.

Startup SL has two startups at Venture Capital or beyond.

![Image](https://cdn-images-1.medium.com/max/800/1*yrbuWPMARv-Fyv6WZZjivw.png)

[Warning: See Caveats above!]

## Startup Stage vs Funding Stage

A startup's "Startup Stage" and "Funding Stage" are correlated. Here is a visualization of this correlation, for the startups on Startup SL.

![Image](https://cdn-images-1.medium.com/max/800/1*PgrulnQD7a8wxs38z4vuxg.png)

This might be clearer:

![Image](https://cdn-images-1.medium.com/max/800/1*zDTdNNujy2qFQD8G2ul2TQ.png)

Like most startup ecosystems, most startups listed on Startup SL are in the Ideation or Traction stage. Few get beyond this stage.

Also there is a (very) weak correlation positive between the startup stage and funding, with many outlyers and exceptions (though some might be self-reporting errors).

## Concluding Thoughts

Please heed the caveats. The underlying data seems approximate at best. However, with some improvements to data quality and coverage, analyses of this type are likely to be useful.

...

For data, code and high resolution images (SVGs), see https://observablehq.com/@nuuuwan/sri-lankan-startups

#### Article 296 · December 17, 2020

# Generalized Virtual Reality (GVR)

### On Reality. Virtual and Otherwise

![Image](https://cdn-images-1.medium.com/max/800/1*xprDzibUIwtU0m7ayNpAAQ.jpeg)

Present Virtual Reality (VR) systems like Facebook's Oculus, are limited and inaccurate; limited because they simulate only some of our senses, mostly sight and sound; inaccurate because these simulations are, at best, approximations. When we look through a VR headset, we know that we are looking through a VR headset. Because images are blotchy and sounds are artificial.

But what if we had "Generalized" VR?

By "Generalized" VR (GVR), I mean a VR system that was unlimited and accurate. Unlimited because it would simulate all our senses: sight, sound, smell, taste, touch, pressure etc. Accurate because it would affect a reality that was so real, that a human wouldn't be able to recognize that it was virtual.

Is GVR possible? And if so, what types of experiences could it credibly simulate? For example, could it simulate the experience a human (say me) walking about some space (say my house)?

If I were walking about my house, I would experience several things. I would see a changing landscape. As I pass a window, I would see the window passing. I would also experience different sounds. As I walk towards the window, the traffic outside would sound louder. If it was a sunny day, I might even feel the heat of the sun through the window. As I walk towards the kitchen, I would smell the aromas of lunch. And so on.

While we are probably years away from systems that can simulate all these experiences, it is still possible to imagine how we might get there.

But is this all that I experience?

There is one thing that I experience while walking around my house, which might be more difficult to simulate. It is the sense of "doing".

An accurate simulation of the sense would give me a realistic experience of being. For example, I'm "being" next to the window. But would a VR system give me the experience of "doing"? For instance, "doing" the act of walking towards the window?

Is it possible to "simulate" the "feeling of doing"?

Believers in "free will" might say "no". But Neuroscience is tending in the direction of a cautious "yes".

Evidence indicates that when I raise my foot, to walk towards the window, the feeling that "I must will my foot to rise" does not precede, but proceeds my foot rising. In other words, my foot rises first, and I post-rationalize the action that I "I willed my foot to rise", or "I raised my foot".

Hence, while I don't know exactly how, it might be possible to induce a sense of "free will" through some electro-chemical hacking of the brain.

All this leads to the much bigger "Matrix" question: Are we already in some GVR system? And if so or if not, how can we know for sure?

#### Article 297 · December 21, 2020

# On Vacations

### Confessions of a Work-from-home Chocoholic

August Holidays were particularly long, almost two months because classrooms at our school were taken-up for A. Level paper-marking. Like the shorter vacations in April and December, I loved the first few days of "The Holidays", where we could sleep till late, not worry about homework, and spend hours on things which we didn't have time for during term time.

Unlike April and December, I gradually used to get bored, and after about four weeks, I would often mope about the house racking my brains on what to do. However, this feeling of meaningless boredom soon ended, as the vacation, itself drew to a close. As the impending doom of early mornings and homework became more and more visible on the horizon, the vacation regained its privileged status.

Hence, despite the depression in the middle, the last week of an August vacation, was often the best time. Rather like the last teaspoons of chocolate mousse.

...

CoViD19 has turned vacations on its head. The idea of staying for a few days by the beach, or the mountains, or some other place away from home is fast becoming a distant dream. When I lived in London, a train ride or budget flight would land you in another country, one or two time zones away. Today, I console myself with documentaries and my notes on my travels.

For most of this year, I have worked from home with no physical contact with co-workers. All my meetings and other collaborations have been online. Hence, home is also work, and the line is increasingly blurred.

But I'm one of the lucky ones. Many work-from-homers have had to take pay cuts or lay-off co-workers. Still, others have lost their jobs. Still others never had the luxury of an office job and relied on the ability to leave home to work. For these souls, home is not a place of safety or rest, but the opposite; a sort of economic prison. Those who still have homes, that is...

...

I miss proper vacations, but I console myself that at some point they will be back; though in what form, only time will tell.

But I also try not to rely too much on the future. Some small adjustments can make the present a bit more bearable. For example, consider weekends.

I noticed that my weekends were getting blurred with weekdays. On weekdays I worked at home, and on weekends I was at home, and mostly worked. The sameness of the place created a sort of monotony of action. Hence, though I didn't have to work on a Sunday, I did because that was what I mostly did at the place where I was.

I've gradually weaned myself away from this. I don't work on weekends anymore, and instead, make time for more leisure and family activities. This "differentiation" makes weekends more like vacations, and the weekday more productive. And miraculously, despite the utter lack of proper vacations, I'm beginning to reap some of there benefits, like mental rest and refreshment.

I've been trying to lose a bit of weight, and have kept away from sweet desserts for a few weeks. But in the spirit of "making weekends more like vacations", I loosened this rule a bit. I recall last night and the last few mouthfuls of a chocolatey dessert that I love.

Vacations wouldn't be vacations without the lack of vacations. Pleasure necessarily depends on pain. Chocolate Mousse would not be Chocolate Mousse without no Chocolate Mousse.

![Image](https://cdn-images-1.medium.com/max/800/1*LH-YCjFcRjQumacxzDbk8Q.jpeg)

#### Article 298 · December 24, 2020

# What is the Capital of Brazil?

### And solving problems as athletes and spectators

"What is the Capital of Brazil?", a friend once asked me.

My immediate reaction was to say "Rio de Janeiro", and the cities enormous Christ statue atop a mountain visualized in my mind. But then, almost immediately, my brain said, "No. That's wrong."

Why did I think of Rio? Probably because a few hours before my friend asked the question, I'd been listening to some music, and happened to look-up the composer's name; he was born in Rio.

My next reaction was to say, "Sao Paolo". But again, my brain said, "No! Brazil is one of those countries, like Australia, where the capital is not the biggest city."

Finally, my brain said "Brasilia"; and, of course, that was the right answer.

Utterly unrelated to my friend's question, I felt a very subtle sense of disgust; and I soon realized why. I had been reading about how Brasilia, designed by Oscar Niemeyer, was a planned city, and hence had an "artificial"-ness which was, to many, ugly. For some reason, I had internalized this ugliness.

...

I have work to do this morning.

To be more exact, I have to design the architecture for a Machine Learning system.

"So, why are you wasting time thinking about Brazil?", you might ask.

Well, because "How do I design an ML architecture?" and "What is the Capital of Brazil?" have a couple of things in common. For one thing, they are both "problems", for which I have to (or had to) find "solutions".

As I had thought of Rio de Janeiro, Sao Paolo, and finally the artificial Brasilia, I don't remember spending mental energy at the time. My brain seemed to "flow" from one to the other, eventually reaching the solution. It was almost as if I watched my brain do the work; as if I was a spectator of a race, and my brain was the actual athlete.

In contrast, as I tried to solve the ML Architecture problem, I was trying to be the athlete; and was not making much progress, with no finish line in sight.

...

But what if I tried something different? What if I tried to solve the ML Architecture problem by being a spectator, and not trying to be the athlete?

And so I did.

Without trying to solve the problem, I let my brain wander. I thought of this and thought of that; concepts in ML, the business problems that the architecture was trying to solve, completely disconnected things like what I was going to have for breakfast.

And then, almost like a thunderbolt, my brain said something.

"Why am I trying to solve the ML architecture problem?" my brain asked me. "Is this the most important problem to solve? Is it not better to spend your time working on a different problem? Like what your ML strategy should be for 2021."

Not only did my brain ask me this question, but it also suggested some interesting answers. And so, I've decided not to worry about architecture, and think about the "bigger picture" for 2021.

...

In retrospect, I wonder if we ever "willingly" solve problems, or whether our brains or minds or other subconscious processes solve the problem, and we later take credit for them; rather like spectators claim (at least part of) the credit, when their athlete or team wins

I wonder if there is any significant problem that I or anyone has solved as an athlete, as opposed to as a spectator...

![Image](https://cdn-images-1.medium.com/max/800/1*Za-DMa_f7bfMk6q5jYMadA.png)

#### Article 299 · January 8, 2021

# How I consume Information

This article describes my playbook for consuming information. It is a "work in progress" is constantly evolving. Regardless, and as always, feedback is greatly appreciated!

## Push

By pushes, I mean information that is "pushed" by someone else, in realtime, towards me. With a push, information production and consumption happen at the same time. For example, a realtime phone conversation is an example of a push — where someone speaks to you, and you listen (roughly) simultaneously.

Pushes are disruptive, and so I try to keep it to a minimum. I have only one medium for push information: the Phone. By "phone" mean the old-fashioned sense of the word, where one person "phones" (verb) another person using a phone (noun); not the modern smartphone with its plethora of Apps. Hence, if someone wants me to respond "in realtime", they would have to phone me; no other medium would work.

Pushes have "sound notification" enabled; unlike pulls.

### Anytime Push

Only a very small number of phone numbers can ring me at anytime, even when my phone is "on silent". They include about a dozen phone numbers from close friends and family, a few related to work (e.g. On calls), and special numbers (e.g. Credit Card Fraud Alerts).

The people on Anytime Push know my schedule, when my phone is on silent, and know not to disturb me, except at the most urgent times.

### Limited-Time Push

All phone numbers that are not on Anytime Push mode (which is about 99% of my address book) are on Limited-Time Push mode. These people cannot reach me when my phone is on silent, which is:

* When I'm sleep

* During meetings

* Special occasions like events, holidays and vacations, when I'm not feeling well

## Pull

I like to keep Pushes to a minimum, and hence, consume most of my information via Pulls; where I "pull" information from the source, instead of having the source "push" the information towards me.

Unlike pushes, pulls don't have sound notifications. Hence, a device won't disturb me with a "beep" or a "ping".

### Anytime Pull

Anytime Pulls are where I allow myself to pull information at any time, at my discretion. These include non-muted messaging (e.g. SMS, WhatsApp, Facebook Messenger, Skype, LinkedIn Messages), and special notifications (e.g. Banks).

By "non-muted" I mean, conversations which I have not muted. Many messaging conversations are more like Email, in that they don't deserve instant attention and can easily wait several hours.

Anytime Pulls have visual notifications, like badges and popups, but like all Pulls, don't have sound notifications. Other Pulls (i.e pulls that are not Anytime Pulls) have no notifications.

### 4 Hour Pull

4 Hour Pulls include information I "pull" (roughly) every 4 hours; say at 8 am, 12 noon, 4 pm, and 8 pm daily. These include Email and muted-messagging.

### Daily Pull

Daily Pulls include information I consume daily. These include reading Books, Bookmarked News, News-Magazines, and other long-form sources.

I also "glance" at News about once daily, and bookmark long-form articles to be read later.

### Weekly Pull

Weekly Pulls include News and Social Media (Facebook, Twitter, LinkedIn feeds).

"News" also includes "paper" newspapers. While I subscribe to one daily "paper" newspaper, I only read them on Saturdays, in one big batch.

![Image](https://cdn-images-1.medium.com/max/800/1*jfEZQUhkhc6_4vyciMnMWQ.png)

#### Article 300 · January 12, 2021

### Machine Learning for Business

# How do you evaluate your Machine Learning Model?

### Good answers and bad answers

Suppose you use Machine Learning to solve some business problem in your organization. For example, you might run an e-commerce website, where you sell groceries; where customers log in, browse your stock, checkout what they want, pay for it, and then have the goods delivered to them. You (or one of your colleagues) might have built a machine learning model that "recommends" items for your customers, on the home-page of your website.

![Image](https://cdn-images-1.medium.com/max/800/1*WpwCuPLzdbbPlaRK5CXf7g.png)

Now, suppose I asked you,

>>> "How do you evaluate your Machine Learning Model?"

I.e. How do you know if it's good or bad? And if it can be improved? And if other people have better models? I ask this question often, and different people give very different answers: some good, many not so good.

This article is a "classification" of possible answers to the question "How do you evaluate your Machine Learning Model?": From really bad answers to very good ones. Read on to find out if yours is good or bad.

## ML0 — "I don't."

Sadly, the most common answer to "How do you evaluate your Machine Learning Model?" is:

>>> "I don't"

Few people know how well their Machine Learning Models work. Not everyone is this honest, though. Many people (especially on the "business side") say something elaborate, throwing in jargon, and buzzwords, and references to "technology". They might say something meaningless like:

>>> "We use the cutting edge HardMacro Turquoise AI Stack, and have a best-in-class e-commerce recommendation paradigm".

But it's fairly easy to see through the "BS", and that in reality, they have no idea.

This "ML0" is the lowest level in my classification, and if you think you fall into this group, I have two pieces of good news:

* Most organizations fall into this group. They've invested significant resources into Machine Learning or Data Analytics, but have no idea of the exact benefit it brings.

* This article explains how you can move up from "ML0" and improve your organization uses Machine Learning.

## ML1 — "Using Anecdotes"

Slightly better than having no idea is to have some idea. Many people have an anecdotal sense of their Machine Learning Systems; based on qualitative feedback from more knowledgeable colleagues or customers, like:

>>> "Our Chief Data Scientists said that the new model is much better than the old one"

Or a customer might say

>>> "Oh yes. I use the recommendations on your website all the time. It's very useful".

## ML2 — "Using Technical Metrics"

You might argue that it is "business people" who are guilty of ML0 and ML1. If you are a "technical person" (say a Machine Learning Engineer), you use all manner of fancy quantitative metrics to describe your ML.

For example, you might say that your e-commerce recommendation has:

>>> "A False Positive Rate (FPR) of only 60%"

In laymen's terms this usually means "The probability of a recommended item not being purchased by a customer". Similarly, "False Negative Rate (FNR)" means "the probability of not recommending a product that will be purchased by a customer".

On the one hand, having metrics like FPRs and FNRs (ML2) is better than having no idea on how the ML is doing (ML0), or only having a "qualitative" sense (ML1). On the other hand, it has at least three drawbacks:

* "Technical Metrics" like FPRs and FNRs (and more elaborate metrics like ROC curves etc.), have no clear "real-world" meaning. What would an FPR and FNR of 60% and 27.5% mean to the CEO? Would it be better than 70% and 15%?

* A comparison of Technical Metrics might not translate into Business Metrics. A model that is better than another model based on technical metrics is not necessarily better than the other model on business metrics.

* "Technical Metrics" isolate technical problems and people from the "bigger picture". For example, your e-commerce recommendation system could also be improved by better design, better photos, and different colours. These changes are not reflected in metrics like ROC, and hence cannot be compared to technical changes like ML improvements.

Organizations with ML teams that solely rely on Technical Metrics tend to isolate from the broader group working on the problem. "We care about what we measure" or more accurately "We don't care about what we don't measure."

## ML3 — "Using Business Metrics"

In the best ML organizations, even the most technical ML teams, measure themselves on Business Metrics, not Technical Metrics. For example, when I used to work on Ads Optimization at Facebook, we measured Models that recommend advertisements with metrics such as Revenue, Advertiser Profit, and User Feedback. No one ever mentioned FPRs or ROCs. These might be used operationally, (e.g. to "debug" faulty models), but never as a measure of model performance or quality.

Whenever a report or presentation on ML models, gives Technical Metrics priority over Business Metrics (ML2), it usually means one or both of the following:

* The technical team is unaware or unfamiliar with the actual business problem they are trying to solve.

* The technical team is trying to misguide or impress the audience by throwing technical metrics and other jargon.

## ML4 — "Using Business Metrics, across the Pipeline"

The best organizations not only use Business Metrics to evaluate ML Models and ML Teams but also use business metrics "operationally", at a "low level", say, when optimizing, tuning, and comparing different models.

For example, suppose you have several models for your e-commerce recommendation system: one is based on logistic regression, another based on boosting, another based on deep neural networks. You could either compare these models on "Technical Metrics" (like FPRs and ROCs) or you could try and compare these using Business Metrics, like Sales or Revenue. The Business Metrics would give you a more robust and accurate measure of which model is better.

## ML5 — "Using Multiple Business Metrics, across the Pipeline"

Most non-trivial, real-world problems cannot be measured or evaluated using a single metric (ML4).

For example, an e-commerce recommendation system, Revenue or Sales alone might not be sufficient. We might want to also look at measures like "Long term value of Customer", "Time to complete Checkout", and "Customer Feedback". If recommendations are for cheap, but low-quality products, we might see a short-term improvement in revenue, but a decline in long-term value.

Hence, we should evaluate ML Models (and all other parts of the system) on all the business metrics that the organization cares about, not just one. In practice, this might involve some tricky comparisons of "apples and oranges". But this is where humans judgement must take charge. The best Machine Learning systems are aides for smart humans, not replacements for dumb ones.

![Image](https://cdn-images-1.medium.com/max/800/1*W3yTIq2SJn9SfQxfxoeHJQ.png)