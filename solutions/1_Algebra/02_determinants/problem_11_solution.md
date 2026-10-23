# Solution 11 — Shortening the Calculation with Row Operations

### Problem Statement
Compute the determinant of

$$
A=\begin{pmatrix}1&2&3\\1&3&4\\1&4&6\end{pmatrix}
$$

using row operations to create zeros, and state which operations preserve the determinant.

### Objective
Simplify a determinant by row replacements while tracking its value.

### Concepts and Formulas
Adding a multiple of one row to another does not change the determinant. The determinant of a triangular matrix is the product of its diagonal entries.

### Step-by-Step Solution
First use $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-R_1$. Both operations preserve the determinant:

$$
\begin{pmatrix}1&2&3\\0&1&1\\0&2&3\end{pmatrix}.
$$

Next, use $R_3\leftarrow R_3-2R_2$, which also preserves the determinant:

$$
\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix}.
$$

This is upper triangular, so its determinant is $1\cdot1\cdot1=1$.

### Final Answer

$$
\boxed{\det A=1}.
$$

Each operation used was a row replacement, so none changed the determinant.

### Key Takeaways
- Creating zeros below pivots can make a determinant easy to read.
- Row replacements preserve the determinant; row swaps and row scalings require additional tracking.