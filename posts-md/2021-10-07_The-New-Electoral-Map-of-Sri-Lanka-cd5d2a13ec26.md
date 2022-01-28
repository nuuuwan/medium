#### Article 340 · October 7, 2021

# The New Electoral Map of Sri Lanka

In How to Draw Sri Lanka's New Electoral Map, we discussed the workings of an Electoral Map Mapping Algorithm (EMMA).

As we saw, EMMA takes the Old Electoral Map of Sri Lanka as input. It modifies it step-by-step, gradually making it more and more optimal in terms of the five properties proposed in "5 Properties of Good Electoral Maps". Once "sufficiently optimal", EMMA outputs the New Electoral Map.

In this article, we will look at EMMA's output.

## Assumptions

Before we proceed, let's look at two assumptions that we've made.

### Electoral Map with 160 Polling Divisions each with one seat

EMMA generates an Electoral Map dividing Sri Lanka into 160 Polling Divisions, each with one seat. Since EMMA respects Electoral District (ED) boundaries, these 160 seats are first allocated amongst the 22 Electoral Districts.

![Image](https://cdn-images-1.medium.com/max/800/1*5SoytupXNB1idn3Hcf9PNA.png)

The seats allocated by EMMA to each ED differs from the 2020 (and other) Parliamentary Election Allocations because EMMA allocates only 160 seats to the EDs, while in Parliamentary Elections, 196 seats are allocated (of which 160 are allocated proportionally and 36 based on province, somewhat disproportionally).

### Population vs Registered Voters

EMMA allocates seats proportional to population, while in Parliamentary Elections, the 160 seats allocated proportionally are allocated in proportion to the number of registered voters.

EMMA uses population (from the 2012 census) because it needs population data at the Grama Niladhari Division (GND) level. As of now, we don't have access to registered voters at this level. Hence, EMMA cannot use registered voters for proportional allocation.

Compared to the Parliamentary Elections allocation, EMMA's allocation is likely to favour populations a smaller proportion of registered voters — i.e. those with younger populations.