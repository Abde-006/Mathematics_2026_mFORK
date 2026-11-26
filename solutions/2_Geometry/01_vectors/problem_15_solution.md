## Exercise 15 — Comparing Directions Using the Cosine of the Angle

### Problem statement

Given

$$
a=(1,2,1),\qquad b=(2,4,2),\qquad c=(2,0,3)
$$

compute

$$
\frac{u\cdot v}{\|u\|\|v\|}
$$

for each pair, order the pairs by increasing angle, and explain why $a$ and $b$ have cosine $1$ even though their lengths differ.

### Formula used

For nonzero vectors,

$$
\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}
$$

The cosine decreases as the angle increases from $0$ to $\pi$. Therefore:

- cosine $1$ means angle $0^\circ$;
- a larger positive cosine means a smaller acute angle;
- cosine $0$ means a right angle.

The denominator normalizes for vector length.

### Solution

First calculate the lengths:

$$
\|a\|=\sqrt{1^2+2^2+1^2}=\sqrt{6}
$$

$$
\|b\|=\sqrt{2^2+4^2+2^2}=\sqrt{24}=2\sqrt{6}
$$

$$
\|c\|=\sqrt{2^2+0^2+3^2}=\sqrt{13}
$$

#### Pair $(a,b)$

Compute the dot product:

$$
a\cdot b=1(2)+2(4)+1(2)=12
$$

Then

$$
\frac{a\cdot b}{\|a\|\|b\|}
=\frac{12}{\sqrt{6}(2\sqrt{6})}
=\frac{12}{12}
=1
$$

This cosine corresponds to angle $0^\circ$.

#### Pair $(a,c)$

Compute the dot product:

$$
a\cdot c=1(2)+2(0)+1(3)=5
$$

Then

$$
\frac{a\cdot c}{\|a\|\|c\|}
=\frac{5}{\sqrt{6}\sqrt{13}}
=\frac{5}{\sqrt{78}}
$$

#### Pair $(b,c)$

Compute the dot product:

$$
b\cdot c=2(2)+4(0)+2(3)=10
$$

Then

$$
\frac{b\cdot c}{\|b\|\|c\|}
=\frac{10}{2\sqrt{6}\sqrt{13}}
=\frac{5}{\sqrt{78}}
$$

### Ordering

The cosine values are

$$
1,\qquad \frac{5}{\sqrt{78}},\qquad \frac{5}{\sqrt{78}}
$$

Because cosine decreases as angle increases, the pair $(a,b)$ has the smallest angle. The pairs $(a,c)$ and $(b,c)$ have equal cosine values and therefore equal angles, both larger than the angle of $(a,b)$.

The value $1$ for $(a,b)$ does not depend on their lengths. It depends on direction:

$$
b=(2,4,2)=2(1,2,1)=2a
$$

The vectors point in exactly the same direction and orientation, so their angle is $0^\circ$. The factor $2$ increases the length but cancels in the normalized dot product.

### Final answer

$$
\frac{a\cdot b}{\|a\|\|b\|}=1
$$

$$
\frac{a\cdot c}{\|a\|\|c\|}
=\frac{b\cdot c}{\|b\|\|c\|}
=\frac{5}{\sqrt{78}}
$$

Increasing-angle order:

$$
(a,b),\,(a,c),\,(b,c)
$$
