#### Article 140 · October 19, 2019

# Command Line Analytics

### Analysing Election Results like a boss

Recently, I've written a couple of articles analysing Sri Lankan Presidential Elections, including: Election Projections, Bellwether Polling Divisions, On Floating Voters and A Brief History of Sri Lankan Presidential Elections.

All these analyses are based on data I scraped from the Election Commission Website. I have shared this data in JSON and CSV format on GitHub.

In this article, I share a couple simple commands you can use to answer some interesting questions about elections.

I use data from presidential_election_results.denorm.csv, which is a table of all the results in our seven Presidential Elections.

![Image](https://cdn-images-1.medium.com/max/800/1*I_mTLyr8tj5rs47jYTj0Cw.png)

## Basic Commands

To see all the data, run

```
cat presidential_election_results.denorm.csv
```

This will print out all the lines in the file:

```
year,result_code,electoral_district_name,polling_division_name,party,candidate,votes,percentage,affiliation
```

```
1982,01A,Colombo,Colombo North,UNP,Junius Richard Jayewardene,29380,69.03,green
```

```
1982,01A,Colombo,Colombo North,SLFP,Hector Kobbekaduwa,10641,25.0,blue
```

```
1982,01A,Colombo,Colombo North,JVP,Rohana Wijeweera,1645,3.86,red
```

```
1982,01A,Colombo,Colombo North,LSSP,Colvin Reginald de Silva,361,0.85,red
```

```
1982,01A,Colombo,Colombo North,ACTC,Kumar Ponnambalam,477,1.12,yellow
```

```
1982,01A,Colombo,Colombo North,NSSP,Vasudeva Nanayakkara,60,0.14,red
```

```
1988,01A,Colombo,Colombo North,UNP,Ranasinghe Premadasa,22389,63.26,green
```

```
1988,01A,Colombo,Colombo North,SLFP,Sirimavo Bandaranaike,10744,30.36,blue
```

```
1988,01A,Colombo,Colombo North,SLPP,Oswin Abeygunasekara,2259,6.38,purple
```

```
...
```

To see the field headings, you can run:

```
head -n 1 presidential_election_results.denorm.csv
```

Giving,

```
year,result_code,electoral_district_name,polling_division_name,party,candidate,votes,percentage,affiliation
```

To see the field headings and first line, run:

```
head -n 2 presidential_election_results.denorm.csv
```

```
year,result_code,electoral_district_name,polling_division_name,party,candidate,votes,percentage,affiliation
```

```
1982,01A,Colombo,Colombo North,UNP,Junius Richard Jayewardene,29380,69.03,green
```

This means that in 1982, Junius Richard Jayewardene of the UNP (green) got 29,380 votes (a percentge of 69.03%) in the Colombo North polling divisions, which is part of the Colombo electoral district, and has result code 01A.

You can format this output a bit better by replacing the commas with tabs:

```
head -n 2 presidential_election_results.denorm.csv | tr , ‘\t'
```

```
year result_code electoral_district_name polling_division_name party candidate votes percentage affiliation
```

```
1982 01A Colombo Colombo North UNP Junius Richard Jayewardene 29380 69.03 green
```

If you want to see only a few fiels, say 5) Party, 6) Candidate and 7) Votes:

```
head -n 2 presidential_election_results.denorm.csv | cut -d, -f5,6,7 | tr , '\t'
```

```
party candidate votes
```

```
UNP Junius Richard Jayewardene 29380
```

To see all the Colombo North Results for 1982:

```
cat  presidential_election_results.denorm.csv | grep 1982 | grep "Colombo North"  | cut -d, -f5,6,7 | tr , '\t'
```

```
UNP Junius Richard Jayewardene 29380
```

```
SLFP Hector Kobbekaduwa 10641
```

```
JVP Rohana Wijeweera 1645
```

```
LSSP Colvin Reginald de Silva 361
```

```
ACTC Kumar Ponnambalam 477
```

```
NSSP Vasudeva Nanayakkara 60
```

In descending order of votes:

```
cat  presidential_election_results.denorm.csv | grep 1982 | grep "Colombo North"  | sort -t, -nr -k7 | cut -d, -f5,6,7 | tr , '\t'
```

```
UNP Junius Richard Jayewardene 29380
```

```
SLFP Hector Kobbekaduwa 10641
```

```
JVP Rohana Wijeweera 1645
```

```
ACTC Kumar Ponnambalam 477
```

```
LSSP Colvin Reginald de Silva 361
```

```
NSSP Vasudeva Nanayakkara 60
```

To find how many candidates contested in Colombo North in 1982,

```
cat  presidential_election_results.denorm.csv | grep 1982 | grep "Colombo North"  | wc -l
```

```
6
```

Answer: six candidates.

See all the results for the SLFP in 1982, from polling divisions, excluding postal votes:

```
cat  presidential_election_results.denorm.csv | awk '!/Final Results|AICUM|Postal/' | grep 1982  | grep SLFP | cut -d, -f4,7,8 | tr , '\t' | sort
```

```
Agalawatta 21041 41.25
```

```
Akmeemana 19623 46.97
```

```
Akuressa 20389 40.57
```

```
Ambalangoda 16225 43.99
```

```
Ampara 20552 38.71
```

```
Anamaduwa 19757 45.71
```

```
Anuradhapura-East 14944 45.31
```

```
Anuradhapura-West 15054 42.19
```

```
Aranayake 10433 35.95
```

```
Attanagalla 31495 55.92
```

```
...
```

## Answering questions like a Nerd

### How many candidates have ever contested the presidential election? Who are they?

```
awk 'NR > 1' presidential_election_results.denorm.csv | cut -d, -f6 | sort | uniq | wc -l
```

