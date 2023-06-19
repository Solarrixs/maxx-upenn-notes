---
date: 2023-04-15
type: note
tags: ankify
---

A dictionary is a *mutable* collection key-value pairs, typed with braces {}. Dictionaries are unordered in contrast to the [[list data type]].

`dictionary = {"size": "fat", "color": "gray", "disposition": "loud"}`
- size, color, disposition are keys
- fat, gray, loud are values

There are 4 methods for dictionaries:
1. `dictionary.keys()`
2. `dictionary.values()`
3. `dictionary.items()` - this will create a tuples of both keys and values of `("key", "value")`
4. `dictionary.get("key", 0)` - this will get the value of the key, and if the key doesn't exist, it will return the value 0

You can use multiple assignments to assign keys and values to separate variables:

```
for k, v in dictionary.items()
	print(v, k)
```
