---
date: 2023-04-03
type: note
tags: ankify
---

Functions begin with a `define` statement and end with a colon on the first line. Parameters can also be specified within the parentheses in the `def` function.
The indents specify the actions acted upon by the function. Arguments can be used to be passed into the parameters.

```
def function1(argument):
	print("Function 1")
	print("Function 2" + argument)
```

Functions allow code to be repeated multiple times but only typed out once. This is beneficial in longer programs since there is less duplication of code, which in general reduces the number of code refactoring.
- ex For example, instead of adjusting your code in each instance you typed out a code, by using a function, you only need to adjust the function itself and it'll automatically update for every time you call the function elsewhere.
