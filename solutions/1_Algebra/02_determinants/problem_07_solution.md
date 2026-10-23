# Solution 7 — Using Properties Instead of Recomputing

### Problem Statement
Suppose $A$ is $3\times3$ and $\det A=-4$. Compute $\det(2A)$, $\det(A^T)$, $\det(A^2)$, and $\det(-A)$.

### Objective
Apply determinant properties for scalar multiples, transposes, and products.

### Concepts and Formulas
For an $n\times n$ matrix:

$$
\det(cA)=c^n\det A,\qquad
\det(A^T)=\det A,\qquad
\det(AB)=\det A\,\det B.
$$

### Step-by-Step Solution
Since $A$ is $3\times3$,

$$
\det(2A)=2^3\det A=8(-4)=-32.
$$

Transpose does not change the determinant:

$$
\det(A^T)=\det A=-4.
$$

Using multiplicativity,

$$
\det(A^2)=\det(A)\det(A)=(-4)^2=16.
$$

Finally,

$$
\det(-A)=(-1)^3\det A=-(-4)=4.
$$

### Final Answer

$$
\boxed{\det(2A)=-32,\quad\det(A^T)=-4,\quad\det(A^2)=16,\quad\det(-A)=4.}
$$

### Key Takeaways
- Scaling a $3\times3$ matrix scales its determinant by the cube of the scalar.
- The determinant of a product is the product of the determinants.