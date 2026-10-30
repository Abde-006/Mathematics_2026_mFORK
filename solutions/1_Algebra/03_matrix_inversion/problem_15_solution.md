# Exercise 15 — Two Methods for Solving the Same System

## Problem Statement

For
\[
A=\begin{pmatrix}2&1\\1&3\end{pmatrix},
\qquad
b=\begin{pmatrix}7\\8\end{pmatrix},
\]
solve \(Ax=b\) using (1) \(A^{-1}b\) and (2) Gaussian elimination. Compare the methods and identify the simpler one for this example.

## Objective

Solve the same system in two ways and compare the amount of work required.

## Concepts and Formulas

If \(A\) is invertible, then \(x=A^{-1}b\). Gaussian elimination instead applies row operations to the augmented matrix \([A\mid b]\) to reach an equivalent system that is easy to solve.

## Step-by-Step Solution

### Method 1 — Use the inverse

First,
\[
\det(A)=2\cdot3-1\cdot1=5,
\qquad
A^{-1}=\frac15\begin{pmatrix}3&-1\\-1&2\end{pmatrix}.
\]
Then
\[
x=A^{-1}b
=\frac15\begin{pmatrix}3&-1\\-1&2\end{pmatrix}
\begin{pmatrix}7\\8\end{pmatrix}
=\frac15\begin{pmatrix}21-8\\-7+16\end{pmatrix}
=\begin{pmatrix}\frac{13}{5}\\\frac95\end{pmatrix}.
\]

### Method 2 — Gaussian elimination

Start with the augmented matrix:
\[
\left[\begin{array}{cc|c}
2&1&7\\
1&3&8
\end{array}\right].
\]
Apply \(R_2\leftarrow R_2-\frac12R_1\):
\[
\left[\begin{array}{cc|c}
2&1&7\\
0&\frac52&\frac92
\end{array}\right].
\]
The second row gives
\[
\frac52y=\frac92\quad\Longrightarrow\quad y=\frac95.
\]
Substitute into \(2x+y=7\):
\[
2x+\frac95=7\quad\Longrightarrow\quad2x=\frac{26}{5}
\quad\Longrightarrow\quad x=\frac{13}{5}.
\]

## Verification and Comparison

Both methods produce \(x=(13/5,9/5)^T\). Check:
\[
2\left(\frac{13}{5}\right)+\frac95=7,\qquad
\frac{13}{5}+3\left(\frac95\right)=8.
\]
For this one small system, elimination is simpler: it avoids constructing the full inverse when only one right-hand side is being solved. If the same \(A\) were used with many different right-hand sides, computing reusable information about \(A\) could be worthwhile.

## Final Answer

\[
\boxed{x=\begin{pmatrix}\frac{13}{5}\\\frac95\end{pmatrix}}.
\]
Both methods agree; Gaussian elimination is simpler in this single-system example.

## Key Takeaways

- Independent methods should lead to the same solution.
- For one small right-hand side, elimination often uses fewer essential calculations than finding a full inverse.