#### Article 184 · December 9, 2019

# Burgher Beauties

### What Data Science says about Miss World

Caroline Jurie became the second Sri Lankan to win the Mrs. World Pageant; the first being Rosy Senanayake, who won the inaugural competition in 1984. With six, the United States has the most number of wins by country. Followed by Russia, Peru and Sri Lanka, which have two wins each.

Thisuri Wanniarachchi made an interesting (and somewhat contraversial) tweet about how an Euro-centric standard of beauty might disproportionately influence Miss World (and other beauty pageants). And, for this reason, the (apparent) increased likelihood of Sri Lankan Burgher women to perform well in such competitions.

>>> 

There seemed to be some truth to this claim. Afterall, both Jurie and Senanayake had Burgher heritage. But I was curious as to "how true" this was. Could we answer this question data scientifically?

Was a Data-Driven answer to the question, "What types of Sri Lankan women do well at international beauty pageants?"

## Last Names

One method would be to analyse the last names (surnames) of contestants. See who had Sinhala names, and Tamil names, and Moor or Malay names. And Burgher names.

But there was an obvious problem with this approach. We use a male-parent-centricnaming convention.

For example, I share my last name Senaratna (සේනාරත්න) with my father, but not with my mother. And with my paternal-grandfather, but not my other three grandparents. And with my father's father's father, but not my other seven great-grandparents. Even if all these ancestors with whom I don't share a name, were Burgher, I would not have a Burgher name.

Hence, last names were a dead-end.

## Background Research

We could interview the contestants or do some online research on them. And try to find more details about their ancestry. Possible, but expensive. And even if we do that, there is no guarantee of accurate data.

Another dead-end.

## Genetic Information

The perfect "source-of-truth" would be genetic information. If we analysed the DNA of each contestant, we could find out what their ancestry would have been like. Particularly who had European genes.

For example, according to 23andMe, my ancestry is 78.2% Sri Lankan, 6.2% North-East Indian, 3.6% Southern Indian, and 4.2% Central Asian. Hence, my genes were mostly South-Asian with a bit of Central Asian.

