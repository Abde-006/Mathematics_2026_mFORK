# Solution 15 — Combining Determinant Properties

### Problem Statement
Let $A,B$ be invertible $2\times2$ matrices with $\det A=-2$ and $\det B=3$. Compute

$$
\det(B^{-1}A^TB).
$$

### Objective
Combine determinant rules for products, inverses, and transposes.

### Concepts and Formulas

$$
\det(XYZ)=\det X\,\det Y\,\det Z,\qquad
\det(B^{-1})=\frac{1}{\det B},\qquad
\det(A^T)=\det A.
$$

### Step-by-Step Solution
Apply multiplicativity in the order of the factors:

$$
\det(B^{-1}A^TB)
=\det(B^{-1})\det(A^T)\det(B).
$$

Substitute the given determinants and the inverse/transpose properties:

$$
=\frac{1}{\det B}\det A\det B
=\frac13(-2)(3)=-2.
$$

The factors $\det(B^{-1})=1/3$ and $\det B=3$ multiply to $1$, so they cancel.

### Final Answer

$$
\boxed{\det(B^{-1}A^TB)=-2}.
$$

### Key Takeaways
- The determinant of a product is the product of the determinants in the same order.
- The determinant contributions from $B^{-1}$ and $B$ cancel.