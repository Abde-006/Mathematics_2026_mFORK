## Exercise 2 — Addition and Scalar Multiplication

### Problem Statement
For

$$
A=\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix},
$$

compute

$$
A+B,\quad A-B,\quad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

### Objective
Compute the matrix sums and differences entry by entry, and explain why the matrices must have matching dimensions.

### Concepts and Formulas
- Matrix addition: add corresponding entries.
- Matrix subtraction: subtract corresponding entries.
- Scalar multiplication: multiply every entry by the scalar.
- If matrices are the same size, then each entry has a matching partner.

### Step-by-Step Solution

#### Step 1 — Compute $A+B$

$$
A+B=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}+
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
= \begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}
= \begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}.
$$

We add the entries in the same positions.

#### Step 2 — Compute $A-B$

$$
A-B=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}-
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
= \begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}
= \begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}.
$$

Subtraction is done entry by entry, just like addition.

#### Step 3 — Compute $3A-2B$
First multiply each matrix by its scalar:

$$
3A = 3\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix},
$$

$$
2B = 2\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}=
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}.
$$

Subtract the scaled matrices:

$$
3A-2B=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix}-
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}
= \begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}
= \begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

#### Step 4 — Why same-size matrices are required
Matrix addition is defined only when both matrices have the same dimensions. Why? Because each entry in one matrix must be paired with the corresponding entry in the other matrix.

If one matrix were $2\times 2$ and the other $2\times 3$, there would be no entry in the third column of the second matrix to match the third column of the first. So the operation would not be well defined.

### Final Answer

$$
A+B=\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix},
$$

$$
A-B=\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix},
$$

$$
3A-2B=\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

### Key Takeaways
- Addition and subtraction are done entry by entry.
- Scalar multiplication scales each entry separately.
- Same-size matrices are necessary so the entries line up one-to-one.
