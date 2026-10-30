# Exercise 2 — Gaussian Elimination: One Solution

## Problem Statement

Solve by Gaussian elimination and check the result:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2. \\
\end{cases}
$$

## Objective

Use row operations to reduce the system to an equivalent form that can be solved, then check all equations.

## Concepts and Formulas

An elementary row operation applied to the augmented matrix preserves the solution set. A row such as $[0\ 0\ 0\mid c]$, $c\ne0$, would be a contradiction; a pivot in every variable gives a unique solution.

## Step-by-Step Solution

### Step 1 — Write the augmented matrix

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}.
$$

### Step 2 — Eliminate $x$ from rows 2 and 3

Apply $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}.
$$

Swap rows 2 and 3, then use $R_3\leftarrow R_3+3R_2$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}.
$$

### Step 3 — Back-substitute

The last row gives $z=3$. The second row gives

$$
y-2(3)=-4\quad\Longrightarrow\quad y=2.
$$

The first row gives $x+2+3=6$, so $x=1$.

## Verification

$$
1+2+3=6,\qquad 2(1)-2+3=3,\qquad 1+2(2)-3=2.
$$

All three equations hold.

## Final Answer

$$
(x,y,z)=(1,2,3).
$$

## Key Takeaways

- Elimination creates simpler equivalent equations without changing the solutions.
- Substitute into every original equation to check the result.
