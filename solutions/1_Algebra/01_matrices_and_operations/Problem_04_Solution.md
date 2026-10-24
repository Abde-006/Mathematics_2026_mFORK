## Exercise 4 — Matrix Multiplication and Noncommutativity

### Problem Statement
For

$$
A=\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix},
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

### Objective
Compute the products in both orders and compare the results.

### Concepts and Formulas
- Matrix multiplication is computed by taking dot products of rows of the first matrix with columns of the second matrix.
- In general, $AB\ne BA$ for matrices.
- This is called noncommutativity.

### Step-by-Step Solution

#### Step 1 — Compute $AB$

$$
AB=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Take row 1 of $A$ and column 1 of $B$:

$$
1\cdot2+2\cdot3=2+6=8.
$$

Take row 1 of $A$ and column 2 of $B$:

$$
1\cdot0+2\cdot1=0+2=2.
$$

Take row 2 of $A$ and column 1 of $B$:

$$
0\cdot2+1\cdot3=3.
$$

Take row 2 of $A$ and column 2 of $B$:

$$
0\cdot0+1\cdot1=1.
$$

Therefore,

$$
AB=\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $BA$

$$
BA=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}.
$$

Take row 1 of $B$ with column 1 of $A$:

$$
2\cdot1+0\cdot0=2.
$$

Take row 1 of $B$ with column 2 of $A$:

$$
2\cdot2+0\cdot1=4.
$$

Take row 2 of $B$ with column 1 of $A$:

$$
3\cdot1+1\cdot0=3.
$$

Take row 2 of $B$ with column 2 of $A$:

$$
3\cdot2+1\cdot1=7.
$$

So,

$$
BA=\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}.
$$

#### Step 3 — Compare the results

$$
AB=\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix},\qquad BA=\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}.
$$

Since

$$
AB\ne BA,
$$

matrix multiplication is not commutative.

### Final Answer

$$
AB=\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix},\qquad BA=\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix},
$$

so $AB\ne BA$.

### Key Takeaways
- For matrices, the order of multiplication matters.
- In ordinary arithmetic, $xy=yx$, but for matrices this is often false.
- This is why we must be very careful with the order of matrix products.
