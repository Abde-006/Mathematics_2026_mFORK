# Exercise 11 — Parameter and Invertibility

## Problem Statement

For

$$
A(t)=\begin{pmatrix}
1&t \\
t&1 \\
\end{pmatrix},
$$

find the values of $t$ for which the matrix is invertible, give a formula for its inverse, and explain the excluded values.

## Objective

Use the determinant to determine invertibility as a function of a parameter and express the inverse where it exists.

## Concepts and Formulas

For a $2\times2$ matrix, invertibility is equivalent to a nonzero determinant. The inverse formula divides by that determinant, so it is valid only when the determinant is nonzero.

## Step-by-Step Solution

### Step 1 — Compute the determinant

$$
\det A(t)=1\cdot1-t\cdot t=1-t^2=(1-t)(1+t).
$$

This determinant is zero exactly when $t=1$ or $t=-1$.

### Step 2 — State the invertible parameter values

Therefore $A(t)$ is invertible for every real $t$ except $t=\pm1$.

### Step 3 — Write the inverse

For $t\ne\pm1$, use the $2\times2$ formula:

$$
A(t)^{-1}=\frac1{1-t^2}\begin{pmatrix}
1&-t \\
-t&1 \\
\end{pmatrix}.
$$

### Step 4 — Interpret the excluded values

At $t=1$, both rows are $(1,1)$. At $t=-1$, the rows are $(1,-1)$ and $(-1,1)$, which are negatives. In each case the rows are dependent, and the determinant is zero. The denominator in the inverse formula vanishes because no inverse exists at those values.

## Verification

For $t\ne\pm1$,

$$
A(t)\begin{pmatrix}
1&-t \\
-t&1 \\
\end{pmatrix}
=\begin{pmatrix}
1-t^2&0 \\
0&1-t^2 \\
\end{pmatrix},
$$

so division by $1-t^2$ gives $I_2$.

## Final Answer

The matrix $A(t)$ is invertible exactly when $t\ne\pm1$. For those values,

$$
A(t)^{-1}=\frac1{1-t^2}\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}.
$$

## Key Takeaways

- Parameter values that make the determinant zero must be excluded.
- The inverse formula's denominator signals where the inverse ceases to exist.
