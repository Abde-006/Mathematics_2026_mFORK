# Exercise 8 — Two Systems with the Same Coefficient Matrix

## Problem Statement

Solve both systems by elimination and compare the calculations:
\[
\begin{cases}2x+y=5,\\x-y=1,\end{cases}
\qquad
\begin{cases}2x+y=1,\\x-y=4.\end{cases}
\]

## Objective

Identify which elimination steps depend only on the coefficient matrix and which depend on the right-hand side.

## Concepts and Formulas

When systems have the same coefficient matrix, elimination uses the same row operations on the coefficient columns. The right-hand sides change according to those same operations.

## Step-by-Step Solution

### Step 1 — Eliminate \(x\) in the first system

Subtract twice the second equation from the first:
\[
(2x+y)-2(x-y)=5-2(1),
\]
so \(3y=3\), giving \(y=1\). Then \(x-y=1\) gives \(x=2\).

### Step 2 — Eliminate \(x\) in the second system

Use the same combination of left-hand sides:
\[
(2x+y)-2(x-y)=1-2(4),
\]
so \(3y=-7\), giving \(y=-7/3\). Then \(x-y=4\) gives
\[
x=4-\frac73=\frac53.
\]

### Step 3 — Compare the steps

In both systems the coefficient combination is \(3y\), because the coefficient matrix is the same. The resulting right-hand side differs: it is \(3\) in the first system and \(-7\) in the second. Thus the elimination pattern is shared, but the numerical solution changes with the right-hand side.

## Verification

First solution: \(2(2)+1=5\) and \(2-1=1\). Second solution: \(2(5/3)-7/3=1\) and \(5/3-(-7/3)=4\).

## Final Answer

\[
\boxed{\text{System 1: }(x,y)=(2,1)},\qquad
\boxed{\text{System 2: }(x,y)=\left(\frac53,-\frac73\right)}.
\]

## Key Takeaways

- The same coefficient matrix gives the same elimination operations.
- The transformed right-hand side determines the solution for each system.