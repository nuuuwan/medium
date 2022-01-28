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