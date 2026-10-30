# Exercise 11 — A Parameter in a System of Three Equations

## Problem Statement

Analyze the number of solutions depending on \(t\):
\[
\begin{cases}
x+y+z=1,\\
x+ty+z=2,\\
x+y+tz=3.
\end{cases}
\]
Use elimination and separately examine the parameter value where an elimination step is invalid.

## Objective

Reduce the system while tracking when a parameter-dependent coefficient can or cannot be divided by.

## Concepts and Formulas

Subtracting equations can eliminate common terms. Division by an expression involving a parameter is valid only when that expression is nonzero; its zero case must be analyzed in the original system.

## Step-by-Step Solution

### Step 1 — Eliminate the common terms

Subtract equation 1 from equation 2:
\[
(t-1)y=1.
\]
Subtract equation 1 from equation 3:
\[
(t-1)z=2.
\]

### Step 2 — Analyze \(t\ne1\)

When \(t-1\ne0\), division is valid:
\[
y=\frac1{t-1},\qquad z=\frac2{t-1}.
\]
Using equation 1,
\[
x=1-y-z=1-\frac3{t-1}.
\]
These values determine all variables, so there is exactly one solution:
\[
\left(x,y,z\right)=\left(1-\frac3{t-1},\frac1{t-1},\frac2{t-1}\right).
\]

### Step 3 — Analyze the excluded value \(t=1\)

At \(t=1\), equations 1 and 2 have identical left-hand sides \(x+y+z\) but different right-hand sides \(1\) and \(2\). Subtracting them gives \(0=1\). Equation 3 similarly conflicts with equation 1. Thus the system is inconsistent.

## Verification

For \(t\ne1\), the displayed values satisfy equation 1 because their sum is \(1\). Equations 2 and 3 follow from the differences \((t-1)y=1\) and \((t-1)z=2\). At \(t=1\), the contradiction proves no solution exists.

## Final Answer

\[
\boxed{\begin{cases}
t\ne1:&\text{exactly one solution }
\left(1-\frac3{t-1},\frac1{t-1},\frac2{t-1}\right),\\
t=1:&\text{no solution}.
\end{cases}}
\]

## Key Takeaways

- Always isolate parameter values that make a division step invalid.
- Here the excluded value creates contradictory equations rather than infinitely many solutions.