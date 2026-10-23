# Solution 14 — A System of Equations and the Determinant

### Problem Statement
For $Ax=b$ with

$$
A=\begin{pmatrix}1&2\\k&4\end{pmatrix},
$$

find when there is exactly one solution for every $b$. For the exceptional $k$, give right-hand sides producing infinitely many and no solutions.

### Objective
Connect invertibility with existence and uniqueness for every right-hand side.

### Concepts and Formulas
A square system $Ax=b$ has exactly one solution for every $b$ if and only if $A$ is invertible, equivalently $\det A\ne0$.

### Step-by-Step Solution
Compute

$$
\det A=1\cdot4-2k=4-2k.
$$

This determinant is nonzero when $k\ne2$. For such $k$, $A$ is invertible, so every $b$ gives exactly one solution.

When $k=2$, the second row of $A$ is twice the first, and the equations are

$$
x+2y=b_1,\qquad 2x+4y=b_2.
$$

Choose $b=\begin{pmatrix}1\\2\end{pmatrix}$. The second equation is twice the first, leaving one equation in two unknowns, so there are infinitely many solutions. Choose instead $b=\begin{pmatrix}1\\0\end{pmatrix}$. The equations would require $x+2y=1$ and $2x+4y=0$, which are inconsistent, so there is no solution.

### Final Answer
- Exactly one solution for every $b$ when $\boxed{k\ne2}$.
- For $k=2$, $b=(1,2)^T$ gives infinitely many solutions.
- For $k=2$, $b=(1,0)^T$ gives no solution.

### Key Takeaways
- A nonzero determinant guarantees a unique solution for every right-hand side.
- In the singular case, a system may have infinitely many solutions or none, depending on $b$.