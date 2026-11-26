## Exercise 12 — A Normal Vector to a Plane

### Problem statement

Given $A=(1,0,2)$, $B=(2,1,0)$, and $C=(0,3,1)$, construct two vectors in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

### Formula used

Vectors lying in a plane through $A$, $B$, and $C$ are obtained by point differences:

$$
\overrightarrow{AB}=B-A,\qquad \overrightarrow{AC}=C-A
$$

A cross product of two nonparallel in-plane vectors produces a normal vector:

$$
n=p\times q
$$

Perpendicularity is verified by

$$
n\cdot p=0,\qquad n\cdot q=0
$$

### Solution

Construct two directions from $A$:

$$
\overrightarrow{AB}=B-A=(2-1,1-0,0-2)=(1,1,-2)
$$

$$
\overrightarrow{AC}=C-A=(0-1,3-0,1-2)=(-1,3,-1)
$$

Compute their cross product:

$$
\begin{aligned}
n
&=(1,1,-2)\times(-1,3,-1) \\
&=(1(-1)-(-2)(3),\,(-2)(-1)-1(-1),\,1(3)-1(-1)) \\
&=(-1+6,\,2+1,\,3+1) \\
&=(5,3,4)
\end{aligned}
$$

### Verification

Check $n$ against $\overrightarrow{AB}$:

$$
n\cdot\overrightarrow{AB}
=(5,3,4)\cdot(1,1,-2)
=5+3-8
=0
$$

Check $n$ against $\overrightarrow{AC}$:

$$
n\cdot\overrightarrow{AC}
=(5,3,4)\cdot(-1,3,-1)
=-5+9-4
=0
$$

Both dot products are zero, so $n$ is perpendicular to two independent directions in the plane.

### Final answer

$$
\overrightarrow{AB}=(1,1,-2)
$$

$$
\overrightarrow{AC}=(-1,3,-1)
$$

One normal vector is

$$
n=(5,3,4)
$$
