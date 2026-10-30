# Exercise 14 — A Small Change in the Right-Hand Side

## Problem Statement

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3 \\
\end{cases}
\qquad\mathrm{and}\qquad
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1. \\
\end{cases}
$$

Check consistency and explain how changing one number affects the system.

## Objective

Determine whether each set of equations is mutually consistent and show how a small right-hand-side change can create a contradiction.

## Concepts and Formulas

Equations that are linear combinations of other equations must have right-hand sides that follow the same combination. Elimination detects a mismatch as a false equation.

## Step-by-Step Solution

### Step 1 — Combine the first two equations

Add $x+y=2$ and $2x-y=1$:

$$
3x=3.
$$

Thus the first two equations force $x=1$, and then $y=1$.

### Step 2 — Test the first system

The third equation is $3x=3$, exactly the equation derived from the first two. Hence the system is consistent, with the unique solution $(1,1)$.

### Step 3 — Test the altered system

The first two equations still force $3x=3$, while the altered third equation requires $3x=3.1$. Subtracting gives $0=0.1$, a contradiction. Therefore the altered system is inconsistent.

## Verification

For the first system, $1+1=2$, $2(1)-1=1$, and $3(1)=3$. No pair $(x,y)$ can satisfy both $3x=3$ and $3x=3.1$, so the second system has no solution.

## Final Answer

The first system is consistent, with solution $(x,y)=(1,1)$.

The second system is inconsistent and has no solution.

## Key Takeaways

- A redundant equation must have a right-hand side consistent with the same linear combination.
- Even a small change can turn an identity into a contradiction.
