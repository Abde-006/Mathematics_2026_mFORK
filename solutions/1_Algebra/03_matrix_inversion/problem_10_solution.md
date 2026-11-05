# Exercise 10 — Inverse of a Diagonal Matrix

## Problem Statement

Given

$$
D=\begin{pmatrix}
2&0&0 \\
0&-3&0 \\
0&0&5 \\
\end{pmatrix},
\qquad
E=\begin{pmatrix}
2&0&0 \\
0&0&0 \\
0&0&5 \\
\end{pmatrix},
$$

decide which matrix is invertible without Gauss–Jordan elimination. Give and check the inverse of the invertible matrix.

## Objective

Use the structure of diagonal matrices to identify invertibility and compute the inverse directly.

## Concepts and Formulas

A diagonal matrix is invertible exactly when every diagonal entry is nonzero. Its inverse is diagonal, with each entry replaced by its reciprocal.

## Step-by-Step Solution

### Step 1 — Classify $D$

The diagonal entries of $D$ are $2,-3,5$, all nonzero. Their reciprocals are $\frac12,-\frac13,\frac15$, so the diagonal inverse is

$$
D^{-1}=\begin{pmatrix}
\frac12&0&0 \\
0&-\frac13&0 \\
0&0&\frac15 \\
\end{pmatrix}.
$$

### Step 2 — Check the product

Multiplying matching diagonal entries gives $1$; all off-diagonal entries remain zero:

$$
DD^{-1}
=\begin{pmatrix}
2(\frac12)&0&0 \\
0&(-3)(-\frac13)&0 \\
0&0&5(\frac15) \\
\end{pmatrix}
=I_3.
$$

### Step 3 — Classify $E$

The second diagonal entry of $E$ is zero, so its determinant (the product of the diagonal entries) is $2\cdot0\cdot5=0$. Equivalently, it sends the following nonzero vector to the zero vector:

$$
E\begin{pmatrix}
0 \\
1 \\
0 \\
\end{pmatrix}=0
$$

Therefore, $E$ is not invertible.

## Verification

The displayed reciprocal entries make $DD^{-1}=I_3$. Matrix $E$ sends a nonzero vector to zero, which no invertible matrix can do.

## Final Answer

The inverse is

$$
D^{-1}=\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15 \\
\end{pmatrix}.
$$

The matrix $E$ is not invertible.

## Key Takeaways

- Diagonal matrices can be inverted entry by entry when no diagonal entry is zero.
- A zero diagonal entry makes the matrix singular.
