# Exercise 1 — Definition of the Inverse

## Problem Statement

Given

$$
A=\begin{pmatrix}
2&1 \\
1&1 \\
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1&-1 \\
-1&2 \\
\end{pmatrix},
$$

check directly, without using an inverse formula, whether $B=A^{-1}$. Compute $AB$ and $BA$.

## Objective

Use the definition of a matrix inverse and verify both multiplication orders.

## Concepts and Formulas

A square matrix $B$ is the inverse of $A$ when

$$
AB=BA=I,
$$

where $I$ is the identity matrix of the same size. Matrix multiplication is generally order-dependent, so checking only one order is not the definition's full direct test.

## Step-by-Step Solution

### Step 1 — Compute $AB$

$$
AB=
\begin{pmatrix}
2&1 \\
1&1 \\
\end{pmatrix}
\begin{pmatrix}
1&-1 \\
-1&2 \\
\end{pmatrix}
=\begin{pmatrix}
2(1)+1(-1)&2(-1)+1(2) \\
1(1)+1(-1)&1(-1)+1(2) \\
\end{pmatrix}
=\begin{pmatrix}
1&0 \\
0&1 \\
\end{pmatrix}.
$$

### Step 2 — Compute $BA$

$$
BA=
\begin{pmatrix}
1&-1 \\
-1&2 \\
\end{pmatrix}
\begin{pmatrix}
2&1 \\
1&1 \\
\end{pmatrix}
=\begin{pmatrix}
1(2)+(-1)(1)&1(1)+(-1)(1) \\
(-1)(2)+2(1)&(-1)(1)+2(1) \\
\end{pmatrix}
=\begin{pmatrix}
1&0 \\
0&1 \\
\end{pmatrix}.
$$

### Step 3 — Compare with the definition

Both products equal $I_2$, the $2\times2$ identity matrix. Thus $B$ undoes multiplication by $A$ on either side.

## Verification

The explicit products above each have ones on the diagonal and zeros elsewhere, exactly as required for $I_2$.

## Final Answer

$$
B=A^{-1}=\begin{pmatrix}
1&-1 \\
-1&2 \\
\end{pmatrix}.
$$

## Key Takeaways

- The definition of an inverse is checked by multiplying and obtaining the identity.
- The order of multiplication matters; both products were checked here.
