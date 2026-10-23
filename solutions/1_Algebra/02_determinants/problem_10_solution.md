# Solution 10 — Detecting Dependence

### Problem Statement
Explain without a full determinant calculation why

$$
\det\begin{pmatrix}1&2&3\\2&4&6\\0&1&5\end{pmatrix}=0.
$$

Identify a row dependence and relate it to invertibility.

### Objective
Recognize a zero determinant from linearly dependent rows.

### Concepts and Formulas
A square matrix with linearly dependent rows has determinant zero and is not invertible.

### Step-by-Step Solution
The second row is twice the first:

$$
(2,4,6)=2(1,2,3).
$$

Thus the rows are linearly dependent. A determinant with two proportional rows is zero, so

$$
\det\begin{pmatrix}1&2&3\\2&4&6\\0&1&5\end{pmatrix}=0.
$$

The rows are not independent, so the matrix is singular and has no inverse.

### Final Answer
The specific dependence is $R_2=2R_1$. Therefore the determinant is $0$, and the matrix is not invertible.

### Key Takeaways
- A visible linear dependence among rows immediately implies determinant zero.