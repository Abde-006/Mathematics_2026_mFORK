## Exercise 13 — Do Four Points Lie in One Plane?

### Problem statement

Given

$$
A=(0,0,0),\qquad B=(1,2,0),\qquad C=(0,1,1),\qquad D=(2,5,1)
$$

construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$, find $n=\overrightarrow{AB}\times\overrightarrow{AC}$, construct $\overrightarrow{AD}$, and check $\overrightarrow{AD}\cdot n=0$. Decide whether $D$ lies in the plane determined by $A,B,C$, and justify the criterion.

### Formula used

Two nonparallel vectors from $A$,

$$
p=B-A,\qquad q=C-A
$$

span the plane through $A,B,C$. Their cross product

$$
n=p\times q
$$

is a normal vector. A point $D$ lies in the plane exactly when

$$
(D-A)\cdot n=0
$$

because $D-A$ must then be perpendicular to the normal and therefore parallel to a direction in the plane.

### Solution

Construct the first two plane directions:

$$
\overrightarrow{AB}=B-A=(1,2,0)
$$

$$
\overrightarrow{AC}=C-A=(0,1,1)
$$

Compute a normal:

$$
\begin{aligned}
n
&=\overrightarrow{AB}\times\overrightarrow{AC} \\
&=(2(1)-0(1),\,0(0)-1(1),\,1(1)-2(0)) \\
&=(2,-1,1)
\end{aligned}
$$

Construct the displacement from $A$ to $D$:

$$
\overrightarrow{AD}=D-A=(2,5,1)
$$

Test it against the normal:

$$
\overrightarrow{AD}\cdot n
=(2,5,1)\cdot(2,-1,1)
=4-5+1
=0
$$

Because the dot product is zero, $\overrightarrow{AD}$ is in a direction contained in the plane.

This can also be verified directly:

$$
\overrightarrow{AD}=2\overrightarrow{AB}+\overrightarrow{AC}
=2(1,2,0)+(0,1,1)
=(2,5,1)
$$

### Final answer

$$
n=(2,-1,1)
$$

Since $\overrightarrow{AD}\cdot n=0$, $D$ lies in the plane determined by $A$, $B$, and $C$.
