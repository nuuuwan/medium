### Artificial Intelligence: An Intuitive Approach

# Linear Search

### Chapter 1

Suppose you have a list of integers,

```
list = [64, 56, 3, 17, 8, 50, 49, 34, 49, 73]
```

Now, suppose you want to find the location (a.k.a. "index") of a particular value,

```
search_value = 3
```

## Algorithms

An obvious "strategy" would be to start at the beginning of the list, and check each item until you find the particular value.

```
def linear_search(list, search_value):    """Search for search_value in list."""    for i in range(0, len(list)):        if list[i] == search_value:            return i    return -1
```

[Note, if the search value is not found in the list, we return -1]

This simple algorithm, is known as linear search, because we pass through the list as if we were tracing an imaginary line through it.

How efficient is the algorithm? That depends on what we mean by efficient. Usually, we mean one of two things: 1) Time and 2) Space.

In general, a faster algorithm is a better algorithm. In the worst case, we would need to check every item in the list. In the best case, the first element of the list would be what we were looking for, and the algorithm, would be complete after a simple check. In the average case, we would need to check about half the elements in the list.

