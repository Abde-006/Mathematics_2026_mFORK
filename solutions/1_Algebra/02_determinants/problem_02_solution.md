# Solution 2 — Determinant of a 3×3 Matrix

### Problem Statement
Use Sarrus' rule to compute

$$
A=\begin{pmatrix}1&2&-1\\0&3&4\\2&1&5\end{pmatrix}
$$

and check the result using a determinant property.

### Objective
Apply Sarrus' rule and verify the answer with a determinant-preserving row operation.

### Concepts and Formulas
For a $3\times3$ matrix, Sarrus' rule adds the three downward diagonal products and subtracts the three upward diagonal products. Adding a multiple of one row to another does not change a determinant.

### Step-by-Step Solution
The downward products are

$$
1\cdot3\cdot5+2\cdot4\cdot2+(-1)\cdot0\cdot1=15+16+0=31.
$$

The upward products are

$$
(-1)\cdot3\cdot2+1\cdot4\cdot1+2\cdot0\cdot5=-6+4+0=-2.
$$

Therefore,

$$
\det A=31-(-2)=33.
$$

For a check, replace $R_3$ by $R_3-2R_1$. This preserves the determinant and gives

$$
\begin{pmatrix}1&2&-1\\0&3&4\\0&-3&7\end{pmatrix}.
$$

Expanding along its first column gives

$$
\det A=1\begin{vmatrix}3&4\\-3&7\end{vmatrix}
=3(7)-4(-3)=21+12=33.
$$

### Final Answer

$$
\boxed{\det A=33}.
$$

### Key Takeaways
- Sarrus' rule gives $33$.
- A row replacement of the form $R_i\leftarrow R_i+cR_j$ leaves the determinant unchanged, providing a useful check.