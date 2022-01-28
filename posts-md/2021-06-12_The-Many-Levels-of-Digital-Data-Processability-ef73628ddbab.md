#### Article 327 · June 12, 2021

# The Many Levels of Digital Data Processability

### From pixels to consistent structured information

Humans use computers to solve real-word problems. For example, I (a human) might use my laptop (a computer), to build a model that predicts the number of COVID19 cases in Sri Lanka in the next few weeks (a problem to solve).

In such situations, humans need to supply computers with data that might help find solutions. For example, statistics about COVID19 cases during the past few months (data) might result in a better prediction model (the solution).

By "Processability", I mean how easily a computer can process the data. The better the processability, the more efficient the processing, and the more efficiently the computer can arrive at a solution to the real-world problem.

In this article, I present a 6 levels of Digital Data Processability — from the least processable to the most processable.

## Level 1 — "Pixels"

Consider the latest COVID Press Release from the Department of Government Information (DGI).

![Image](https://cdn-images-1.medium.com/max/800/1*xr00gK7Z1GUCo3rFDTxmDQ.jpeg)

On the one hand, it contains some interesting (be they sombre) statistics about the COVID19 situation in Sri Lanka. It is reasonably well written, and easy for a human to process. On the other hand, it is shared as two JPEG files, one per page, on the DGI's website; very difficult for a computer to directly process.

Digital data in the form of images, where a computer is forced to process pixels, is the least processible form of accessible digital data. If a computer is to process this data, we need to resort to Object Recognition or Optical Character Recognition (OCR). Often these techniques are too expensive or tediious or both, and a human might need to manually convert the digital image into a more processable form.

Hence, Level 1.

## Level 0 — No Data

Before we continue, I must stress, bad data is better than no data. Hence, for completeness, let's call "no data" Level 0.

## Level 2 — Characters

What about PDFs? Is a PDF bextter than an image (like a JPEG)?

Only marginally. When text is presented in a PDF, the PDF file format defines locations to show each text character. For example, if "hello" is presented, the PDF will store the page coordinates of "h", "e", "l" etc. It doesn't explicitly say that "hello" is a word.

Hence, when a computer "sees" a PDF, it only sees characters. Isolated characters are not much of an improvement over isolated pixels. Not unsurprisingly, most data analysts consider PDFs a curse. But since they are marginal better than raw images, let's promote them to Level 2.

## Level 3 — Natural Language

Fortunately, there are ways of converting "lower-level" data into "higher-level" data. For example, I used the python package tesseract to perform OCR (Optical Character Recognition) on the JPEG press release . These days there are highly elaborate and effective OCR systems based on complete Machine Learning.

The OCR results looked like this:

```
Department of Government Information
```

```
12.06.2021Release No: 566/2021Time : 3:00Chief Editor / News EditorDirector (News) / News Manager
```

```
07 COVID deaths reported from 08 May to 31st May:55 COVID deaths reported from 01* June to 10 June:
```

```
No COVID deaths reported yesterday (11):
```

```
Death toll due to COVID 19 from 08 to 31 May 2021 as confirmed yesterday (11) by the DirectorGeneral of Health Services — 07,
```

```
Death toll due to COVID 19 from 01* June to 10 June as confirmed yesterday (11) by the DirectorGeneral of Health Services — 55
```

```
No COVID death was reported so far yesterday, June 11.
```

```
May 08 - 01 death
```

```
May 15 - 01 death
```

```
May 23 - 02 deathsMay 26 - 01 death...
```

[Complete output: https://github.com/nuuuwan/nopdf_data/blob/master/nopdf.dgigovlk.ref566.page001.txt]

Now, unlike the pixels of the JPEG, or the characters of the PDF, the computer has complete words, sentences and paragraphs. Level 3.

## Level 4 — Structured Information

While it is clear to a human what the Natural Language "Total number of COVID 19 deaths as confirmed so far yesterday (June 11th) — 2073" means, we need to help a computer make sense of this data.

To do this, we need to "parse" the data and extracts the nuggets of information that it contains. The "parsing" technique could be as simple as a set of rules, or a complex Machine Learning driven Natural Language Understanding model.

I built a simple rulel based parser that processes press-release text and generates structured information like this:

```
{  "ref_no": "566",  "unixtime": 1623447000,  "datetime": "2021-06-12 03:00",  "deaths_by_day": [    {      "unixtime": 1620412200,      "date": "2021-05-08",      "deaths": 1    },    {      "unixtime": 1621017000,      "date": "2021-05-15",      "deaths": 1    },    ...    {      "unixtime": 1623263400,      "date": "2021-06-10",      "deaths": 5    }  ],  "deaths_by_gender": [    {      "gender": "Female",      "deaths": 27    },    {      "gender": "Male",      "deaths": 35    }  ],  "deaths_by_age": [    {      "age_range": [        0,        20      ],      "deaths": 0    },    {      "age_range": [        20,        29      ],      "deaths": 0    },   ..    {      "age_range": [        99,        130      ],      "deaths": 0    }  ],  "deaths_py_place": [    {      "place": "In Residence ",      "deaths": 13    },    {      "place": "On admission to hospital ",      "deaths": 5    },    {      "place": "While being treated in hospital ",      "deaths": 44    }  ],  "areas_of_residence": [    "Alubomulla",    "Ambakote",    ...    "Waskaduwa"  ],  "causes_of_death_lines": [    "Acute kidney injury",    "Acute respiratory failure",   ...    "Stroke"  ]}
```

[Complete output: https://raw.githubusercontent.com/nuuuwan/nopdf_data/master/nopdf.dgigovlk.ref566.json. You can access the parser on GitHub. Feel free to fork it, or share feedback.]

Level 4.

## Level 5 — Consistent Structured Information

Level 4 is good enough for most data analytics tasks. But perfectionists could go one level further.

Consider the following section of another DGI COVID press release,

![Image](https://cdn-images-1.medium.com/max/800/1*RH1HKcGMFi8CA78OIj3ccw.png)

...and its corresponding Level 4 structured information:

```
...{      "district_name": "Monaragala",      "police_areas": [        {          "police_area_name": "Sewanagala",          "areas": [            {              "area": "Bahirawa"            },            {              "area": "Habarattawela"...
```

Do you see anything wrong?

The official spelling of Monaragala is actually, Moneragala. Consistent, structured information is structured data where such inconsistencies are removed.

On top of having standard spelling, consistent, structured information would also contain data like IDs in addition to names, which are more difficult to misspell. For example, the Moneragala District has ISO code "LK-82", and our Level 5 data would look like this:

```
...  {      "district_id": "LK-82",      "district_name": "Moneragala",      "police_areas": [        {          "police_area_name": "Sewanagala",          "areas": [            {              "gnd_id": "LK-8233045",              "gnd_name": "Bahirawa"            },            {              "gnd_id": "LK-8233070",              "gnd_name": "Habarattawela"            },            {...
```

[Complete output: https://github.com/nuuuwan/nopdf_data/blob/master/nopdf.dgigovlk.ref561.json]

You might argue that the Level 5 version of the press release is more difficult to process, at least for a human. While this might be true, it is trivial to render this into a more attractive format; even one much better than the original press release.

## Concluding Thoughts

Sadly, the DGI's COVID19 press release is representative of a lot of digital data online — both in Sri Lanka and abroad — shared by both public and private organizations. The vast majority consists of Level 1 (images) and Level 2 (PDF) data.

Even sadder, a lot of information which should be shared and accessible, is not (Level 0). For example, the vast proportion of Sri Lanka's public data (i.e. data that Sri Lankans have the right to access and use) is not accessible.

While many techniques transforming low-level data to high-level data (including those I describe), are effective and valuable, they are a waste in situations where high-level data can be shared in the first place. I hope owners of data realize this and are smarter in how they share data. I, for one, will be happy to help them achieve this goal.

![Image](https://cdn-images-1.medium.com/max/800/1*DhggRGMXoYRPsuMdqFwPSw.png)