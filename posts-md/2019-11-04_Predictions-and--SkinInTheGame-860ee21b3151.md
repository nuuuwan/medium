#### Article 156 · November 4, 2019

# Predictions and #SkinInTheGame

### Betting on the 2019 Sri Lankan Presidential Elections

There are millions of reasons to despise astrologers. But my personal favourite is that they face no downside if they make bogus predictions. They say whatever nonsense comes to mind and leave the poor client to face the music. As far as the charlatan is concerned it is heads you lose, tails he wins.

![Image](https://cdn-images-1.medium.com/max/800/1*oUVAPJ8HLmdGE6Ux134HAA.jpeg)

As Nasim Taleb would have put it, astrologers have absolutely no #SkinInTheGame.

Many astrologers have made predictions about the 2019 Sri Lankan Presidential Elections. And so have many Data Scientists: professional and amateur (like yours truly).

Unfortunately, too many Data Scientists have been making predictions based on suspect methodologies. But since they too, like astrologers, have no #SkinInTheGame, they have no incentive to do otherwise.

In this article, I describe a simple strategy to add #SkinInTheGame to predictions: All predictions must be accompanied by betting odds. You can't predict, if you also don't let everyone else (or at least your friends) bet on your odds.

## How to define odds

Recently, an astrologer turned data scientists (or data scientist turned astrologer — it is hard to tell the difference sometimes), sent me a lengthy analysis which concluded that Mr Rajapaksa would get 55% of the national vote, and Mr Premadasa 45%.

The "analysis" was utter garbage, but I thought I'd use it as an illustrative example.

Given the 55% probability for Purple, the odds in favour of Blue is 55/45, or 11/9. The odds are the "probability of winning" divided by the "probability of loosing". If Blue wins, and you bet Rs. 55, you win an additional Rs. 45.

Similarly, your odds for Green would be 45/55, or 9/11. If Green wins and you bet Rs.45, you win an additional Rs.55.

Punters would note that I make two assumptions:

* That the market is rational and efficient. I.e. that the market's notion of probability would be identical to the bookmakers.

* The bookmaker is "not-for-profit", and keeps no margin on bets. In the real world, bookmakers would have anything from a 5% to 50% margin on bets.

This is correct.

## So Nuwan, what odds are you giving?

The closest I came to giving probabilities for candidates was in A Machine's Opinion.

![Image](https://cdn-images-1.medium.com/max/800/1*y1DesBsC1XKpaZvUL_z4mw.png)

Green would probably get between 38.4% and 51.2% of the vote, and the Blues between 46.4% and 59.1%.

This is a bit different from the previous example because this is not single probabilities, but "Error Bounds" of probabilities. How might we translate these numbers into betting odds?

In each scenario, we would have to assume the worst case from the bookmaker's point-of-view. And as a result, define odds based on the best case probability for each candidate.

So, we would assume that Green had a 51.2% chance of winning, and Blue had a 59.1% chance of winning. Rounding up for good measure, the odds would be something like 14/13 for Green and 3/2 for Blue.

## But isn't this Illegal?

To be clear, I won't be making any "books" for the next election. And to be even clearer, 59.1% and 51.2% were not my opinions. Readers of A Machine's Opinion would know that it was my laptop's opinion. So if you have any questions on betting, talk to the machine, ‘cos the Human ‘ain't listening.

On the other hand, if you are a proper Data Scientist and you've offered odds, you have a "get out of jail free card": Error Bounds. Given the complexity and uncertainty around the election, any legitimate prediction should have huge Error Bounds. I'd say even broader than the 38.4% to 51.2% that I (ahem, I mean my laptop) came up with.

![Image](https://cdn-images-1.medium.com/max/800/1*IzmAOcujIfdaQUwSs5-76A.jpeg)

The good thing about error bars is that it will result in you (the bookmaker) making such huge profits that the bet will look nothing like a bet, and more like a donation. And as far as I know, there is no law against charitable donations to deserving Data Scientists.

The bad thing is, with such odds, no one in their right mind will bet.

The astrologers and bad Data Scientist, who don't understand error bounds, have no "get out of jail free card". Not only are they likely to lose money on bets, but the authorities are also likely to charge them with criminal behaviour. And about time.

Happy Punting!