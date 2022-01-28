#### Article 350 · December 6, 2021

# Antifragile Algorithms

### Or Beyond Robust Programming

Most algorithms a Fragile. A few are Robust. This article is how we can do even better than Robust: How we can write Antifragile algorithms.

## Fragile, Robust, and Antifragile

In his classic book, Antifragile: Things That Gain from Disorder, Nassim Taleb differentiates between three types of things: the Fragile, the Robust, and the Antifragile.

Fragile things suffer from even small amounts of stress or noise. For example, you are likely to label a crate of crystal glasses as "Fragile" or "Handle with care" because even a small amount of mishandling (i.e. stress or noise) will break the glasses.

In contrast, if you were shipping packets of salt or bars of gold, you would not label their containers "Fragile". You're unlikely to label anything because mishandling or not, they are likely to remain unchanged and undamaged. We refer to this quality of remaining undamaged with stresses and noise as "Robustness".

You might say "Robustness" is the opposite of "Fragile". But this is like saying the opposite of "negative" is "zero", or the opposite of losing money is "not losing money".

The opposite of "negative" is "positive", and the opposite of "losing money" is gaining money. Similarly, the opposite of becoming damaged in the face of small stresses is improving in the face of small stresses. If you were transporting some good (I don't know what), which was Antifragile, you would mark the crate "Please handle carelessly".

Now, what if Algorithms could be Antifragile?

## Fragile Algorithms

Suppose you wanted to scrape a news article from the newspaper's website. Suppose you built a very simple scrape that identified the title of the article and the body of the article.

Suppose an h1 HTML tag always contained the title, a p HTML tag contained the body, and there was no other content with these tags.

```
<h1>Another Gas Explosion in Fartington City</h1><p>Our Fartington correspondent reports that yet another...</p>
```

To find the title and body, you need to find the h1 and p tags. If you used BeautifulSoup for parsing HTML, your code would look something like this:

```
soup = BeautifulSoup(html, ‘html.parser')article_title = soup.find(‘h1')article_body = soup.find(‘p')
```

This parser is simple, which is good. But it is also Fragile; a very small stress or noise will break or deteriorate it.

What is a small stress or noise in the Algorithms world? A small change that will break the algorithm. For example, what if the designer of the news site replaces the h1 tag of the title with a different tag?

```
<div class="div-article-heading">   Another Gas Explosion in Fartington City</div>
```

You might also confront this stress if you use the same algorithm to crawl a different news site.

## Robust Algorithms

A simple way of making your crawling algorithm more robust would be to look for different patterns of potential headings. For example, you could do something like,

```
title = soup.find(‘h1')if not title:    title = soup.find(‘div', class_='div-article-heading'):
```

You can make your algorithm even more robust by detecting the title in some more generic way. For example, you could detect the font size and weight of the various text types and determine that the "title" was the biggest and boldest.

As I hinted, this algorithm is more robust. The algorithm doesn't break or deteriorate with noise and stress (i.e. changes to the article format).

## Antifragile Algorithms

But what if we could do even better? What if our algorithm improved with noise and stress? What if there existed a news article parsing algorithm that got better as it parsed more and more various and different news sites?

Some might suggest a Supervised Learning Algorithm, where you input many examples of news websites, along with their titles and bodies. The algorithm would learn to parse the title and body and get better with more and more examples. In this sense, this Supervised Learning Algorithm is Antifragile.

However, Supervised Learning is, in a sense, cheating because you are "helping" it with training data, a benefit that our other algorithms didn't have. On the other hand, an Unsupervised Learning Algorithm could be both Antifragile and work without help.

Here's a very broad outline of what it might look like:

```
for many articles:    find various types of text found in that articlefor these various types of text:    exclude common text like links and other generic items    find "title-like" text    find "body-like" text
```

![Image](https://cdn-images-1.medium.com/max/800/1*ywt285wmOf3wPPJYvzp_pw.png)

## Concluding Generalizations

In many situations, designing Antifragile products or systems is difficult and counter-intuitive. However, in some situations (like News Article Crawling), we often write Fragile algorithms because it is easy, and because we don't think "Antifragile first". In general, we (programmers) should look for the Antifragile option first.