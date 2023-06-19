---
date: 2023-04-22
type: note
tags: ankify
---

A class is essentially defining an abstract thing that otherwise cannot be represented in just a string, number, or boolean.

To do this, you need to create a new file, set a class for it, and use the `def __init__(self, *attributes*):` function.

```
Student.py
class Student:
	def __init__(self, major, GPA, smart):
		self.name = name
		self.major = major
		self.GPA = GPA
		self.smart = smart
```

Then in another file, you can call the student class to create an object.

```
main.py
from Student import Student
student1 = Student("Maxx", "Bioengineering", 4.00, True) # This is an object defined from the student class
student2 = Student("Max", "Biology", 3.00, False) # This is another object defined from the student class
print(student1.name)
print(student2.GPA)
```

You can also define object functions within the class that you can reference in another file.

```
Student.py
class Student:
	def __init__(self, major, GPA, smart):
		self.name = name
		self.major = major
		self.GPA = GPA
		self.smart = smart
def onHonorRoll(self):
	if self.GPA >= 3.5:
		return True
	else:
		return False
```

```
main.py
from Student import Student
student1 = Student("Maxx", "Bioengineering", 4.00, True) # This is an object defined from the student class
print(student1.onHonorRole())
```
