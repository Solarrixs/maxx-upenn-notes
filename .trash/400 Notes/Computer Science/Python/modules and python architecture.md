---
date: 2023-03-23
type: note
tags: ankify
---

Python is designed to inherently make use of "modules". In my mind, modules are smaller code files that can be referenced with a larger "main" or "top-level" file (think master file) that executes lower level files.
- This defines the Python architecture: a main file composed of many module files linked by `import` statements.
- This is useful, since each file is a self-contained namespace, meaning variables can have the same name but will not return a name collision error.

Modules also hold attributes within them that can be referenced by upper-level files. The attribute can be accessed using the dot expression syntax: `object.attribute`.
- ex Within the `myfile.py` with a line containing `title = "The Meaning of Life"`, the title is an attribute. To access that data in another file called `main.py`, add a line containing the codes `import myfile | print(myfile.title)` (note that the pipe operator | signifies a line break).

Modules tend to hold many attributes, so the use of the `dir` function will fetch the list of attributes available within a module.
- ex `dir(myfile)`

Using the `exec(open("module.py").read())` function can also launch modules without having to import and reload constantly; however, this leads to potential silent overwrites of variables.
- ex If you define variable $x$, then use `exec(open("script1.py").read())` that contains a different value for the variable $x$, the variable defined in `script1.py` will be used.
