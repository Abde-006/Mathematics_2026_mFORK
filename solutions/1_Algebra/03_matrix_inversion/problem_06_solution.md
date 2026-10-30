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

$$
\det(A)=2\cdot3-1\cdot1=5.
$$

Using the $2\times2$ inverse formula,

$$
A^{-1}=\frac15\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}.
$$

### Step 2 — Compute $A^{-1}b$

$$
x=\frac15\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
=\frac15\begin{pmatrix}
15-7 \\
-5+14 \\
\end{pmatrix}
=\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}.
$$

### Step 3 — Substitute into the original system

The first row gives $2x_1+x_2$:

$$
2\left(\frac85\right)+\frac95=\frac{16+9}{5}=5.
$$

The second row gives $x_1+3x_2$:

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
