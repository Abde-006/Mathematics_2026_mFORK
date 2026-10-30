## Exercise 8 — Linear Combination and Checking the Result

### Problem Statement
Determine whether $w=(5,1)$ can be written as $w=au+bv$ for $u=(1,1)$ and $v=(2,-1)$. If possible, find and check $a,b$, and explain the geometric meaning.

### Objective
Solve for coefficients in a linear combination and verify the resulting vector.

### Concepts and Formulas
- A linear combination $au+bv$ scales each vector and adds the results.
- Equality of vectors requires equality in each coordinate.
- Two nonparallel vectors in $\mathbb R^2$ span the plane.

### Step-by-Step Solution

#### Step 1 — Match coordinates

$$
a(1,1)+b(2,-1)=(a+2b,a-b)=(5,1)
$$

This gives the system

$$
\begin{cases}
a+2b=5, \\
a-b=1. \\
\end{cases}
$$

#### Step 2 — Solve the system
Subtract the second equation from the first: $3b=4$, so $b=4/3$. Substituting into $a-b=1$ gives $a=7/3$.

#### Step 3 — Reconstruct $w$

$$
\frac{7}{3}(1,1)+\frac{4}{3}(2,-1)
=\left(\frac{7}{3}+\frac{8}{3},\frac{7}{3}-\frac{4}{3}\right)
=(5,1)
$$

### Verification
The reconstructed first and second coordinates are $5$ and $1$, respectively, so the coefficients satisfy the original vector equation.

### Final Answer

$$
a=\frac{7}{3},\qquad b=\frac{4}{3},\qquad w=\frac{7}{3}u+\frac{4}{3}v
$$

Geometrically, scaling and adding the two directions reaches $w$. Since $u$ and $v$ are not parallel, they span the plane, so vectors in $\mathbb R^2$ can be expressed using them.

### Key Takeaways
- A vector linear-combination question becomes a system of coordinate equations.
- Reconstructing the target vector is an effective check.
