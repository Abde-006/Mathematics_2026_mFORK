# Exercise 14 — A Matrix That Is Its Own Inverse

## Problem Statement

Assume a square matrix \(A\) satisfies \(A^2=I\). Show that \(A^{-1}=A\), then give a \(2\times2\) example different from \(I\) and \(-I\) and verify it.

## Objective

Use the definition of inverse to prove a general statement and check a concrete example.

## Concepts and Formulas

A matrix \(B\) is the inverse of \(A\) if \(AB=BA=I\). The equation \(A^2=I\) means \(AA=I\).

## Step-by-Step Solution

### Step 1 — Prove the statement

Since \(A^2=I\), we have \(AA=I\). The two factors are both \(A\), so also \(AA=I\) in the reverse order. Thus \(A\) satisfies the defining condition for its own inverse:
\[
A^{-1}=A.
\]

### Step 2 — Choose an example

Consider the matrix that swaps the two coordinates:
\[
A=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
\]
It is different from \(I_2\) and \(-I_2\).

### Step 3 — Verify the example

\[
A^2=
\begin{pmatrix}0&1\\1&0\end{pmatrix}
\begin{pmatrix}0&1\\1&0\end{pmatrix}
=\begin{pmatrix}1&0\\0&1\end{pmatrix}=I_2.
\]

## Verification

The multiplication gives \(A^2=I_2\); hence this example is its own inverse by the definition.

## Final Answer

\[
\boxed{A^2=I\implies A^{-1}=A};
\qquad
\boxed{\begin{pmatrix}0&1\\1&0\end{pmatrix}^{-1}
=\begin{pmatrix}0&1\\1&0\end{pmatrix}}.
\]

## Key Takeaways

- A matrix whose square is the identity is its own inverse.
- Coordinate-swap transformation applied twice restores the original vector.