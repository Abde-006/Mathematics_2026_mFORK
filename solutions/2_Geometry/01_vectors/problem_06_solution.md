## Exercise 6 — Projection and Perpendicular Component

### Problem statement

For $u=(4,2)$ and $v=(1,1)$, find the projection of $u$ onto $v$, then compute $r=u-\mathrm{proj}_v u$ and verify $r\cdot v=0$. Explain the result geometrically.

### Formula used

The projection onto a nonzero direction $v$ is

$$
\mathrm{proj}_v u
=\frac{u\cdot v}{v\cdot v}v
$$

The coefficient $(u\cdot v)/(v\cdot v)$ is used because it chooses the scalar multiple of $v$ that points in the correct direction along $v$.

The perpendicular component is

$$
r=u-\mathrm{proj}_v u
$$

It is perpendicular to $v$ because the projection accounts for every part of $u$ parallel to $v$.

### Solution

First compute the dot products:

$$
u\cdot v=4(1)+2(1)=6
$$

$$
v\cdot v=1^2+1^2=2
$$

The projection coefficient is therefore

$$
\frac{u\cdot v}{v\cdot v}=\frac{6}{2}=3
$$

Multiply $v$ by this coefficient:

$$
\mathrm{proj}_v u=3(1,1)=(3,3)
$$

Subtract it from $u$:

$$
r=(4,2)-(3,3)=(1,-1)
$$

### Verification

Check the perpendicularity:

$$
r\cdot v=(1,-1)\cdot(1,1)=1-1=0
$$

Therefore $r$ is perpendicular to $v$. The decomposition also reconstructs $u$:

$$
(3,3)+(1,-1)=(4,2)
$$

### Geometric interpretation

The vector $(3,3)$ is the shadow of $u$ along the line spanned by $v$. The vector $(1,-1)$ is the perpendicular offset from that line to the tip of $u$.

### Final answer

$$
\mathrm{proj}_v u=(3,3)
$$

$$
r=(1,-1)
$$
