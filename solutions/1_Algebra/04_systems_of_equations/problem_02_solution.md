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

For row 2, subtract twice row 1: $(2,-1,1\mid3)-2(1,1,1\mid6)=(0,-3,-1\mid-9)$. For row 3, subtract row 1: $(1,2,-1\mid2)-(1,1,1\mid6)=(0,1,-2\mid-4)$.

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}.
$$

Swap rows 2 and 3 so the second pivot is $1$. Then add three times row 2 to row 3: $(0,-3,-1\mid-9)+3(0,1,-2\mid-4)=(0,0,-7\mid-21)$.

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}.
$$

### Step 3 — Back-substitute

Divide the last row by $-7$ to get $z=3$. Substitute $z=3$ into the second row:

$$
y-2(3)=-4\quad\Longrightarrow\quad y-6=-4\quad\Longrightarrow\quad y=2.
$$

Substitute $y=2$ and $z=3$ into the first row:

$$
x+2+3=6\quad\Longrightarrow\quad x+5=6\quad\Longrightarrow\quad x=1.
$$

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
