#### Article 4 · April 1, 2018

# Classification Algorithms, Elections and Electoral Metaphors

### Including "What is democracy analogous to in the Machine Learning discourse?"

![Image](https://cdn-images-1.medium.com/max/800/1*oZEcwIj9LoNj-64W-satnQ.png)

A classification algorithm assigns some observation to some class of things. For example, given an email (the "observation") a spam detection algorithm could determined if it should be classified as spam or not-spam (the two "classes"). The algorithm will use various attributes of the email (e.g. who sent it, the text in it, what time it was sent etc) to determine which class it belongs to. These "attributes" are known as "features".

In elections, people vote to choose an individual to hold political office. The Electoral System determines how the aggregate votes are used to determine the winner. For example, the recent UK parliamentary election uses a "First-past-the-post" system, while Sri Lankan parliamentary elections use proportional representation.

Elections are analogous to Classification Algorithms. The observation is a single election. The features are the people voting. And the class selected by the algorithm, is the winner of the election.

Here is a list of some well know Classification Algorithms and Concepts, as "Electoral Metaphors". For readers familiar with Basic Machine Learning, I'll leave it as an amusing exercise for you to guess what these might be. If you're not, you could reflect on how Electoral systems have many things in common with Machine Learning algorithms — even when these commonalities might not be desirable.

* The election has exactly two candidates. Different people have different numbers of votes. People determined to be more likely to pick the "right" winner have more votes. "Right" means "likely to be successful based on past elections". Some people who are known to consistently pick the wrong candidate have "negative votes". Each person assigns all there votes for one of the candidates. Finally, all the votes are added up, and the candidate with the most votes wins. In some instances, one candidate might get some "bonus votes", if they are determined to be more suitable, irrespective of what the voters thing.

* The election can have two or more candidates. First, the person deemed most likely to pick the right winner votes. The election might end at this point, if "the system" is confident enough that the person got it right. If not, another person gets to vote. Exactly, which person gets to vote next might depend of how the previous person voted, and based on which next person is most likely to pick a winner "rightly". So, the order in which people vote might change depending how the people before them voted. This process continues until the system is sure of the candidate. As is evident, often not everyone gets to vote, as the election might be already decided before it's there turn to vote.

* In some systems, the number of people who get to vote in an election is artificially constrained to a small number. The assumption is that if too many people vote, the election will be made complicated by too many considerations and issues, and might not lead to the most "optimal" result (whatever that means).

* The election can have two or more candidates. The people don't initially select the final candidates, but select a set of proxy candidates, who will then vote on their behalf. These proxy candidates might then vote for the final candidates, or might, alternatively, vote for and select another set of proxy candidates. As with 1), both the initial voters and the proxy candidates might have unequal numbers of votes, which are determined according to who is most likely to pick the right candidates.

* The election can have two or more candidates. From all the people eligible to vote, a sub-group is selected at random, asked to vote, and the winning candidate for the sub-group is chosen. This process is repeated for many sub-groups. Each sub-group is then analysed for how well they might pick the "right" winner, and assigned a weight — with some subgroups having a higher weight than others. Finally, the winner is determined by the candidate who wins the most number of sub-groups, weighted by each subgroup's weight.

* In electoral systems where people are allowed to have unequal numbers of votes, we might want to restrict the amount of "unequalness". Because, if political power is too unequal, them the results of elections might be meaningless or even harmful. So sometimes we force each person to have at most only some number of votes over the mean number of votes per person.

* In some electoral systems, people don't vote for candidates, but vote for a list of political propositions — aligned with their political beliefs. Each of the candidates promise to carry out various political propositions. The winning candidate or candidates, are those whose political promises are most similar (or, as is referred to in the trade: "nearest") to those picked by the people.

* People don't vote. Instead, a subset of them are selected to be political candidates at random. The candidates then discuss their political opinions and form groups of like-minded people. The group with the largest number of people governs.

* Elections can get complicated when too many political issues are actively under discussion (security, immigration, taxes, education, healthcare etc). Hence, sometimes opinions on different issues are bucketed, into single groups. For example, if most people who favour higher taxes on the rich, also favour free universal healthcare, the two issues can be bucketed into "the High Tax and Free Healthcare" bucket. This process can be extended until the many issues and opinions, are minimised into a small set of lobby groups. Care is taken to ensure a manageable number of buckets.