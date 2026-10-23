# Solution 4 — Triangular Matrix

### Problem Statement
Compute the determinant of

$$
\begin{pmatrix}2&4&1\\0&-3&5\\0&0&7\end{pmatrix}
$$

without expansion, and state the rule for any triangular matrix.

### Objective
Use the diagonal-product rule for triangular matrices.

### Concepts and Formulas
The determinant of any upper- or lower-triangular matrix is the product of its diagonal entries.

### Step-by-Step Solution
The matrix is upper triangular, so multiply its diagonal entries:

$$
\det A=2\cdot(-3)\cdot7=-42.
$$

The entries above the diagonal do not affect this product. More generally, for a triangular $n\times n$ matrix with diagonal entries $a_{11},\ldots,a_{nn}$,

$$
\det A=\prod_{i=1}^{n}a_{ii}.
$$

### Final Answer

$$
\boxed{\det A=-42}.
$$

### Key Takeaways
- For a triangular matrix, multiply the diagonal entries.
- This avoids determinant expansion.