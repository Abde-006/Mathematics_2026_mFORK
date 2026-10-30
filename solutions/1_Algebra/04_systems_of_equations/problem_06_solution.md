# Exercise 6 — A System with a Parameter

## Problem Statement

Analyze the system, depending on \(a\):
\[
\begin{cases}
x+y=2,\\
ax+ay=4.
\end{cases}
\]
Determine which cases (one solution, infinitely many solutions, or no solution) occur.

## Objective

Compare the equations as the parameter changes and classify the solution set for every \(a\).

## Concepts and Formulas

The second left-hand side is \(a(x+y)\). Using the first equation, its value must be \(2a\). Consistency requires that value to equal the second right-hand side, \(4\).

## Step-by-Step Solution

### Step 1 — Use the first equation in the second

Since \(x+y=2\), the left side \(ax+ay=a(x+y)=2a\). Therefore the second equation is consistent with the first exactly when
\[
2a=4,\quad\text{so}\quad a=2.
\]

### Step 2 — Analyze \(a=2\)

When \(a=2\), the second equation is \(2x+2y=4\), exactly twice the first. It adds no new information. The system reduces to \(x+y=2\), which has infinitely many solutions:
\[
(x,y)=(2-t,t),\qquad t\in\mathbb R.
\]

### Step 3 — Analyze \(a\ne2\)

If \(a\ne2\), the first equation forces \(ax+ay=2a\ne4\), while the second requires it to equal \(4\). The system is inconsistent and has no solution.

## Verification

At \(a=2\), every vector \((2-t,t)\) sums to \(2\) and satisfies both equations. For \(a\ne2\), the forced value \(2a\) disagrees with \(4\).

## Final Answer

\[
\boxed{\begin{cases}
a=2:&\text{infinitely many solutions},\\
a\ne2:&\text{no solution}.
\end{cases}}
\]
Exactly one solution never occurs.

## Key Takeaways

- The equations have proportional left-hand sides for every \(a\).
- Only when the right-hand sides match the same proportion can the system be consistent.