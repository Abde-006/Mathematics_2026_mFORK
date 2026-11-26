## Exercise 4 — Dot Product and Perpendicularity

### Problem statement

For $u=(1,2,-1)$ and $v=(2,-1,3)$, compute $u\cdot v$ and determine whether the vectors are perpendicular. Then find $a$ so that $w=(2,-1,a)$ is perpendicular to $u$, and check the result.

### Formula used

The dot product in $\mathbb R^3$ is

$$
(a_1,a_2,a_3)\cdot(b_1,b_2,b_3)
=a_1b_1+a_2b_2+a_3b_3
$$

For nonzero vectors, perpendicularity is equivalent to

$$
u\cdot v=0
$$

This test is used both to decide whether the given pair is perpendicular and to solve for the unknown coordinate.

### Solution

Compute the dot product of $u$ and $v$:

$$
u\cdot v
=1(2)+2(-1)+(-1)(3)
=2-2-3
=-3
$$

Since $-3\neq0$, $u$ and $v$ are not perpendicular.

For $w=(2,-1,a)$, impose perpendicularity to $u$:

$$
u\cdot w
=1(2)+2(-1)+(-1)a
=2-2-a
=-a
$$

Setting this equal to zero gives

$$
-a=0
$$

so

$$
a=0
$$

### Verification

Substitute $a=0$:

$$
u\cdot(2,-1,0)=1(2)+2(-1)+(-1)(0)=2-2+0=0
$$

Thus $(2,-1,0)$ is perpendicular to $u$.

### Final answer

$$
u\cdot v=-3
$$

The vectors $u$ and $v$ are not perpendicular.

$$
a=0
$$
