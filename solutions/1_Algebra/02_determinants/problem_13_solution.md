# Solution 13 — Determinant by Elimination

### Problem Statement
Use elimination to compute

$$
A=\begin{pmatrix}1&2&3\\2&5&7\\1&0&2\end{pmatrix}
$$

and record the effect of every row operation on the determinant.

### Objective
Reduce the matrix to triangular form while preserving the determinant.

### Concepts and Formulas
Row replacements $R_i\leftarrow R_i+cR_j$ do not change a determinant. A triangular matrix's determinant is the product of its diagonal entries.

### Step-by-Step Solution
Apply $R_2\leftarrow R_2-2R_1$; the determinant is unchanged:

$$
\begin{pmatrix}1&2&3\\0&1&1\\1&0&2\end{pmatrix}.
$$

Apply $R_3\leftarrow R_3-R_1$; the determinant is again unchanged:

$$
\begin{pmatrix}1&2&3\\0&1&1\\0&-2&-1\end{pmatrix}.
$$

Finally apply $R_3\leftarrow R_3+2R_2$, another determinant-preserving replacement:

$$
\begin{pmatrix}1&2&3\\0&1&1\\0&0&1\end{pmatrix}.
$$

The resulting matrix is upper triangular, so its determinant is $1\cdot1\cdot1=1$.

### Final Answer

$$
\boxed{\det A=1}.
$$

### Key Takeaways
- All three elimination steps were row replacements and preserved the determinant.
- The final triangular matrix makes the determinant the product of its diagonal entries.