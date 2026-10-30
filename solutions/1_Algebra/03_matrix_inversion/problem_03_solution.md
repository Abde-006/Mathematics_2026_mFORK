# Exercise 3 — When Does the Inverse Not Exist?

## Problem Statement

For

$$
A=\begin{pmatrix}
2&4 \\
1&2 \\
\end{pmatrix},
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

## Objective

Connect the determinant test for invertibility with linear dependence of the rows.

## Concepts and Formulas

A square matrix is invertible exactly when its determinant is nonzero. If the rows are linearly dependent, the determinant is zero and the matrix cannot have an inverse.

## Step-by-Step Solution

### Step 1 — Use the determinant

$$
\det(A)=2\cdot2-4\cdot1=4-4=0.
$$

Therefore $A$ is singular and has no inverse.

### Step 2 — Check the rows

The first row is twice the second:

$$
(2,4)=2(1,2).
$$

Thus the rows are linearly dependent. One row contributes no information beyond the other, so the matrix does not have full rank and cannot be inverted.

## Verification

The determinant test and row-dependence test agree: both identify the same obstruction to invertibility.

## Final Answer

Therefore, $A^{-1}$ does not exist.

Its determinant is zero, and its rows are linearly dependent.

## Key Takeaways

- A zero determinant rules out an inverse.
- Proportional rows are linearly dependent and force a zero determinant.
