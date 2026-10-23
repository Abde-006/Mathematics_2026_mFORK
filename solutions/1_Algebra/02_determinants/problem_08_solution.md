# Solution 8 — Determinant of a Product

### Problem Statement
For square matrices $A,B$ with $\det A=3$ and $\det B=-5$, compute $\det(AB)$, $\det(BA)$, and $\det(A^{-1}B)$ when defined.

### Objective
Use determinant multiplicativity and the determinant of an inverse.

### Concepts and Formulas

$$
\det(XY)=\det X\,\det Y,\qquad
\det(X^{-1})=\frac{1}{\det X}\quad\text{if }X\text{ is invertible}.
$$

### Step-by-Step Solution
For the product in either order,

$$
\det(AB)=\det A\det B=3(-5)=-15,
$$

$$
\det(BA)=\det B\det A=(-5)3=-15.
$$

Because $\det A=3\ne0$, $A^{-1}$ exists. Therefore,

$$
\det(A^{-1}B)=\det(A^{-1})\det B
=\frac{1}{3}(-5)=-\frac53.
$$

The first two determinant values are equal because real-number multiplication is commutative, even though the matrices $AB$ and $BA$ need not be equal.

### Final Answer

$$
\boxed{\det(AB)=-15,\quad\det(BA)=-15,\quad\det(A^{-1}B)=-\frac53.}
$$

### Key Takeaways
- Determinants of matrix products multiply, regardless of the order of the scalar factors.
- The equality of the two determinant values does not imply $AB=BA$.