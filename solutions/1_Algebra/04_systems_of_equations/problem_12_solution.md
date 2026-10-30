# Exercise 12 — Homogeneous System

## Problem Statement

Solve the homogeneous system

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0. \\
\end{cases}
$$

Give all solutions in parametric form and explain why the zero vector is always a solution of a homogeneous system.

## Objective

Find the complete solution set, recognize a redundant equation, and identify the role of the zero vector.

## Concepts and Formulas

A homogeneous system has the form $Ax=0$. Its zero vector always solves it because $A0=0$. Nonzero solutions may also exist when the equations are dependent.

## Step-by-Step Solution

### Step 1 — Identify the redundant equation

The second equation is exactly twice the first, so it adds no new condition. The independent equations are

$$
x+2y-z=0,\qquad x-y+2z=0.
$$

### Step 2 — Relate the variables

Subtract the second independent equation from the first:

$$
3y-3z=0\quad\Longrightarrow\quad y=z.
$$

Let the free variable $z=t$, so $y=t$. Substitution into $x+2y-z=0$ gives

$$
x+2t-t=0\quad\Longrightarrow\quad x=-t.
$$

### Step 3 — Describe all solutions

$$
(x,y,z)=(-t,t,t),\qquad t\in\mathbb R.
$$

## Verification

For every $t$, the left sides are $-t+2t-t=0$, $2(-t)+4t-2t=0$, and $-t-t+2t=0$. At $t=0$, the solution is $(0,0,0)$, as guaranteed by homogeneity.

## Final Answer

$$
(x,y,z)=t(-1,1,1),\quad t\in\mathbb R.
$$

## Key Takeaways

- The zero vector always solves $Ax=0$, since multiplying any matrix by zero gives zero.
- Dependent equations can leave free variables and therefore nonzero solutions.
