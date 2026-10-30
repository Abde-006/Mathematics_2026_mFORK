# Exercise 2 — Formula for a $2\times2$ Matrix

## Problem Statement

Find the inverse of

$$
A=\begin{pmatrix}
3&2 \\
5&4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix, then check it by multiplication.

## Objective

Apply the determinant criterion and inverse formula, and verify the proposed inverse against the definition.

## Concepts and Formulas

For

$$
M=\begin{pmatrix}
a&b \\
c&d \\
\end{pmatrix}
$$

, if $ad-bc\ne0$, then

$$
M^{-1}=\frac1{ad-bc}\begin{pmatrix}
d&-b \\
-c&a \\
\end{pmatrix}.
$$

## Step-by-Step Solution

### Step 1 — Check invertibility

$$
\det(A)=3\cdot4-2\cdot5=12-10=2.
$$

Since $2\ne0$, $A$ is invertible.

### Step 2 — Apply the formula

Swap the diagonal entries $3,4$, change the signs of the off-diagonal entries $2,5$, and divide by the determinant:

$$
A^{-1}=\frac12\begin{pmatrix}
4&-2 \\
-5&3 \\
\end{pmatrix}
=\begin{pmatrix}
2&-1 \\
-\frac52&\frac32 \\
\end{pmatrix}.
$$

### Step 3 — Verify by multiplication

$$
AA^{-1}=
\begin{pmatrix}
3&2 \\
5&4 \\
\end{pmatrix}
\begin{pmatrix}
2&-1 \\
-\frac52&\frac32 \\
\end{pmatrix}
=\begin{pmatrix}
6-5&-3+3 \\
10-10&-5+6 \\
\end{pmatrix}
=I_2.
$$

## Verification

The product $AA^{-1}$ equals the identity matrix, confirming the calculated inverse.

## Final Answer

$$
A^{-1}=\begin{pmatrix}
2&-1 \\
-\frac52&\frac32 \\
\end{pmatrix}.
$$

## Key Takeaways

- A $2\times2$ matrix is invertible exactly when its determinant is nonzero.
- The formula should be followed by a multiplication check when requested.
