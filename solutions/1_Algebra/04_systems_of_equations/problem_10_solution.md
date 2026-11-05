# Exercise 10 — A Polynomial Through Three Points

## Problem Statement

Find $p(x)=ax^2+bx+c$ passing through $(0,1),(1,3),(2,9)$. Form a system for $a,b,c$ and check all three points.

## Objective

Convert conditions on a polynomial into a linear system for its unknown coefficients.

## Concepts and Formulas

To pass through $(x_0,y_0)$, a polynomial must satisfy $p(x_0)=y_0$. Substituting a fixed input makes the expression linear in the unknown coefficients $a,b,c$.

## Step-by-Step Solution

### Step 1 — Substitute each point

Substitute each input-output pair into $p(x)=ax^2+bx+c$:

- At $(0,1)$: $a(0)^2+b(0)+c=1$, so $c=1$.
- At $(1,3)$: $a+b+c=3$.
- At $(2,9)$: $4a+2b+c=9$.

The resulting system is

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9. \\
\end{cases}
$$

### Step 2 — Solve for the coefficients

From the first equation, $c=1$. Substitute it into the second and third equations:

$$
a+b+1=3\quad\Longrightarrow\quad a+b=2,
$$

$$
4a+2b+1=9\quad\Longrightarrow\quad 4a+2b=8
\quad\Longrightarrow\quad 2a+b=4.
$$

Subtract $a+b=2$ from $2a+b=4$ to get $a=2$. Substitute into $a+b=2$ to obtain $b=0$.

### Step 3 — Write the polynomial

$$
p(x)=2x^2+1.
$$

## Verification

$$
p(0)=1,\qquad p(1)=2+1=3,\qquad p(2)=2(4)+1=9.
$$

It passes through all three points.

## Final Answer

$$
p(x)=2x^2+1.
$$

## Key Takeaways

- Point conditions become equations for the unknown coefficients.
- Verifying each input-output pair checks that the polynomial fits all data.
