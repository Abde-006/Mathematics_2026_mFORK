# Exercise 5 — Row Echelon Form and Number of Solutions

## Problem Statement

For the augmented matrix

$$
\begin{pmatrix}
1&2&-1&\mid&3 \\
0&1&2&\mid&1 \\
0&0&0&\mid&0 \\
\end{pmatrix},
$$

determine the number of solutions and write them parametrically. Explain which variables are free.

## Objective

Read pivots and free variables directly from row echelon form.

## Concepts and Formulas

A pivot column corresponds to a leading variable. A variable whose column has no pivot is free. A consistent system with at least one free variable has infinitely many solutions.

## Step-by-Step Solution

### Step 1 — Translate each nonzero row into an equation

The first two rows give

$$
x+2y-z=3,\qquad y+2z=1.
$$

The last row is $0=0$, so it adds no constraint and does not cause a contradiction.

### Step 2 — Identify the free variable

There are pivots in the $x$- and $y$-columns, but none in the $z$-column. Thus $z$ is free. Set $z=t$, for any real $t$.

### Step 3 — Solve for the pivot variables

From the second equation,

$$
y+2t=1\quad\Longrightarrow\quad y=1-2t.
$$

From the first equation,

$$
x+2(1-2t)-t=3
\quad\Longrightarrow\quad x=1+5t.
$$

## Verification

Substitution gives $y+2z=(1-2t)+2t=1$, and $x+2y-z=(1+5t)+2(1-2t)-t=3$, for every $t$.

## Final Answer

$$
(x,y,z)=(1+5t,\,1-2t,\,t),\quad t\in\mathbb R.
$$

There are infinitely many solutions because the consistent system has one free variable.

## Key Takeaways

- Pivot columns determine leading variables; nonpivot columns determine free variables.
- A zero row $0=0$ is consistent but contributes no new condition.
