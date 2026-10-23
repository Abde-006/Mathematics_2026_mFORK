# Solution 1 — Determinant of a 2×2 Matrix

### Problem Statement
Compute the determinants of

$$
\begin{pmatrix}3&-2\\5&4\end{pmatrix}
\qquad\text{and}\qquad
\begin{pmatrix}1&7\\2&14\end{pmatrix},
$$

and determine which matrix is invertible.

### Objective
Use the formula for a $2\times2$ determinant to test invertibility.

### Concepts and Formulas
For $\begin{pmatrix}a&b\\c&d\end{pmatrix}$,

$$
\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc.
$$

A square matrix is invertible exactly when its determinant is nonzero.

### Step-by-Step Solution
For the first matrix,

$$
\det\begin{pmatrix}3&-2\\5&4\end{pmatrix}
=3(4)-(-2)(5)=12+10=22.
$$

For the second matrix,

$$
\det\begin{pmatrix}1&7\\2&14\end{pmatrix}
=1(14)-7(2)=14-14=0.
$$

The first determinant is nonzero, while the second is zero.

### Final Answer
The determinants are $22$ and $0$, respectively. The first matrix is invertible; the second is not.

### Key Takeaways
- A $2\times2$ determinant is the diagonal product difference $ad-bc$.
- A square matrix is invertible if and only if its determinant is nonzero.