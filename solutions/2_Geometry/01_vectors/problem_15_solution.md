## Exercise 15 — Comparing Directions Using the Cosine of the Angle

### Problem Statement
For $a=(1,2,1)$, $b=(2,4,2)$, and $c=(2,0,3)$, compute $\frac{u\cdot v}{\|u\|\|v\|}$ for each pair, order the pairs by increasing angle, and explain why the value for $a,b$ is $1$ despite their different lengths.

### Objective
Compare angles using normalized dot products and distinguish direction from vector length.

### Concepts and Formulas
- For nonzero vectors $u,v$, $\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}$.
- Since cosine decreases as the angle increases from $0$ to $\pi$, larger cosine values correspond to smaller angles.

### Step-by-Step Solution

#### Step 1 — Compute lengths

$$
\|a\|=\sqrt{1+4+1}=\sqrt{6},\qquad
\|b\|=\sqrt{4+16+4}=\sqrt{24}=2\sqrt{6}
$$

$$
\|c\|=\sqrt{4+0+9}=\sqrt{13}
$$

#### Step 2 — Compute each normalized dot product
For $a$ and $b$:

$$
a\cdot b=1(2)+2(4)+1(2)=12,\qquad
\frac{a\cdot b}{\|a\|\|b\|}=\frac{12}{\sqrt{6}(2\sqrt{6})}=1
$$

For $a$ and $c$:

$$
a\cdot c=1(2)+2(0)+1(3)=5,\qquad
\frac{a\cdot c}{\|a\|\|c\|}=\frac{5}{\sqrt{78}}
$$

For $b$ and $c$:

$$
b\cdot c=2(2)+4(0)+2(3)=10,\qquad
\frac{b\cdot c}{\|b\|\|c\|}=\frac{10}{\sqrt{24}\sqrt{13}}=\frac{5}{\sqrt{78}}
$$

#### Step 3 — Order the angles
The cosine for $(a,b)$ is $1$, so its angle is $0^\circ$. The other two cosine values are equal and positive, so their angles are equal and larger than zero.

### Verification
$b=2a$, so $a$ and $b$ have the same direction and orientation even though $\|b\|=2\|a\|$. Also $b\cdot c=2(a\cdot c)$ and $\|b\|=2\|a\|$, so the scaling cancels in the normalized dot product for the pairs with $c$.

### Final Answer

$$
\frac{a\cdot b}{\|a\|\|b\|}=1,\qquad
\frac{a\cdot c}{\|a\|\|c\|}=\frac{5}{\sqrt{78}},\qquad
\frac{b\cdot c}{\|b\|\|c\|}=\frac{5}{\sqrt{78}}
$$

The pairs in increasing angle order are $(a,b)$ first, followed by the tie $(a,c)$ and $(b,c)$. The value $1$ for $(a,b)$ occurs because one vector is a positive scalar multiple of the other, giving angle zero.

### Key Takeaways
- Normalizing the dot product removes the effect of vector lengths.
- Positive scalar multiples have identical direction and cosine value $1$.
