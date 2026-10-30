# Exercise 12 — Finding Inverses Without Starting from Scratch

## Problem Statement

It is known that

$$
A^{-1}=\begin{pmatrix}
2&-1 \\
-3&2 \\
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$.

## Objective

Use standard inverse properties to compute the requested matrices directly from $A^{-1}$.

## Concepts and Formulas

For invertible $A$ and nonzero scalar $c$,

$$
(cA)^{-1}=\frac1cA^{-1},\qquad
(A^T)^{-1}=(A^{-1})^T,\qquad
(A^2)^{-1}=(A^{-1})^2.
$$

## Step-by-Step Solution

### Step 1 — Compute $(3A)^{-1}$

$$
(3A)^{-1}=\frac13A^{-1}
=\begin{pmatrix}
\frac23&-\frac13 \\
-1&\frac23 \\
\end{pmatrix}.
$$

### Step 2 — Compute $(A^T)^{-1}$

Transpose the known inverse:

$$
(A^T)^{-1}=(A^{-1})^T
=\begin{pmatrix}
2&-3 \\
-1&2 \\
\end{pmatrix}.
$$

### Step 3 — Compute $(A^2)^{-1}$

Reverse the order in the inverse of $AA$; here both factors are $A$, so

$$
(A^2)^{-1}=(A^{-1})^2
=\begin{pmatrix}
2&-1 \\
-3&2 \\
\end{pmatrix}
\begin{pmatrix}
2&-1 \\
-3&2 \\
\end{pmatrix}
=\begin{pmatrix}
7&-4 \\
-12&7 \\
\end{pmatrix}.
$$

## Verification

The properties can be checked by multiplying: $(3A)(\frac13A^{-1})=I$; $(A^T)(A^{-1})^T=(A^{-1}A)^T=I$; and $A^2(A^{-1})^2=A(AA^{-1})A^{-1}=I$.

## Final Answer

$$
(3A)^{-1}=\begin{pmatrix}
\frac23&-\frac13 \\
-1&\frac23 \\
\end{pmatrix},
\quad
(A^T)^{-1}=\begin{pmatrix}
2&-3 \\
-1&2 \\
\end{pmatrix},
\quad
(A^2)^{-1}=\begin{pmatrix}
7&-4 \\
-12&7 \\
\end{pmatrix}.
$$

## Key Takeaways

- Known inverse properties can avoid recomputing a matrix inverse.
- Products reverse order when inverted, even though $A\cdot A$ has the same factors.
