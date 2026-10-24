## Exercise 5 — Matrix Times Vector

### Problem Statement
Let

$$
A=\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

### Objective
Compute the matrix-vector product and express it as a linear combination of the matrix columns.

### Concepts and Formulas
- A matrix-vector product uses the rows of the matrix and the entries of the vector.
- If

$$
A=[c_1\ c_2],
$$

then

$$
Ax=x_1c_1+x_2c_2.
$$

This means the vector $x$ tells us how much of each column to take.

### Step-by-Step Solution

#### Step 1 — Compute $Ax$

$$
Ax=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute each entry:
- First entry: $2\cdot4+(-1)\cdot2=8-2=6$
- Second entry: $1\cdot4+3\cdot2=4+6=10$

Therefore,

$$
Ax=\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

#### Step 2 — Express it as a linear combination of the columns
The columns of $A$ are

$$
c_1=\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},\qquad c_2=\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}.
$$

The vector $x$ is

$$
x=\begin{pmatrix}
4 \\
2 \\
\end{pmatrix},
$$

so the linear combination is

$$
4c_1+2c_2.
$$

Compute it:

$$
4\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}+2\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
= \begin{pmatrix}
8 \\
4 \\
\end{pmatrix}+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
= \begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

This matches the matrix-vector product.

### Final Answer

$$
Ax=\begin{pmatrix}
6 \\
10 \\
\end{pmatrix},
$$

and

$$
Ax=4\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}+2\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}.
$$

### Key Takeaways
- Multiplying a matrix by a vector is a structured way of combining the columns of the matrix.
- The entries of the vector act as coefficients in a linear combination.
- This idea is fundamental in linear algebra.
