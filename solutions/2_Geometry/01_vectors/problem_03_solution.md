## Exercise 3 — Vector Normalization

### Problem Statement
For $v=(3,4)$, find a unit vector $e$ with the same direction and orientation. Check its length, reconstruct $v$ as $\|v\|e$, and explain what changes and what remains unchanged during normalization.

### Objective
Separate a vector's direction from its magnitude by constructing a unit vector.

### Concepts and Formulas
- The length of $(x,y)$ is $\sqrt{x^2+y^2}$.
- For a nonzero vector, the unit vector in its direction is $e=v/\|v\|$.
- Normalization changes the length to one but preserves direction and orientation.

### Step-by-Step Solution

#### Step 1 — Find the magnitude of $v$

$$
\|v\|=\sqrt{3^2+4^2}=\sqrt{25}=5
$$

#### Step 2 — Divide by the magnitude

$$
e=\frac{v}{\|v\|}=\left(\frac{3}{5},\frac{4}{5}\right)
$$

#### Step 3 — Verify that $e$ is a unit vector

$$
\|e\|=\sqrt{\left(\frac{3}{5}\right)^2+\left(\frac{4}{5}\right)^2}
=\sqrt{\frac{9}{25}+\frac{16}{25}}=1
$$

#### Step 4 — Reconstruct the original vector

$$
\|v\|e=5\left(\frac{3}{5},\frac{4}{5}\right)=(3,4)=v
$$

### Verification
The calculated unit vector has length one, and multiplying it by the original length recovers both coordinates of $v$.

### Final Answer

$$
e=\left(\frac{3}{5},\frac{4}{5}\right),\qquad \|v\|=5,\qquad v=5e
$$

Normalization changes the length from $5$ to $1$, while the direction and orientation stay the same.

### Key Takeaways
- Dividing a nonzero vector by its length produces a unit vector.
- A vector can be represented as its magnitude times its unit direction.
