# Solution 6 — Parameter and Invertibility

### Problem Statement
For

$$
A(t)=\begin{pmatrix}t&1\\2&t\end{pmatrix},
$$

find all values of $t$ for which $A(t)$ is not invertible.

### Objective
Determine the singular parameter values from the determinant.

### Concepts and Formulas
A square matrix is not invertible exactly when its determinant is zero.

### Step-by-Step Solution
Compute the determinant:

$$
\det A(t)=t\cdot t-1\cdot2=t^2-2.
$$

Set it equal to zero:

$$
t^2-2=0
\quad\Longleftrightarrow\quad
t^2=2
\quad\Longleftrightarrow\quad
t=\pm\sqrt2.
$$

### Final Answer
The matrix is not invertible when

$$
\boxed{t=\sqrt2\text{ or }t=-\sqrt2}.
$$

At exactly these values its determinant is zero; for all other real $t$, it is invertible.

### Key Takeaways
- To find singular values in a parameterized square matrix, solve $\det A(t)=0$.