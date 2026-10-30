# Exercise 7 — Inverse of a Product

## Problem Statement

For

$$
A=\begin{pmatrix}
1&1 \\
0&1 \\
\end{pmatrix},
\qquad
B=\begin{pmatrix}
2&0 \\
0&3 \\
\end{pmatrix},
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$, compare them, and explain why the order is reversed.

## Objective

Verify the inverse-of-a-product rule with concrete matrices and understand the order reversal.

## Concepts and Formulas

For invertible matrices $A,B$,

$$
(AB)^{-1}=B^{-1}A^{-1}.
$$

The reversal is necessary because $B$ acts first on a vector when the product $AB$ acts: $ABv=A(Bv)$.

## Step-by-Step Solution

### Step 1 — Multiply $A$ and $B$

$$
AB=\begin{pmatrix}
1&1 \\
0&1 \\
\end{pmatrix}
\begin{pmatrix}
2&0 \\
0&3 \\
\end{pmatrix}
=\begin{pmatrix}
2&3 \\
0&3 \\
\end{pmatrix}.
$$

### Step 2 — Invert the product

The determinant of $AB$ is $2\cdot3=6$. Therefore

$$
(AB)^{-1}
=\frac16\begin{pmatrix}
3&-3 \\
0&2 \\
\end{pmatrix}
=\begin{pmatrix}
\frac12&-\frac12 \\
0&\frac13 \\
\end{pmatrix}.
$$

### Step 3 — Compute the reversed product

$$
A^{-1}=\begin{pmatrix}
1&-1 \\
0&1 \\
\end{pmatrix},
\qquad
B^{-1}=\begin{pmatrix}
\frac12&0 \\
0&\frac13 \\
\end{pmatrix}.
$$

Thus

$$
B^{-1}A^{-1}
=\begin{pmatrix}
\frac12&0 \\
0&\frac13 \\
\end{pmatrix}
\begin{pmatrix}
1&-1 \\
0&1 \\
\end{pmatrix}
=\begin{pmatrix}
\frac12&-\frac12 \\
0&\frac13 \\
\end{pmatrix}.
$$

This matches the inverse found in Step 2.

### Step 4 — Explain why the order reverses

$$
(AB)(B^{-1}A^{-1})
=A(BB^{-1})A^{-1}
=AIA^{-1}=I.
$$

The middle factors $B$ and $B^{-1}$ cancel first, followed by $A$ and $A^{-1}$.

## Verification

The two computed matrices are equal, and the factor cancellation proves their product with $AB$ is the identity.

## Final Answer

$$
(AB)^{-1}=B^{-1}A^{-1}
=\begin{pmatrix}
\frac12&-\frac12 \\
0&\frac13 \\
\end{pmatrix}.
$$

## Key Takeaways

- The inverse of a product is the product of the inverses in reverse order.
- To undo a sequence of transformations, undo the last operation first.
