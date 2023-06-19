---
date: 2023-04-22
type: note
tags: ankify
---

If you have multiple objects with in a master to slave relationship, and you want the slaves to inherit all the attributes of the master, you can simply inherit those attributes instead of manually copying each one into the slave.py file.

```
class Chef:
	def Chicken(self):
		print("The chef makes chicken.")
```

```
from Chef import Chef
class ChineseChef:
	def Rice(self):
		print("The chef makes rice.")
```

```
main.py
from Chef import Chef
from ChineseChef import ChineseChef

Chef1 = Chef()
Chef2 = ChineseChef()

Chef1.Chicken()
Chef2.Rice()
Chef2.Chicken()
```
