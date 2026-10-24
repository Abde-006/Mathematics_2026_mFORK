## Exercise 3 — When Can Matrices Be Multiplied?

### Problem Statement
The matrix sizes are

$$
A_{2\times3},\quad B_{3\times4},\quad C_{4\times2},\quad D_{2\times2}.
$$

For the products

$$
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA,
$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

### Objective
Determine which matrix products are defined and identify the dimensions of each defined product.

### Concepts and Formulas
For matrices $M_{m\times n}$ and $N_{p\times q}$, the product $MN$ is defined only if

$$
n=p.
$$

If defined, the result has size

$$
m\times q.
$$

This rule is the compatibility condition for matrix multiplication.

### Step-by-Step Solution

#### Step 1 — Check $AB$

$$
A_{2\times3}\cdot B_{3\times4}
$$

Inner dimensions: $3=3$, so the product is defined.
Result size:

$$
2\times4.
$$

#### Step 2 — Check $BA$

$$
B_{3\times4}\cdot A_{2\times3}
$$

Inner dimensions: $4\neq2$, so this product is undefined.

#### Step 3 — Check $BC$

$$
B_{3\times4}\cdot C_{4\times2}
$$

Inner dimensions: $4=4$, so the product is defined.
Result size:

$$
3\times2.
$$

#### Step 4 — Check $CB$

$$
C_{4\times2}\cdot B_{3\times4}
$$

Inner dimensions: $2\neq3$, so this product is undefined.

#### Step 5 — Check $AC$

$$
A_{2\times3}\cdot C_{4\times2}
$$

Inner dimensions: $3\neq4$, so this product is undefined.

#### Step 6 — Check $CA$

$$
C_{4\times2}\cdot A_{2\times3}
$$

Inner dimensions: $2=2$, so the product is defined.
Result size:

$$
4\times3.
$$

#### Step 7 — Check $AD$

$$
A_{2\times3}\cdot D_{2\times2}
$$

Inner dimensions: $3\neq2$, so this product is undefined.

#### Step 8 — Check $DA$

$$
D_{2\times2}\cdot A_{2\times3}
$$

Inner dimensions: $2=2$, so the product is defined.
Result size:

$$
2\times3.
$$

### Final Answer
- $AB$ is defined and has size $2\times4$
- $BA$ is undefined
- $BC$ is defined and has size $3\times2$
- $CB$ is undefined
- $AC$ is undefined
- $CA$ is defined and has size $4\times3$
- $AD$ is undefined
- $DA$ is defined and has size $2\times3$

### Key Takeaways
- Matrix multiplication is not always possible.
- The rule is: the number of columns in the left matrix must equal the number of rows in the right matrix.
- The result size is determined by the outer dimensions.
