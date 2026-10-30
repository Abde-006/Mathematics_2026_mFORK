# Exercise 9 — Matrix Equation

## Problem Statement

Given

$$
A=\begin{pmatrix}
1&2 \\
0&1 \\
\end{pmatrix},
\qquad
B=\begin{pmatrix}
3&1 \\
2&4 \\
\end{pmatrix},
$$

solve $AX=B$. Decide which side to use for $A^{-1}$, then check by computing $AX$.

## Objective

Solve a matrix equation while respecting multiplication order.

## Concepts and Formulas

To isolate $X$ in $AX=B$, multiply both sides on the **left** by $A^{-1}$:

$$
A^{-1}(AX)=A^{-1}B\quad\Longrightarrow\quad X=A^{-1}B.
$$

Matrix multiplication is not generally commutative, so the inverse must be applied on the side adjacent to $A$.

## Step-by-Step Solution

### Step 1 — Find $A^{-1}$

Since $A$ is upper triangular with diagonal entries $1,1$,

$$
A^{-1}=\begin{pmatrix}
1&-2 \\
0&1 \\
\end{pmatrix};
\quad AA^{-1}=I_2.
$$

### Step 2 — Multiply on the left

$$
X=A^{-1}B
=\begin{pmatrix}
1&-2 \\
0&1 \\
\end{pmatrix}
\begin{pmatrix}
3&1 \\
2&4 \\
\end{pmatrix}
=\begin{pmatrix}
-1&-7 \\
2&4 \\
\end{pmatrix}.
$$

### Step 3 — Check in the original equation

$$
AX=
\begin{pmatrix}
1&2 \\
0&1 \\
\end{pmatrix}
\begin{pmatrix}
-1&-7 \\
2&4 \\
\end{pmatrix}
=\begin{pmatrix}
3&1 \\
2&4 \\
\end{pmatrix}=B.
$$

## Verification

The product $AX$ equals the given matrix $B$, so the equation is satisfied.

## Final Answer

$$
X=\begin{pmatrix}
-1&-7 \\
2&4 \\
\end{pmatrix}.
$$

## Key Takeaways

- In $AX=B$, multiply by $A^{-1}$ on the left.
- Preserve the order of factors when solving matrix equations.