![Image](https://cdn-images-1.medium.com/max/800/1*29rqiLsO0vSWAG0Xv4NGaQ.png)

Unfortunately, I had neither the time nor the resources to ask every Miss/Mrs. Sri Lanka for a saliva sample. So that I could do some DNA analysis.

So, yet another dead-end.

## Faces

Then I thought, "What about Faces?"

Can we do some data analysis on pictures of beauty pageant contestants? And "see what they look like?"

And was there some unbiased way of doing this? There was!

What if we asked a Face Recognition system to cluster images using the same criteria as used to recognise faces?

That would work.

## Parenthesis: How Face Recognition Works

Before we address our question, let's see how Face Recognition works.

Let's start with a photo. Say, 2018 Miss Sri Lanka winner, Nadia Gyi.

![Image](https://cdn-images-1.medium.com/max/800/1*NbO5kTi0-KEusrYbLEMbKg.png)

The Face Recognition system starts with Face "Detection". I.e. find the portion of the photo that is "the face". Something like:

![Image](https://cdn-images-1.medium.com/max/800/1*qt5QEZXImaywU3ICOviZEw.png)

Next, the system detects various parts of the face. Like lips, chin, eyes, nose etc. It stores the coordinates of these parts.

```
[{'chin': [[81, 178], [81, 195], [84, 213], [93, 232], [102, 248], [113, 264], [125, 280], [137, 294], [154, 298], [175, 293], [198, 283], [221, 268], [241, 250], [254, 228], [260, 202], [259, 174], [257, 147]],
```

```
'left_eyebrow': [[76, 146], [82, 140], [91, 140], [102, 142], [112, 146]], 'right_eyebrow': [[139, 141], [155, 133], [172, 127], [191, 126], [210, 130]],
```

```
'nose_bridge': [[128, 165], [127, 179], [125, 194], [124, 208]],
```

```
'nose_tip': [[120, 219], [126, 222], [132, 223], [140, 220], [149, 217]],
```

```
'left_eye': [[91, 174], [96, 172], [105, 170], [116, 171], [106, 176], [97, 177]],
```

```
'right_eye': [[158, 165], [166, 162], [177, 161], [190, 160], [178, 166], [168, 167]],
```

```
'top_lip': [[120, 246], [123, 242], [130, 238], [136, 240], [141, 237], [157, 240], [176, 241], [170, 243], [143, 246], [137, 247], [132, 247], [124, 247]],
```

```
'bottom_lip': [[176, 241], [160, 255], [146, 261], [140, 262], [133, 261], [126, 256], [120, 246], [124, 247], [132, 247], [138, 248], [143, 247], [170, 243]]}]
```

Finally, the system converts these measurements into a "numerical signature" which is representative of the face.

```
[0.026797764003276825, 0.08502992987632751, 0.04182086139917374, -0.19603687524795532, -0.15643954277038574, -0.07881894707679749, -0.07458163797855377, -0.07068698108196259, 0.1689264476299286, -0.15674743056297302, 0.18560218811035156, -0.06397917866706848, -0.14878053963184357,...]
```

The signature consists of a list of numbers that represent various complex ratios of face parts which are deemed to be "most representative" of the particular face, based on millions of examples. Note, since these are ratios, putting on make-up or wearing a hat or glasses won't change the signature. Only complex plastic surgery could change the ratio of (say) the length of your nose to the width of your lips.

## Test Run

We can cluster beauty pageant contestant, by grouping candidates with similar "face signatures". But before we do actual clustering, let's test the system.

I took face photos of the. 2019 Miss Sri Lanka Dewmi Thathsarani, and 2018 Miss World winner Vanessa Ponce, and "asked" our Face Recognition system to cluster the images.

If it works properly, one cluster should only contain pictures of Thathsarani. The other only those of Ponce.

![Image](https://cdn-images-1.medium.com/max/800/1*9Obs1Tv5yq45W2lq1upnCg.png)

And it works! So far so good.

## Actual Run

I scraped the web for pics of Miss Sri Lanka and Miss World winners since 2000, and used my Face Recognition system into five groups.

(Note, I used Miss, instead of Mrs., because more face photos were available of the former online)

Let's see what the five clusters looked like.

### Cluster 1 — "Sri Lanka"

The first cluster consists of only Miss Sri Lanka winners (indicated by the red border).

Each cluster has some "Archetype Face" or "Mean Face" and candidates are sorted in order of the "difference" or distance from this face. The faces at the top are more similar to the cluster mean.

![Image](https://cdn-images-1.medium.com/max/800/1*jYAlYq_hfe4DIim8wkWW6Q.png)

(For clarity, I haven't displayed all the candidates in the cluster)

### Cluster 2 — "European"

The second cluster consists of only Miss World winners (indicated by the blue border) and is dominated by very "European" looking faces. Most of the candidates also have light hair.

Though our Face Recognition system, which is "colour blind" disregards colors, the "color" of a person is obvious correlated with face ratios.

![Image](https://cdn-images-1.medium.com/max/800/1*XUKPQGPD4DdHI3VuPZRI6A.png)

### Cluster 3 — "Asian"

The third cluster is dominated by South, Central and East Asian Miss World winners, and one Miss Sri Lanka (at some distance from the Cluster Mean).

![Image](https://cdn-images-1.medium.com/max/800/1*gg091rOGdLaRr5ZUtg6fhA.png)

### Cluster 4 — "International"

The fourth cluster has Miss Worlds from multiple continents. Who are surprisingly similar in some ways (e.g. Noses).

![Image](https://cdn-images-1.medium.com/max/800/1*x6L-BzW53BkxrG8VtL7XMw.png)

### Cluster 5 — Sri Lanka 2

The final cluster consists of only Miss Sri Lankas. Who differ somewhat from Cluster 1.

(A friend implied that Cluster 5 looks more Sri Lankan than Cluster 1. She might very well think that, but the data can't possibly comment.)

![Image](https://cdn-images-1.medium.com/max/800/1*n7kV4zvK2qS5ohHFjf_DEw.png)

## Bad News, and Good News

Since our system only compares faces and knows nothing of ancestry, we can't judge Thisuri's "Burgher Heritage" point.

However, we have to agree with Thisuri that a significant portion of Miss Worlds (Cluster 2) have very "Euro-Centric" features.

Still, the world seems to be changing. Asia, in particular, is rising. A lot of Miss Worlds are likely to be South, Central and East Asian in the future. Like Cluster 3.

Sadly, there is bad news for Sri Lanka. There was minimal similarity between the Miss Sri Lanka faces, and the Miss World faces. Note how little clusters 2, 3 and 4, overlapped with 1 and 5. For some reason, despite being clearly very beautiful, Miss Sri Lankas don't "look like" Miss Worlds. Since this applies to all Sri Lankans, this must also apply to Sri Lankan Burghers. If Mrs. World is anything like Miss World, the Jurie and Senanayaka wins seem to be Black Swans.

Overall, one characteristic that all the clusters seem to have is some "sameness". Everyone seems to look the "same" in many ways, which implies that beauty pageants might be converging to some (if not necessarily European) narrow standard of beauty.

Hence, I tend to agree with Thisuri's final point. Why do women have to get up on stage and be judged? On some narrow set of standards? There are better things to do.

For example, Sri Lanka has a severe shortage of Computer Scientists and Data Scientists. And an even more severe shortage of female CSs and DSs. Why not adopt one of these professions? Using fancy Face Recognition to cluster the faces of beauties might be almost as fun as being one.