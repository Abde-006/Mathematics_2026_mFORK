# Exercise 8 — Inverse of a Transformation

## Problem Statement

The scaling

$$
S=\begin{pmatrix}
2&0 \\
0&\frac12 \\
\end{pmatrix}
$$

doubles the first coordinate and halves the second. Find $S^{-1}$, describe it geometrically, and check the pair of transformations on a vector.

## Objective

Interpret the inverse matrix as the transformation that undoes a given scaling.

## Concepts and Formulas

For a diagonal matrix with nonzero diagonal entries, the inverse is diagonal with the reciprocal entries. The inverse transformation reverses the effect of the original transformation.

## Step-by-Step Solution

### Step 1 — Reverse each coordinate scaling

To undo multiplication of the first coordinate by $2$, multiply it by $1/2$. To undo multiplication of the second coordinate by $1/2$, multiply it by $2$. Hence

$$
S^{-1}=\begin{pmatrix}
\frac12&0 \\
0&2 \\
\end{pmatrix}.
$$

### Step 2 — Check the inverse matrices

$$
SS^{-1}
=\begin{pmatrix}
2&0 \\
0&\frac12 \\
\end{pmatrix}
\begin{pmatrix}
\frac12&0 \\
0&2 \\
\end{pmatrix}
=I_2.
$$

The reverse product is also $I_2$, since both matrices are diagonal.

### Step 3 — Check the action on a vector

For

$$
v=\begin{pmatrix}
2 \\
4 \\
\end{pmatrix}
$$

,

$$
Sv=\begin{pmatrix}
4 \\
2 \\
\end{pmatrix},
\qquad
S^{-1}(Sv)=\begin{pmatrix}
2 \\
4 \\
\end{pmatrix}=v.
$$

## Verification

The vector returns to its original coordinates after applying $S$ and then $S^{-1}$.

## Final Answer

$$
S^{-1}=\begin{pmatrix}
\frac12&0 \\
0&2 \\
\end{pmatrix}.
$$

Geometrically, it halves the first coordinate and doubles the second.

## Key Takeaways

- An inverse transformation undoes the original action.
- For diagonal scaling, take the reciprocal of each nonzero scale factor.
