# Exercise 13 — Undoing a Composite Transformation

## Problem Statement

Let
\[
S=\begin{pmatrix}2&0\\0&1\end{pmatrix},
\qquad
H=\begin{pmatrix}1&1\\0&1\end{pmatrix},
\qquad T=HS.
\]
Find \(T^{-1}\) by computing \(T\) first and by using the product rule. Also compute \(H^{-1}S^{-1}\) and explain why it is the wrong order.

## Objective

Practice reversing the order of factors when finding the inverse of a composite transformation.

## Concepts and Formulas

For invertible \(H,S\),
\[
(HS)^{-1}=S^{-1}H^{-1}.
\]
The rightmost matrix acts first, so undoing a composite map requires reversing the action order.

## Step-by-Step Solution

### Step 1 — Compute \(T=HS\)

\[
T=\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}2&0\\0&1\end{pmatrix}
=\begin{pmatrix}2&1\\0&1\end{pmatrix}.
\]
Its determinant is \(2\), so it is invertible. Applying the \(2\times2\) formula,
\[
T^{-1}=\frac12\begin{pmatrix}1&-1\\0&2\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}.
\]

### Step 2 — Use the inverse product rule

\[
S^{-1}=\begin{pmatrix}\frac12&0\\0&1\end{pmatrix},
\qquad
H^{-1}=\begin{pmatrix}1&-1\\0&1\end{pmatrix}.
\]
Therefore
\[
S^{-1}H^{-1}
=\begin{pmatrix}\frac12&0\\0&1\end{pmatrix}
\begin{pmatrix}1&-1\\0&1\end{pmatrix}
=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix},
\]
agreeing with Step 1.

### Step 3 — Test the unreversed order

\[
H^{-1}S^{-1}
=\begin{pmatrix}1&-1\\0&1\end{pmatrix}
\begin{pmatrix}\frac12&0\\0&1\end{pmatrix}
=\begin{pmatrix}\frac12&-1\\0&1\end{pmatrix}.
\]
This is different from \(T^{-1}\). In \(T=HS\), \(S\) acts first and \(H\) acts second. Undo \(H\) first, then \(S\), which is the product \(S^{-1}H^{-1}\).

## Verification

The two correct methods produce the same inverse. Reversing the product as \(H^{-1}S^{-1}\) gives a different matrix, confirming that order matters.

## Final Answer

\[
\boxed{T^{-1}=S^{-1}H^{-1}=\begin{pmatrix}\frac12&-\frac12\\0&1\end{pmatrix}},
\qquad
\boxed{H^{-1}S^{-1}=\begin{pmatrix}\frac12&-1\\0&1\end{pmatrix}\ne T^{-1}}.
\]

## Key Takeaways

- A composite transformation is undone from the last operation to the first.
- The inverse of a product is the reversed product of the inverses.