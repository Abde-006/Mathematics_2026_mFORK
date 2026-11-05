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

Subtract the first row from the third row, entry by entry:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & -1 & 1 & \mid & -1 & 0 & 1 \\
\end{pmatrix}.
$$

Add the second row to the third row. On the left, $(0,-1,1)+(0,1,1)=(0,0,2)$; on the right, $(-1,0,1)+(0,1,0)=(-1,1,1)$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 2 & \mid & -1 & 1 & 1 \\
\end{pmatrix}.
$$

Divide the entire third row by $2$ to make its pivot $1$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}.
$$

### Step 3 — Clear the third-column entries above the pivot

Subtract the third row from the second row to eliminate the $1$ above the third-column pivot:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 0 & \mid & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & \mid & -\frac12 & \frac12 & \frac12 \\
\end{pmatrix}.
$$

The first row still has a $1$ in the second column. Subtract the second row from the first:

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
