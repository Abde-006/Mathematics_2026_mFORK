# Solution 3 — Swapping Two Rows

### Problem Statement
For

$$
A=\begin{pmatrix}1&2&0\\0&3&1\\2&1&1\end{pmatrix},
$$

compute $\det A$, then swap the first and second rows to form $B$. Predict and verify $\det B$.

### Objective
Use and verify the determinant sign change caused by a row swap.

### Concepts and Formulas
Interchanging two rows multiplies a determinant by $-1$.

### Step-by-Step Solution
Expand $\det A$ along its first row:

$$
\det A
=1\begin{vmatrix}3&1\\1&1\end{vmatrix}
-2\begin{vmatrix}0&1\\2&1\end{vmatrix}
=1(3-1)-2(0-2)=2+4=6.
$$

Swapping the first two rows predicts $\det B=-6$. The swapped matrix is

$$
B=\begin{pmatrix}0&3&1\\1&2&0\\2&1&1\end{pmatrix}.
$$

Expanding along its first row,

$$
\det B
=-3\begin{vmatrix}1&0\\2&1\end{vmatrix}
+1\begin{vmatrix}1&2\\2&1\end{vmatrix}
=-3(1)+(1-4)=-6.
$$

The direct calculation agrees with the prediction.

### Final Answer

$$
\det A=6,\qquad \det B=-6.
$$

### Key Takeaways
- A single row swap reverses the sign of a determinant.
- The calculated value for $B$ confirms this property.