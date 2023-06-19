---
date: 2023-02-09
type: note
tags: 
---

To integrate:

$$
\int \cos^jx\sin^{k}x \, dx 
$$

1. if $k$ is odd, rewrite $\sin^kx = \sin^{k-1}x\sin x$ and use the identity $\sin^2x=1-\cos^2x$ and take the u-sub of $u=\cos x$
2. if $j$ is odd, rewrite $\cos^jx=\cos^{j-1}x\cos x$ and use the identity $\cos^2x=1-\sin^2x$ and take the u-sub of $u=\sin x$
3. if **both** $j$ and $j$ are even, use $\sin^2x=\frac{{1-\cos(2x)}}{2}$ and $\cos^2x=\frac{{1+\cos(2x)}}{2}$, then simplify and reapply the above strategies
