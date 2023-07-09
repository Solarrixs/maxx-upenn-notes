---
date: 2023-07-10
type: note
tags: 
---

## Applications of Multi-Calculus
Vectors and matrices are highly useful in certain applications:
- Statistics: Extracting patterns from data requires linear algebra to perform linear regressions
- Machine Learning: Vectors and dot products in high dimensions determine patterns in data. A hyperplane also separates data of different types.
- High Dimension Geometry: Utilizes determinants and matrices to compute volumes in multiple dimensions.
- Large linear systems of equations: Can be solved using matrices and vectors.

## Equation of Planes
Planes are just lines in 3D. So formulas of planes are similar to formula of lines.
Point-slope plane equation: $n_{x}(x-x_{0})+n_{y}(y-y_{0})+n_{z}(z-z_{0})=0$. This is a plane with the slope of $(n_{x}, n_{y}, n_{z})$ that passes through $(x_{0}, y_{0}, z_{0})$.
Intercept form plane equation: $\frac{x}{a}+ \frac{y}{b} + \frac{z}{c} = 1$

> [!help|c-pink dim]- Equations of parallel planes
> What is the equation of a plane passing through the point (0, -1, 5) & parallel to the plane given by $2x-4y+3z=8$?
>
> > [!done|clean]- Answer
> > Using the point-slope equation: $2(x-0) -4(y+1)+3(z-5)=0$ or $2x-4y+3z=19$.

## Parametrized Lines in 3D
Lines will often use a parametrized variable, such as s or r. That means a line can be represented by $x(t), y(t), z(t)$.

> [!help|c-pink dim]- Parametrization of a line passing through points
> Find the parametrization of the line passing through (4, 2, 5) and (-1, 3, 3)
>
> > [!done|clean]- Answer
> > The x starts at 4 and changes from 4 to -1, so that becomes $-5t+4$
> > The y starts at 2 and changes from 2 to 3, so that becomes $1t+2$
> > The z starts at 5 and changes from 5 to 3, so that becomes $-2z+5$

## Curves and Surfaces
Curves and surfaces can be defined parametrically or implicitly. Parametrically defined surfaces and curves are represented by multiple variables, such as $x(r,s), y(r,s), z(r,s)$.

### Sphere

$$
(x-x_{0})^2+(y-y_{0})^2+(z-z_{0})^2=r^2
$$

or

$$
\dfrac{(x-x_{0})^2}{r^2}+\dfrac{(y-y_{0})^2}{r^2}+\dfrac{(z-z_{0})^2}{r^2}=1
$$

### Ellipsoids

$$
\dfrac{(x-x_{0})^2}{a^2}+\dfrac{(y-y_{0})^2}{b^2}+\dfrac{(z-z_{0})^2}{c^2}=1
$$

### Hyperboloids

$$
\dfrac{(x-x_{0})^2}{a^2}+\dfrac{(y-y_{0})^2}{b^2}-\dfrac{(z-z_{0})^2}{c^2}=1
$$

This hyperboloid "opens up" from the z-axis side because it has the negative sign and is connected.

$$
\dfrac{(x-x_{0})^2}{a^2}-\dfrac{(y-y_{0})^2}{b^2}-\dfrac{(z-z_{0})^2}{c^2}=1
$$

This hyperboloid "opens up" from the x-axis side because it has the positive sign and is disconnected.

A cone is a degenerate hyperboloid. It meets at a point in the middle.

$$
\dfrac{(x-x_{0})^2}{a^2}+\dfrac{(y-y_{0})^2}{b^2}=\dfrac{(z-z_{0})^2}{c^2}
$$

### Elliptic Paraboloids
Similar to hyperboloid but one term becomes linear and that is where it opens up.

$$
\dfrac{(x-x_{0})^2}{a^2}+\dfrac{(y-y_{0})^2}{b^2}=z-z_{0}
$$

### Hyperbolic Paraboloids
Similar to a parabola + hyperbola along certain cross sections

$$
\dfrac{(x-x_{0})^2}{a^2}-\dfrac{(y-y_{0})^2}{b^2}=z-z_{0}
$$
