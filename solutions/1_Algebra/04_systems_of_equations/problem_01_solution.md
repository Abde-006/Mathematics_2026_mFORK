# Exercise 1 — From a System to a Matrix

## Problem Statement

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7 \\
\end{cases}
$$

in the form $Ax=b$. Identify $A$, $x$, and $b$, and explain how the rows correspond to the equations.

## Objective

Translate a linear system into matrix notation by collecting its coefficients, unknowns, and constants.

## Concepts and Formulas

In $Ax=b$, each row of $A$ contains the coefficients of one equation in the same variable order. The vector $x$ lists the unknowns, and $b$ lists the right-hand sides.

## Step-by-Step Solution

### Step 1 — Fix the variable order

Use the order $x,y,z$. The coefficients in the first equation are $2,-1,1$; in the second they are $1,3,-2$; in the third they are $3,1,1$.

### Step 2 — Form the matrices and vectors

$$
A=\begin{pmatrix}
2&-1&1 \\
1&3&-2 \\
3&1&1 \\
\end{pmatrix},
\qquad
x=\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix},
\qquad
b=\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}.
$$

Thus the system is $Ax=b$.

### Step 3 — Match each row to its equation

The first row of $A$ gives $2x-y+z$, which equals the first entry $4$ of $b$. The second row gives $x+3y-2z=1$, and the third gives $3x+y+z=7$.

## Verification

Multiplying the displayed coefficient rows by the variable vector reproduces all three original left-hand sides in order.

## Final Answer

$$

\begin{pmatrix}
2&-1&1 \\
1&3&-2 \\
3&1&1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}
=\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

## Key Takeaways

- Keep one fixed variable order across every equation.
- Row $i$ of the coefficient matrix matches equation $i$.
