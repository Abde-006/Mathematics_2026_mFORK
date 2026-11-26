## Exercise 10 — Triangle Area from Vectors

### Problem statement

For $A=(0,0,0)$, $B=(2,1,0)$, and $C=(1,3,2)$:

1. Construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$.
2. Compute the parallelogram area using the cross product.
3. Find the triangle area.
4. Explain the factor $\frac12$.

### Lettered quantities

Let $A$, $B$, and $C$ denote the three given points. Define

$$
\vec p=\overrightarrow{AB},\qquad
\vec q=\overrightarrow{AC}
$$

Here $\vec p$ and $\vec q$ are the two side vectors of the triangle that begin at $A$. The symbols $A_{\mathrm{parallelogram}}$ and $A_{\triangle ABC}$ represent the parallelogram area and triangle area, respectively.

### Formula used

#### Formula 1 — Vector between two points

If $X=(x_1,x_2,x_3)$ and $Y=(y_1,y_2,y_3)$, then the vector from $X$ to $Y$ is

$$
\overrightarrow{XY}=Y-X
=(y_1-x_1,y_2-x_2,y_3-x_3)
$$

This formula is used to construct $\vec p=\overrightarrow{AB}$ and $\vec q=\overrightarrow{AC}$ from coordinate differences.

#### Formula 2 — Cross product

For $\vec p=(p_1,p_2,p_3)$ and $\vec q=(q_1,q_2,q_3)$, the cross product is

$$
\vec p\times\vec q
=
(p_2q_3-p_3q_2,\,
p_3q_1-p_1q_3,\,
p_1q_2-p_2q_1)
$$

This formula produces a vector perpendicular to both side vectors.

#### Formula 3 — Magnitude of a vector

For $\vec w=(w_1,w_2,w_3)$, its length is

$$
\|\vec w\|=\sqrt{w_1^2+w_2^2+w_3^2}
$$

Applying this formula to $\vec p\times\vec q$ gives the area of the parallelogram spanned by $\vec p$ and $\vec q$:

$$
A_{\mathrm{parallelogram}}=\|\vec p\times\vec q\|
$$

#### Formula 4 — Triangle area

A triangle is half of the corresponding parallelogram:

$$
A_{\triangle ABC}
=\frac12\|\overrightarrow{AB}\times\overrightarrow{AC}\|
$$

The factor $\frac12$ appears because a diagonal divides a parallelogram into two equal triangles.

### Solution

#### Step 1 — Construct $\vec p=\overrightarrow{AB}$ using Formula 1

Use $X=A=(0,0,0)$ and $Y=B=(2,1,0)$:

$$
\vec p=\overrightarrow{AB}
=B-A
=(2-0,1-0,0-0)
=(2,1,0)
$$

#### Step 2 — Construct $\vec q=\overrightarrow{AC}$ using Formula 1

Use $X=A=(0,0,0)$ and $Y=C=(1,3,2)$:

$$
\vec q=\overrightarrow{AC}
=C-A
=(1-0,3-0,2-0)
=(1,3,2)
$$

#### Step 3 — Compute $\vec p\times\vec q$ using Formula 2

From Steps 1 and 2,

$$
\vec p=(p_1,p_2,p_3)=(2,1,0)
$$

and

$$
\vec q=(q_1,q_2,q_3)=(1,3,2)
$$

Substitute these lettered components into the cross-product formula:

$$
\begin{aligned}
\vec p\times\vec q
&=(p_2q_3-p_3q_2,\,
p_3q_1-p_1q_3,\,
p_1q_2-p_2q_1) \\
&=(1(2)-0(3),\,0(1)-2(2),\,2(3)-1(1)) \\
&=(2,-4,5)
\end{aligned}
$$

#### Step 4 — Compute the parallelogram area using Formula 3

Use $\vec w=\vec p\times\vec q=(2,-4,5)$:

$$
\begin{aligned}
A_{\mathrm{parallelogram}}
&=\|\vec p\times\vec q\| \\
&=\|(2,-4,5)\| \\
&=\sqrt{2^2+(-4)^2+5^2} \\
&=\sqrt{4+16+25} \\
&=\sqrt{45} \\
&=3\sqrt5
\end{aligned}
$$

Thus the parallelogram area is $3\sqrt5$ square units.

#### Step 5 — Compute the triangle area using Formula 4

The triangle uses the same two side vectors, but it occupies half of their parallelogram:

$$
\begin{aligned}
A_{\triangle ABC}
&=\frac12\|\vec p\times\vec q\| \\
&=\frac12(3\sqrt5) \\
&=\frac{3\sqrt5}{2}
\end{aligned}
$$

### Verification

The cross product is $(2,-4,5)$, so its magnitude is positive and nonzero. Therefore $\vec p$ and $\vec q$ are not parallel, $A$, $B$, and $C$ are not collinear, and the triangle has a nonzero area.

The factor $\frac12$ is necessary because the diagonal $AC$ divides the parallelogram spanned by $\overrightarrow{AB}$ and $\overrightarrow{AC}$ into two triangles of equal area.

### Final answer

$$
A_{\mathrm{parallelogram}}=3\sqrt5
$$

$$
A_{\triangle ABC}=\frac{3\sqrt5}{2}
$$
