## Exercise 8 — Linear Combination and Checking the Result

### Problem statement

Check whether

$$
w=(5,1)
$$

can be written as $w=au+bv$, where $u=(1,1)$ and $v=(2,-1)$. If so, find $a,b$, reconstruct $w$, and explain the geometric meaning.

### Formula used

A linear combination scales both vectors and adds them:

$$
au+bv=a(u_1,u_2)+b(v_1,v_2)
=(au_1+bv_1,au_2+bv_2)
$$

Matching coordinates gives a system of equations. Because $u$ and $v$ are nonparallel, they span $\mathbb R^2$, so every vector in the plane should have a solution.

### Solution

Form the combination:

$$
au+bv
=a(1,1)+b(2,-1)
=(a+2b,a-b)
$$

Set this equal to $(5,1)$:

$$
(a+2b,a-b)=(5,1)
$$

This gives

$$
\begin{cases}
a+2b=5, \\
a-b=1.
\end{cases}
$$

Subtract the second equation from the first:

$$
(a+2b)-(a-b)=5-1
$$

$$
3b=4
$$

so

$$
b=\frac{4}{3}
$$

Substitute into $a-b=1$:

$$
a-\frac{4}{3}=1
$$

$$
a=\frac{7}{3}
$$

### Verification

Reconstruct $w$:

$$
\frac{7}{3}(1,1)+\frac{4}{3}(2,-1)
=\left(\frac{7}{3}+\frac{8}{3},\frac{7}{3}-\frac{4}{3}\right)
=(5,1)
$$

This matches $(5,1)$ in both coordinates.

### Geometric interpretation

The coefficient $a$ scales $u$, and $b$ scales $v$. Their scaled sum reaches $w$. Since $u$ and $v$ point in different directions, their possible sums fill the plane.

### Final answer

$$
a=\frac{7}{3},\qquad b=\frac{4}{3}
$$

$$
w=\frac{7}{3}u+\frac{4}{3}v=(5,1)
$$
