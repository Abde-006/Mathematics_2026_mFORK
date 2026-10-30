## Exercise 10 — Triangle Area from Vectors

### Problem Statement
For $A=(0,0,0)$, $B=(2,1,0)$, and $C=(1,3,2)$, construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$, compute the parallelogram area using the cross product, and find the triangle area. Explain the factor $1/2$.

### Objective
Use the magnitude of a cross product to find parallelogram and triangle areas.

### Concepts and Formulas
- The area of the parallelogram spanned by $p,q$ is $\|p\times q\|$.
- A triangle formed by the same two side vectors has half the parallelogram's area.

### Step-by-Step Solution

#### Step 1 — Construct side vectors

$$
\overrightarrow{AB}=B-A=(2,1,0),\qquad
\overrightarrow{AC}=C-A=(1,3,2)
$$

#### Step 2 — Compute their cross product

$$
\overrightarrow{AB}\times\overrightarrow{AC}
=(1\cdot2-0\cdot3,\;0\cdot1-2\cdot2,\;2\cdot3-1\cdot1)
=(2,-4,5)
$$

#### Step 3 — Find the areas

$$
\|\overrightarrow{AB}\times\overrightarrow{AC}\|
=\sqrt{2^2+(-4)^2+5^2}=\sqrt{45}=3\sqrt{5}
$$

This is the parallelogram area. The triangle occupies half of that parallelogram:

$$
\mathrm{Area}_{\triangle ABC}=\frac{1}{2}(3\sqrt{5})=\frac{3\sqrt{5}}{2}
$$

### Verification
The cross-product magnitude is nonnegative and gives the parallelogram spanned by the two sides from $A$. A diagonal divides that parallelogram into two equal-area triangles.

### Final Answer
The parallelogram area is $3\sqrt{5}$, and the triangle area is $3\sqrt{5}/2$.

### Key Takeaways
- A cross-product magnitude measures the area spanned by its input vectors.
- The factor $1/2$ appears because a triangle is half of its corresponding parallelogram.
