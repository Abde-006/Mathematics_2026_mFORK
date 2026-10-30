# Exercise 4 — Infinitely Many Solutions

## Problem Statement

Solve in parametric form:
\[
\begin{cases}
x+y+z=2,\\
2x+2y+2z=4,\\
x-y+z=0.
\end{cases}
\]
Identify a free variable and check one parameter value.

## Objective

Identify a redundant equation, describe infinitely many solutions with a parameter, and verify one solution.

## Concepts and Formulas

A free variable is a variable without a pivot after elimination. Assigning it a parameter gives a parametric description of the solution set.

## Step-by-Step Solution

### Step 1 — Eliminate redundant information

The second equation is exactly twice the first. Subtract \(2\) times row 1 from row 2 in the augmented matrix:
\[
\left[\begin{array}{ccc|c}
1&1&1&2\\
0&0&0&0\\
1&-1&1&0
\end{array}\right].
\]
Now apply \(R_3\leftarrow R_3-R_1\):
\[
\left[\begin{array}{ccc|c}
1&1&1&2\\
0&0&0&0\\
0&-2&0&-2
\end{array}\right].
\]
The third row gives \(y=1\).

### Step 2 — Choose a free variable

Substitute \(y=1\) into the first equation:
\[
x+z=1.
\]
There is no pivot restricting \(z\), so let \(z=t\), where \(t\) is any real number. Then \(x=1-t\).

### Step 3 — State the family of solutions

\[
(x,y,z)=(1-t,1,t),\qquad t\in\mathbb R.
\]

## Verification

Choose \(t=0\), giving \((1,1,0)\). The left-hand sides are \(2\), \(4\), and \(0\), respectively, so all three equations hold.

## Final Answer

\[
\boxed{(x,y,z)=(1-t,1,t),\quad t\in\mathbb R.}
\]
The free variable is \(z=t\).

## Key Takeaways

- A zero row \(0=0\) is redundant and does not constrain the variables.
- One free variable produces a one-parameter family of solutions.