# Exercise 15 — Two Methods for Solving the Same System

## Problem Statement

For

$$
A=\begin{pmatrix}
2&1 \\
1&3 \\
\end{pmatrix},
\qquad
b=\begin{pmatrix}
7 \\
8 \\
\end{pmatrix},
$$

solve $Ax=b$ using (1) $A^{-1}b$ and (2) Gaussian elimination. Compare the methods and identify the simpler one for this example.

## Objective

Solve the same system in two ways and compare the amount of work required.

## Concepts and Formulas

If $A$ is invertible, then $x=A^{-1}b$. Gaussian elimination instead applies row operations to the augmented matrix $[A\mid b]$ to reach an equivalent system that is easy to solve.

## Step-by-Step Solution

### Method 1 — Use the inverse

Calculate the determinant, then use the $2\times2$ inverse formula:

First,

$$
\det(A)=2\cdot3-1\cdot1=5,
\qquad
A^{-1}=\frac15\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}.
$$

Then

$$
x=A^{-1}b
=\frac15\begin{pmatrix}
3&-1 \\
-1&2 \\
\end{pmatrix}
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
=\frac15\begin{pmatrix}
3(7)+(-1)(8) \\
(-1)(7)+2(8) \\
\end{pmatrix}
=\frac15\begin{pmatrix}
21-8 \\
-7+16 \\
\end{pmatrix}
=\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}.
$$

### Method 2 — Gaussian elimination

Write the augmented matrix:

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}.
$$

Swap the two rows, $R_1\leftrightarrow R_2$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}.
$$

Next apply $R_2\leftarrow R_2-2R_1$. The second row becomes
$(2,1\mid7)-2(1,3\mid8)=(0,-5\mid-9)$, so

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}.
$$

Divide the second row by $-5$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & 1 & \mid & \frac95 \\
\end{pmatrix}.
$$

The second row gives

$$
y=\frac95.
$$

Substitute this value into the first row, $x+3y=8$:

$$
x+3\left(\frac95\right)=8
\quad\Longrightarrow\quad
x=8-\frac{27}{5}
=\frac{40}{5}-\frac{27}{5}
=\frac{13}{5}.
$$

## Verification and Comparison

Both methods produce $x=(13/5,9/5)^T$. Check:

$$
2\left(\frac{13}{5}\right)+\frac95=7,\qquad
\frac{13}{5}+3\left(\frac95\right)=8.
$$

For this one small system, elimination is simpler: it avoids constructing the full inverse when only one right-hand side is being solved. If the same $A$ were used with many different right-hand sides, computing reusable information about $A$ could be worthwhile.

## Final Answer

$$
x=\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}.
$$

Both methods agree; Gaussian elimination is simpler in this single-system example.

## Key Takeaways

- Independent methods should lead to the same solution.
- For one small right-hand side, elimination often uses fewer essential calculations than finding a full inverse.
