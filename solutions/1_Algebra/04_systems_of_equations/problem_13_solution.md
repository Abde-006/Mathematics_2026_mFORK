# Exercise 13 — Does Every Equation Add New Information?

## Problem Statement

Solve
\[
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2,
\]
and determine whether all three equations are independently necessary to describe the solution set.

## Objective

Find the solution set and test whether one equation follows from the other two.

## Concepts and Formulas

An equation is redundant if it can be obtained by combining the other equations. A redundant equation does not further restrict the solution set.

## Step-by-Step Solution

### Step 1 — Check whether the third equation follows

Subtract the second equation from the first:
\[
(x_1+x_2)-(x_2+x_3)=10-8
\quad\Longrightarrow\quad x_1-x_3=2.
\]
This is exactly the third equation, so it is redundant.

### Step 2 — Solve the independent equations

Let \(x_2=s\) be free. From the first equation,
\[
x_1=10-s.
\]
From the second,
\[
x_3=8-s.
\]
Therefore all solutions have the form
\[
(x_1,x_2,x_3)=(10-s,s,8-s),\qquad s\in\mathbb R.
\]

## Verification

For every \(s\), \(x_1+x_2=(10-s)+s=10\) and \(x_2+x_3=s+(8-s)=8\). The third left-hand side is
\[
x_1-x_3=(10-s)-(8-s)=2,
\]
as required.

## Final Answer

\[
\boxed{(x_1,x_2,x_3)=(10-s,s,8-s),\quad s\in\mathbb R.}
\]
The third equation follows from the first minus the second and is not independently necessary.

## Key Takeaways

- A linear combination of equations can reveal redundancy.
- Removing a redundant equation does not change the solution set.