```
64
```

Answer: 64

```
awk 'NR > 1' presidential_election_results.denorm.csv | cut -d, -f6 | sort | uniq
```

```
A. A. Suraweera
```

```
A. Dissanayaka
```

```
A. K. J. Arachchige
```

```
A. S. P. Liyanage
```

```
A. W. Premawardhana
```

```
Abdul Rasool
```

```
Aithurus Mohamed Illias
```

### Who are the Rajapaksa's who have contested the Presidential Election? Sirisenas? Sinhes?

```
awk 'NR > 1' presidential_election_results.denorm.csv | cut -d, -f6 | sort | uniq | grep Rajapaksa
```

```
Mahinda Rajapaksa
```

```
Namal Ajith Rajapaksa
```

```
awk 'NR > 1' presidential_election_results.denorm.csv | cut -d, -f6 | sort | uniq | grep Sirisena
```

```
Arachchige Rathnayaka Sirisena
```

```
Maithripala Sirisena
```

```
awk 'NR > 1' presidential_election_results.denorm.csv | cut -d, -f6 | sort | uniq | grep sin
```

```
Arthur Jayasena Ranasinghe
```

```
Hudson Samarasinghe
```

```
Rajiva Wijesinha
```

```
Ranasinghe Premadasa
```

```
Ranil Wickremesinghe
```

### What parties have contested presidential elections? Any with SL?

```
awk 'NR > 1' presidential_election_results.denorm.csv | cut -d, -f5 | sort | uniq
```

```
AACAAKO
```

```
ACAKO
```

```
ACTC
```

```
DNM
```

```
DUA
```

```
DUNF
```

```
FSP
```

```
awk 'NR > 1' presidential_election_results.denorm.csv | cut -d, -f5 | sort | uniq | grep SL
```

```
SLFP
```

```
SLLP
```

```
SLMP
```

```
SLNF
```

```
SLPF
```

```
SLPP
```

### What is the highest percentage of votes a candidate has won in a polling division? Who and when?

```
cut -d, -f1,4,6,7,8 presidential_election_results.denorm.csv | awk '!/Postal|Final/'  | sort -t, -nr -k5 | head -n 5 | tr , '\t'
```

```
2005 Kilinochchi Ranil Wickremesinghe 1 100.0
```

```
1994 Point Pedro Chandrika Kumaratunga 8 100.0
```

```
1994 Manipay Chandrika Kumaratunga 18 100.0
```

```
1994 Kayts Chandrika Kumaratunga 14761 97.16
```

```
2005 Paddiruppu Ranil Wickremesinghe 24142 94.72
```

Answer: Ranil Wickremesinghe won the only vote cast in Kilinochchi in 2005. As trivially, Chandrika Kumaratunga won all 8 and 18 votes cast in Point Pedro and Manipay respectively in 1994.

### Who won Borella in 2005?

```
grep Borella presidential_election_results.denorm.csv | grep 2005 | cut -d, -f5,6,7,8 | sort -t, -nr -k3 | tr , '\t'
```

```
UNP Ranil Wickremesinghe 25784 61.67
```

```
UPFA Mahinda Rajapaksa 15644 37.42
```

```
USP Siritunga Jayasuriya 115 0.28
```

```
ULPP Victor Hettigoda 80 0.19
```

```
JSP A. A. Suraweera 60 0.14
```

```
NLF Chamil Jayaneththi 32 0.08
```

```
SEP Wije Dias 23 0.06
```

```
ULF Anura De Silva 22 0.05
```

```
RPP Aruna de Soyza 18 0.04
```

```
SLNF Wimal Geeganage 17 0.04
```

```
DUA A. K. J. Arachchige 10 0.02
```

```
SLPF P. Nelson Perera 3 0.01
```

```
UNAF H. S. Dharmadwaja 1 0.0
```

Answer: Ranil Wickremesinghe with 61.67% of the vote.

### Who has historically won Attanagalla?

```
grep Attanagalla presidential_election_results.denorm.csv | sort -t, -nr -k8  | head -n 7 | sort | cut -f 1,5,6,7,8 -d, | tr , '\t'
```

```
1982 SLFP Hector Kobbekaduwa 31495 55.92
```

```
1988 SLFP Sirimavo Bandaranaike 35758 60.12
```

```
1994 PA Chandrika Kumaratunga 51923 73.64
```

```
1999 PA Chandrika Kumaratunga 51204 65.79
```

```
2005 UPFA Mahinda Rajapaksa 52393 60.52
```

```
2010 UPFA Mahinda Rajapaksa 61337 66.3
```

```
2015 UPFA Mahinda Rajapaksa 54777 51.71
```

### What is the highest number of votes a candidate has won in a polling division? Which year was that?

```
cat  presidential_election_results.denorm.csv | awk '!/Final Results|AICUM|Postal/' | sort -t, -nr -k 7 | head -n 5 | cut -d, -f1,4,6,7 | tr , '\t'
```

```
2015 Nuwara Eliya-Maskeliya Maithripala Sirisena 171578
```

```
2005 Nuwara Eliya-Maskeliya Ranil Wickremesinghe 156343
```

```
2010 Nuwara Eliya-Maskeliya Sarath Fonseka 112866
```

```
2015 Batticaloa Maithripala Sirisena 97779
```

```
1994 Nuwara Eliya-Maskeliya Chandrika Kumaratunga 94262
```

Answer: Maithripala Sirisena won 171,578 votes in Nuwara Eliya-Maskeliya in 2015

Please comment with your own interesting command-line analytics!

...

Caveat: For all the examples above, there are A) more efficient, B) more elegant, C) more correct, alternatives. For convenience, and laziness, I typed out whatever first came to mind 😉