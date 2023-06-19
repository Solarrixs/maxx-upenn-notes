---
date: 2023-04-28
type: note
tags: ankify
---

The training of a model with $x_{n}$ and $y_{n}$ with the loss being a mean squared error:

$$
L(w) = \frac{1}{N} \sum_{n=1}^N (y_{n}-f(x_{n};w))^2
$$

The function $f(x_{n};w)$ represents the input data adjusted by the pre-defined neural weights. The equation points to finding the value of $w$ to minimize the loss error.
