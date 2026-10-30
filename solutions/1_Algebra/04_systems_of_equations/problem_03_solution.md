# Exercise 3 — Inconsistent System

## Problem Statement

Solve or show that the system is inconsistent:
\[
\begin{cases}
x+2y=3,\\
2x+4y=7.
\end{cases}
\]
Show the contradiction after elimination and interpret it in terms of the equations.

## Objective

Recognize that a system has no solution when elimination produces a false equality.

## Concepts and Formulas

Row operations preserve the solution set. A row \([0\ 0\mid c]\) for \(c\ne0\) represents \(0=c\), which is impossible.

## Step-by-Step Solution

### Step 1 — Form the augmented matrix

\[
\left[\begin{array}{cc|c}
1&2&3\\
2&4&7
\end{array}\right].
\]

### Step 2 — Eliminate the first variable

Apply \(R_2\leftarrow R_2-2R_1\):
\[
\left[\begin{array}{cc|c}
1&2&3\\
0&0&1
\end{array}\right].
\]
The second row says
\[
0x+0y=1,\quad\text{or}\quad 0=1,
\]
which is a contradiction.

### Step 3 — Interpret the contradiction

The left side of the second equation is twice the first equation's left side, but its right side is \(7\), not twice \(3\), which would be \(6\). The equations demand incompatible values for the same expression.

## Verification

If the first equation holds, doubling it forces \(2x+4y=6\); it cannot simultaneously equal \(7\).

## Final Answer

\[
\boxed{\text{The system is inconsistent and has no solution.}}
\]

## Key Takeaways

- A zero row of coefficients with a nonzero right-hand side signals no solution.
- Proportional left-hand sides must have proportionally matching right-hand sides for consistency.