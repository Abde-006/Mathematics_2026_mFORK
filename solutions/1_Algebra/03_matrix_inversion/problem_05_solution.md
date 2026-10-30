# Exercise 5 — A $3\times3$ Matrix

## Problem Statement

Use Gauss–Jordan elimination to find and check the inverse of

$$
A=\begin{pmatrix}
1&1&0 \\
0&1&1 \\
1&0&1 \\
\end{pmatrix}.
$$

## Objective

Extend the augmented-matrix inverse method to a $3\times3$ matrix and verify the result by multiplication.

## Concepts and Formulas

Reduce $[A\mid I_3]$ by elementary row operations. If the left block becomes $I_3$, the right block is $A^{-1}$. A final product $AA^{-1}=I_3$ checks the result.

## Step-by-Step Solution

### Step 1 — Set up the augmented matrix

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
1 & 0 & 1 & \mid & 0 & 0 & 1 \\
\end{pmatrix}.
$$

### Step 2 — Create a pivot in the third column

Apply $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & -1 & 1 & \mid & -1 & 0 & 1 \\
\end{pmatrix}.
$$

Then apply $R_3\leftarrow R_3+R_2$ and $R_3\leftarrow\frac12R_3$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}.
$$

### Step 3 — Clear the third-column entries above the pivot

Apply $R_2\leftarrow R_2-R_3$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 0 & \mid & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}.
$$

Then apply $R_1\leftarrow R_1-R_2$:

$$
\begin{pmatrix}
1 & 0 & 0 & \mid & \frac12 & -\frac12 & \frac12 \\
0 & 1 & 0 & \mid & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}.
$$

### Step 4 — Read off the inverse

$$
A^{-1}=\frac12\begin{pmatrix}
1&-1&1 \\
1&1&-1 \\
-1&1&1 \\
\end{pmatrix}.
$$

## Verification

The product of $A$ with the displayed inverse is

$$
AA^{-1}=\frac12
\begin{pmatrix}
2&0&0 \\
0&2&0 \\
0&0&2 \\
\end{pmatrix}
=I_3.
$$

## Final Answer

$$
A^{-1}=\frac12\begin{pmatrix}
1&-1&1 \\
1&1&-1 \\
-1&1&1 \\
\end{pmatrix}.
$$

## Key Takeaways

- Gauss–Jordan elimination works in the same way for larger square matrices.
- Keeping the identity block attached tracks the row operations needed to form the inverse.
