---
date: 2023-04-03
type: note
tags: ankify
---

A list is a value that contains multiple values in an ordered sequence. Items are comma-delimited.

```
["item1", "item2", "item3"]
```

A variable can be set to a list.

```
variable = ["item1", "item2", "item3"]
```

You can access specific items within a list. The first item is always referred to as index 0. You can also use negative index numbers to start from the back.

```
variable = ["item1", "item2", "item3"]
variable[0] = "item1"
variable[-1] = "item3"
```

There can also be nested lists. Multiple indexes are required to access the values in the indexes.

```
variable = [["item1", "item2", "item3"], [10, 20, 30, 40]]
variable[0][0] = "item1"
variable[1][3] = 40
```

You can also obtain a list from another list as a slice. The initial value is included, but the final value is excluded from the list. You can also use a shortcut by omitting the initial or final value.

```
variable = ["item1", "item2", "item3"]
variable[1:3] = ["item2", "item3"]
vairable[:2] = ["item1", "item2"]
variable[1:] = ["item2", "item3"]
```

You can count the number of values in a list using `len()`

```
variable = ["item1", "item2", "item3"]
len(variable) = 3
```

You can also change the value within a list, or delete them using `del`

```
variable = ["item1", "item2", "item3"]

variable[1] = "replacement"
variable = ["item1", "replacement", "item3"]

variable[2] = variable[1]
variable = ["item1", "replacement", "replacement"]

del variable[2]
variable = ["item1", "replacement"]
```

List can also be concatenated and replicated

```
[1, 2, 3] + ["A", "B", "C"] = [1, 2, 3 "A", "B", "C"]
[1, 2, 3] * 3 = [1, 2, 3, 1, 2, 3, 1, 2, 3]
```

A value can be determined if it is in or not in a list using the `in` and `not in` operators.

```
'howdy' in ['hello', 'hi', 'howdy', 'heyas']
'howdy' in list1 = True
"cat" in list1 = False
```

There are numerous list methods as well.

```
list1 = ["cat", "dog", "moose", "cow"]
list1.insert(1, "chicken") = ["cat", "chicken", "dog", "moose", "cow"]
list1.append("bird") = ["cat", "chicken", "dog", "moose", "cow", "bird"]
list1.remove("dog") = ["cat", "chicken", "moose", "cow, "bird"]
list1.sort() = ["bird", "cat", "chicken", "cow", "moose"]
list1.sort(reverse=True) = ["moose", "cow", "chicken", "cat", "bird"]
list1.reverse() = ["bird", "cat", "chicken", "cow", "moose"]
```
