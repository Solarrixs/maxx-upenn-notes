---
date: 2023-04-16
type: note
tags: ankify
---

Called using `import re`.

Input the regular expression within `re.compile(r"regular expression here")`.

Then use the `search()` and `group()` methods to find and extract the matching pattern from a text.
- You can also use the `.findall()` method to find all occurrences of the regex pattern.
- You can use the `.sub()` method to activate a search and replace function within regex
	- ex `namesRegex.sub("replace with this text", "search text here")`

```
import re
phoneNumRegex = re.compile(r"\d\d\d-\d\d\d-\d\d\d\d")
mo = phoneNumRegex.search("Text text text 123-123-1234")
print(mo.group())
```

## Character Classes
`\d` matches any digit.
`\D` matches any non-digit characters.
`\w` matches any word characters.
`\W` matches any non-word characters.
`\s` matches any space characters.
`\S` matches any non-space characters.
`[]` creates a custom character class. Adding a `^` makes it a negative character class.
- ex `(r"\[^aeiouAEIOUa-fA-F])`

`.` matches for any character (except a new line).
`.*` matches for any character 0 or more times. Basically an anything search. You can also use `.*?` to match anything in a non-greedy manner.

## Regex Syntax
`|` signifies an "or" regex module.
- ex `exampleRegex = re.compile(r"Bat(man|mobile|copter")

`()` marks groups within a regex, which can be specifically called upon using `mo.group(1) or mo.group(2)`.
`?` matches the preceding group for regex patterns 0 or 1 time.
`*` matches the preceding group for regex patterns 0 or more times.
`+` matches the preceding group for regex patterns 1 or more times.
`{}` matches the preceding group for regex patterns a specific number of times using `{1} or {2} or {110}`. You can also specify a range, such as `{1:3}` or {:3} or `{3:}`
- Putting a `?` after curly braces makes it do a nongreedy match, meaning it matches the shortest string possible.
`^` only accepts matches in the beginning of the string and `$` only accepts matches at the end of the string. Using both `^` and `$` in a regex syntax ensures that the format is contained in the entire string.
- ex `allDigitsRegex = re.compile(r"^\d+$")` will match for a string containing only digits such as `2398532985235230` but not `3894209a`.

Passing `re.DOTALL` (dot matches newlines as well) or `re.I` (ignore case) as an second argument to `re.compile()`, such as `re.compile(r"[aeiou]", re.I)`.
