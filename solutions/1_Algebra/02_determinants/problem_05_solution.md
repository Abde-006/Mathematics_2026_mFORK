# Solution 5 — Row Operations

### Problem Statement
Find the determinant of

$$
A=\begin{pmatrix}1&2&3\\2&1&0\\-1&4&2\end{pmatrix}
$$

by simplifying with row operations, recording how each operation affects the determinant.

### Objective
Track determinant-preserving row replacements during simplification.

### Concepts and Formulas
- Replacing $R_i$ by $R_i+cR_j$ does not change the determinant.
- A triangular matrix's determinant is the product of its diagonal entries.

### Step-by-Step Solution
Apply $R_2\leftarrow R_2-2R_1$; this does not change the determinant:

$$
\begin{pmatrix}1&2&3\\0&-3&-6\\-1&4&2\end{pmatrix}.
$$

Then apply $R_3\leftarrow R_3+R_1$, also determinant-preserving:

$$
\begin{pmatrix}1&2&3\\0&-3&-6\\0&6&5\end{pmatrix}.
$$

Expanding along the first column reduces the determinant to

$$
\begin{vmatrix}-3&-6\\6&5\end{vmatrix}
=(-3)(5)-(-6)(6)=-15+36=21.
$$

### Verification
Both row operations were row replacements, so neither changed the determinant. The reduced $2\times2$ determinant is $21$.

### Final Answer

$$
\boxed{\det A=21}.
$$

### Key Takeaways
- Row replacements of the form $R_i\leftarrow R_i+cR_j$ preserve the determinant.
- Track row swaps and row scalings separately, since those do change it.