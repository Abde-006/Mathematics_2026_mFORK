# Solution 12 — A Parameter Revealed by a Row Operation

### Problem Statement
For

$$
A(t)=\begin{pmatrix}1&2&3\\2&4&t\\0&1&1\end{pmatrix},
$$

find the noninvertible values of $t$ after applying $R_2\leftarrow R_2-2R_1$, and explain the row behavior at that value.

### Objective
Use a determinant-preserving row operation to expose the singular parameter.

### Concepts and Formulas
Replacing a row by itself plus a multiple of another row preserves the determinant. A square matrix is singular exactly when its determinant is zero.

### Step-by-Step Solution
Apply the requested operation:

$$
R_2-2R_1=(2,4,t)-2(1,2,3)=(0,0,t-6).
$$

The resulting matrix is

$$
\begin{pmatrix}1&2&3\\0&0&t-6\\0&1&1\end{pmatrix}.
$$

The operation preserves the determinant. Expanding along the first column,

$$
\det A(t)=
\begin{vmatrix}0&t-6\\1&1\end{vmatrix}
=0\cdot1-(t-6)\cdot1=6-t.
$$

Set $6-t=0$, obtaining $t=6$. At this value the transformed second row is zero. In the original matrix, $R_2=(2,4,6)=2R_1$.

### Final Answer
The matrix is not invertible only for

$$
\boxed{t=6}.
$$

At $t=6$, the second row of the original matrix is twice its first row.

### Key Takeaways
- A row operation can expose dependence without changing the determinant.
- A zero row in the transformed matrix signals a zero determinant.