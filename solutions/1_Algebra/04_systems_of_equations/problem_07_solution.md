# Exercise 7 — Choosing a Method Deliberately

## Problem Statement

Choose and justify a suitable method for each situation:

1. Solve the triangular system \(2x-y=3,\;4y=8\).
2. Plan how to solve three systems \(Ax=b_i\) when the same invertible \(A\) is used and \(A^{-1}\) is already known.
3. Plan how to solve one \(3\times3\) system when \(A^{-1}\) is not given and only one solution vector is needed.

## Objective

Choose a solution strategy based on matrix structure, whether an inverse is available, and how many right-hand sides must be solved.

## Concepts and Formulas

- A triangular system is efficiently solved by back-substitution.
- If \(A^{-1}\) is known, each system \(Ax=b_i\) can be solved as \(x_i=A^{-1}b_i\).
- For one right-hand side, Gaussian elimination usually avoids the extra work of constructing a full inverse.

## Step-by-Step Solution

### Case 1 — Use back-substitution

The second equation directly gives \(4y=8\), hence \(y=2\). Substitute into the first:
\[
2x-2=3\quad\Longrightarrow\quad 2x=5\quad\Longrightarrow\quad x=\frac52.
\]
Thus the solution is \((x,y)=(5/2,2)\).

### Case 2 — Reuse the known inverse

For each right-hand side \(b_i\), compute
\[
x_i=A^{-1}b_i.
\]
The inverse is already available, so the same matrix \(A^{-1}\) is reused three times; only the matrix-vector multiplication changes. If \(A^{-1}\) had to be computed, that one-time cost could be shared across all three systems.

### Case 3 — Eliminate for the one requested vector

Form \([A\mid b]\) and use Gaussian elimination to solve the system directly. Because only one right-hand side is involved and the inverse is not supplied, calculating all of \(A^{-1}\) would generally do unnecessary work.

## Verification

For Case 1, substitution gives \(2(5/2)-2=3\) and \(4(2)=8\). Cases 2 and 3 are method plans as requested, not specific systems to calculate.

## Final Answer

- Case 1: back-substitution gives \(\boxed{(x,y)=(5/2,2)}\).
- Case 2: reuse the known inverse and compute \(A^{-1}b_i\) for each right-hand side.
- Case 3: use Gaussian elimination on \([A\mid b]\) to find the single requested solution.

## Key Takeaways

- Triangular structure makes back-substitution natural.
- Reuse a known inverse when the same matrix serves multiple right-hand sides.
- Avoid finding a full inverse when elimination directly answers a single-system question.