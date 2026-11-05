# Exercise 4 — Gauss–Jordan Elimination

## Problem Statement

Find the inverse of

$$
A=\begin{pmatrix}
1&2 \\
3&5 \\
\end{pmatrix}
$$

using Gauss–Jordan elimination. Show the augmented matrices and explain why reducing the left side to the identity produces the inverse on the right.

## Objective

Use elementary row operations to transform $[A\mid I]$ into $[I\mid A^{-1}]$.

## Concepts and Formulas

Each elementary row operation is equivalent to multiplying on the left by an invertible elementary matrix. Applying the same operations to both blocks of $[A\mid I]$, if the left block becomes $I$, the accumulated row-operation matrix $E$ satisfies $EA=I$. Hence $E=A^{-1}$, which is the resulting right block.

## Step-by-Step Solution

### Step 1 — Set up the augmented matrix

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}.
$$

### Step 2 — Eliminate below the first pivot

The first pivot is the $1$ in the upper-left corner. Subtract three times the first row from the second row. On the left this gives $(3,5)-3(1,2)=(0,-1)$; apply the same operation to the right-hand entries:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}.
$$

Multiply the entire second row by $-1$ so its pivot becomes $1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}.
$$

### Step 3 — Eliminate above the second pivot

The second pivot is now $1$. Subtract twice the second row from the first to make the entry above it zero:

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}.
$$

The left block is now $I_2$, so the right block is the inverse.

## Verification

$$
\begin{pmatrix}
1&2 \\
3&5 \\
\end{pmatrix}
\begin{pmatrix}
-5&2 \\
3&-1 \\
\end{pmatrix}
=\begin{pmatrix}
1&0 \\
0&1 \\
\end{pmatrix}.
$$

## Final Answer

$$
A^{-1}=\begin{pmatrix}
-5&2 \\
3&-1 \\
\end{pmatrix}.
$$

## Key Takeaways

- Every row operation must be applied to the entire augmented matrix.
- The right block becomes $A^{-1}$ precisely when the left block becomes $I$.
