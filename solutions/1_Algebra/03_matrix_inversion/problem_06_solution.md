# Exercise 6 — Solving a System Using the Inverse

## Problem Statement

Solve $Ax=b$, where

$$
A=\begin{pmatrix}
2&1 \\
1&3 \\
\end{pmatrix},
\qquad
b=\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$, then substitute the result into the equation.

## Objective

Use an inverse matrix to solve a linear system and verify the resulting vector.

## Concepts and Formulas

If $A$ is invertible, multiplying $Ax=b$ on the left by $A^{-1}$ gives

$$
x=A^{-1}b,
$$

because $A^{-1}A=I$.

## Step-by-Step Solution

### Step 1 — Find $A^{-1}$

First compute the determinant:

$$
\det(A)=2\cdot3-1\cdot1=5.
$$

Since the determinant is nonzero, the inverse exists. Swap the diagonal entries, change the signs of the off-diagonal entries, and divide by $5$:

$$
A^{-1}=\frac15\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}.
$$

### Step 2 — Compute $A^{-1}b$

Multiply each row of the inverse by the column vector $b$:

$$
x=A^{-1}b
=\frac15\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
=\frac15\begin{pmatrix}
3(5)+(-1)(7) \\
(-1)(5)+2(7) \\
\end{pmatrix}
=\frac15\begin{pmatrix}
15-7 \\
-5+14 \\
\end{pmatrix}
=\frac15\begin{pmatrix}
8 \\
9 \\
\end{pmatrix}
=\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}.
$$

### Step 3 — Substitute into the original system

Substitute $x_1=\frac85$ and $x_2=\frac95$ into the first equation:

$$
2\left(\frac85\right)+\frac95=\frac{16+9}{5}=5.
$$

Substitute the same values into the second equation:

$$
\frac85+3\left(\frac95\right)=\frac{8+27}{5}=7.
$$

Both equations are satisfied.

## Verification

$$
A\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}
=\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}=b.
$$

## Final Answer

$$
x=\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}.
$$

## Key Takeaways

- The inverse method applies when the coefficient matrix is invertible.
- Substitution in the original system confirms the computed vector.
