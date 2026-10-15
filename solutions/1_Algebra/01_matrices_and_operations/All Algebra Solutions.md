# My Solutions — 

This workbook records the solutions, reasoning, and checks for each exercise.

## Solution Method

Each exercise is approached by:

- identifying the requested result,
- applying the relevant matrix rule,
- showing the calculations,
- checking the result, and
- summarizing the main idea.

The solutions include both final answers and supporting reasoning.

## Exercise 1 — Matrix Size and Entries

### Problem Statement
Given

$$
A=\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5 \\
\end{pmatrix},\qquad
B=\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$.
3. Write the second row of $A$ and the first column of $B$ as vectors.

### Objective
Identify the matrix dimensions, interpret entry indices, and express selected rows and columns as vectors.

### Concepts and Formulas
- A matrix of size $m\times n$ has $m$ rows and $n$ columns.
- The entry $a_{ij}$ means the element in row $i$, column $j$.
- A row vector has one row and several columns.
- A column vector has several rows and one column.

### Step-by-Step Solution

#### Step 1 — Determine the matrix sizes
Matrix $A$ has 2 rows and 3 columns, so its size is $2\times 3$.

Matrix $B$ has 3 rows and 2 columns, so its size is $3\times 2$.

This is the standard meaning of size: the first number is rows, the second is columns.

#### Step 2 — Read individual entries
For matrix $A$:

$$
A=
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5 \\
\end{pmatrix}
$$

- $a_{12}$ means row 1, column 2, so

$$
a_{12}=-1.
$$

- $a_{23}$ means row 2, column 3, so

$$
a_{23}=5.
$$

For matrix $B$:

$$
B=
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1 \\
\end{pmatrix}
$$

- $b_{21}$ means row 2, column 1, so

$$
b_{21}=-2.
$$

- $b_{32}$ means row 3, column 2, so

$$
b_{32}=1.
$$

#### Step 3 — Write a row and a column as vectors
The second row of $A$ is

$$
[0\quad 4\quad 5].
$$

This is a row vector.

The first column of $B$ is

$$
\begin{pmatrix}
1 \\
-2 \\
4 \\
\end{pmatrix}.
$$

This is a column vector.

### Verification
We can check the positions:
- In $A$, row 2 is $(0,4,5)$, which matches the second row.
- In $B$, the first column is indeed $(1,-2,4)^T$.

### Final Answer
- $A$ is $2\times 3$ and $B$ is $3\times 2$.
- $a_{12}=-1$, $a_{23}=5$, $b_{21}=-2$, $b_{32}=1$.
- Second row of $A$: $[0\ 4\ 5]$.
- First column of $B$: $(1,-2,4)^T$.

### Key Takeaways
- The size of a matrix is always written as rows $\times$ columns.
- Index notation tells us exactly where an entry sits.
- Rows and columns are not interchangeable: they have different shapes and meanings.

---

## Exercise 2 — Addition and Scalar Multiplication

### Problem Statement
For

$$
A=\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix},
$$

compute

$$
A+B,\quad A-B,\quad 3A-2B.
$$

Explain why matrix addition is possible only for matrices of the same size.

### Objective
Compute the matrix sums and differences entry by entry, and explain why the matrices must have matching dimensions.

### Concepts and Formulas
- Matrix addition: add corresponding entries.
- Matrix subtraction: subtract corresponding entries.
- Scalar multiplication: multiply every entry by the scalar.
- If matrices are the same size, then each entry has a matching partner.

### Step-by-Step Solution

#### Step 1 — Compute $A+B$

$$
A+B=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}+
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
= \begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}
= \begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}.
$$

We add the entries in the same positions.

#### Step 2 — Compute $A-B$

$$
A-B=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}-
\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}
= \begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}
= \begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}.
$$

Subtraction is done entry by entry, just like addition.

#### Step 3 — Compute $3A-2B$
First multiply each matrix by its scalar:

$$
3A = 3\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix},
$$

$$
2B = 2\begin{pmatrix}
4 & -2 \\
0 & 5 \\
\end{pmatrix}=
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}.
$$

Subtract the scaled matrices:

$$
3A-2B=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix}-
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}
= \begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}
= \begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

#### Step 4 — Why same-size matrices are required
Matrix addition is defined only when both matrices have the same dimensions. Why? Because each entry in one matrix must be paired with the corresponding entry in the other matrix.

If one matrix were $2\times 2$ and the other $2\times 3$, there would be no entry in the third column of the second matrix to match the third column of the first. So the operation would not be well defined.

### Final Answer

$$
A+B=\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix},
$$

$$
A-B=\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix},
$$

$$
3A-2B=\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

### Key Takeaways
- Addition and subtraction are done entry by entry.
- Scalar multiplication scales each entry separately.
- Same-size matrices are necessary so the entries line up one-to-one.

---

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

---

## Exercise 4 — Matrix Multiplication and Noncommutativity

### Problem Statement
For

$$
A=\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix},
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

### Objective
Compute the products in both orders and compare the results.

### Concepts and Formulas
- Matrix multiplication is computed by taking dot products of rows of the first matrix with columns of the second matrix.
- In general, $AB\ne BA$ for matrices.
- This is called noncommutativity.

### Step-by-Step Solution

#### Step 1 — Compute $AB$

$$
AB=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Take row 1 of $A$ and column 1 of $B$:

$$
1\cdot2+2\cdot3=2+6=8.
$$

Take row 1 of $A$ and column 2 of $B$:

$$
1\cdot0+2\cdot1=0+2=2.
$$

Take row 2 of $A$ and column 1 of $B$:

$$
0\cdot2+1\cdot3=3.
$$

Take row 2 of $A$ and column 2 of $B$:

$$
0\cdot0+1\cdot1=1.
$$

Therefore,

$$
AB=\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $BA$

$$
BA=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}.
$$

Take row 1 of $B$ with column 1 of $A$:

$$
2\cdot1+0\cdot0=2.
$$

Take row 1 of $B$ with column 2 of $A$:

$$
2\cdot2+0\cdot1=4.
$$

Take row 2 of $B$ with column 1 of $A$:

$$
3\cdot1+1\cdot0=3.
$$

Take row 2 of $B$ with column 2 of $A$:

$$
3\cdot2+1\cdot1=7.
$$

So,

$$
BA=\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}.
$$

#### Step 3 — Compare the results

$$
AB=\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix},\qquad BA=\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}.
$$

Since

$$
AB\ne BA,
$$

matrix multiplication is not commutative.

### Final Answer

$$
AB=\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix},\qquad BA=\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix},
$$

so $AB\ne BA$.

### Key Takeaways
- For matrices, the order of multiplication matters.
- In ordinary arithmetic, $xy=yx$, but for matrices this is often false.
- This is why we must be very careful with the order of matrix products.

---

## Exercise 5 — Matrix Times Vector

### Problem Statement
Let

$$
A=\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},\qquad x=\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

### Objective
Compute the matrix-vector product and express it as a linear combination of the matrix columns.

### Concepts and Formulas
- A matrix-vector product uses the rows of the matrix and the entries of the vector.
- If

$$
A=[c_1\ c_2],
$$

then

$$
Ax=x_1c_1+x_2c_2.
$$

This means the vector $x$ tells us how much of each column to take.

### Step-by-Step Solution

#### Step 1 — Compute $Ax$

$$
Ax=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Compute each entry:
- First entry: $2\cdot4+(-1)\cdot2=8-2=6$
- Second entry: $1\cdot4+3\cdot2=4+6=10$

Therefore,

$$
Ax=\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

#### Step 2 — Express it as a linear combination of the columns
The columns of $A$ are

$$
c_1=\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},\qquad c_2=\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}.
$$

The vector $x$ is

$$
x=\begin{pmatrix}
4 \\
2 \\
\end{pmatrix},
$$

so the linear combination is

$$
4c_1+2c_2.
$$

Compute it:

$$
4\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}+2\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
= \begin{pmatrix}
8 \\
4 \\
\end{pmatrix}+
\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
= \begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

This matches the matrix-vector product.

### Final Answer

$$
Ax=\begin{pmatrix}
6 \\
10 \\
\end{pmatrix},
$$

and

$$
Ax=4\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}+2\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}.
$$

### Key Takeaways
- Multiplying a matrix by a vector is a structured way of combining the columns of the matrix.
- The entries of the vector act as coefficients in a linear combination.
- This idea is fundamental in linear algebra.

---

## Exercise 6 — Transpose

### Problem Statement
For

$$
A=\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

### Objective
Compute the transposes and the product $AB$, then verify the transpose identity.

### Concepts and Formulas
- The transpose of a matrix swaps rows and columns.
- If $A$ has size $m\times n$, then $A^T$ has size $n\times m$.
- For compatible matrices,

$$
(AB)^T=B^TA^T.
$$

### Step-by-Step Solution

#### Step 1 — Compute $A^T$

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

so

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $B^T$

$$
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

so

$$
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}.
$$

#### Step 3 — Compute $AB$
Since $A$ is $2\times3$ and $B$ is $3\times2$, their product is defined and has size $2\times2$.

$$
AB=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}.
$$

Compute entry by entry:
- First row, first column:

$$
1\cdot1+2\cdot2+3\cdot(-1)=1+4-3=2.
$$

- First row, second column:

$$
1\cdot0+2\cdot1+3\cdot3=0+2+9=11.
$$

- Second row, first column:

$$
4\cdot1+5\cdot2+6\cdot(-1)=4+10-6=8.
$$

- Second row, second column:

$$
4\cdot0+5\cdot1+6\cdot3=0+5+18=23.
$$

Hence,

$$
AB=\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}.
$$

#### Step 4 — Compute $(AB)^T$
Taking the transpose of the result:

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}.
$$

#### Step 5 — Compute $B^TA^T$

$$
B^TA^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}.
$$

Compute each entry:
- First row, first col:

$$
1\cdot1+2\cdot2+(-1)\cdot3=1+4-3=2.
$$

- First row, second col:

$$
1\cdot4+2\cdot5+(-1)\cdot6=4+10-6=8.
$$

- Second row, first col:

$$
0\cdot1+1\cdot2+3\cdot3=2+9=11.
$$

- Second row, second col:

$$
0\cdot4+1\cdot5+3\cdot6=5+18=23.
$$

Thus,

$$
B^TA^T=\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}.
$$

This is exactly the same as $(AB)^T$.

### Final Answer

$$
A^T=\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix},\qquad B^T=\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix},
$$

$$
AB=\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix},
$$

and

$$
(AB)^T=B^TA^T=\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}.
$$

### Key Takeaways
- Transposing swaps rows and columns.
- The transpose reverses the order of multiplication: $(AB)^T=B^TA^T$.
- This identity is important because it preserves structure while changing the order of factors.

---

## Exercise 7 — Identity Matrix, Zero Matrix, and Powers

### Problem Statement
For

$$
A=\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix},
$$

compute

$$
AI,\quad IA,\quad A+0,\quad A^2,\quad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

### Objective
Verify the roles of the identity and zero matrices, and identify the pattern in successive powers of $A$.

### Concepts and Formulas
- The identity matrix $I$ satisfies $AI=IA=A$.
- The zero matrix $0$ satisfies $A+0=A$.
- Matrix powers mean repeated multiplication, e.g. $A^2=A\cdot A$.

### Step-by-Step Solution

#### Step 1 — Identify the identity and zero matrices
For a $2\times2$ matrix,

$$
I=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad 0=\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $AI$ and $IA$

$$
AI=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}=A.
$$

$$
IA=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}=A.
$$

This shows that $I$ acts like the multiplicative identity in matrix algebra.

#### Step 3 — Compute $A+0$

$$
A+0=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}+
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}=A.
$$

This shows that the zero matrix acts like the additive identity.

#### Step 4 — Compute $A^2$

$$
A^2=A\cdot A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}.
$$

Compute each entry:
- top-left: $2\cdot2+1\cdot0=4$
- top-right: $2\cdot1+1\cdot2=2+2=4$
- bottom-left: $0\cdot2+2\cdot0=0$
- bottom-right: $0\cdot1+2\cdot2=4$
Thus,

$$
A^2=\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}.
$$

#### Step 5 — Compute $A^3$

$$
A^3=A^2A=
\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}.
$$

Compute:
- top-left: $4\cdot2+4\cdot0=8$
- top-right: $4\cdot1+4\cdot2=4+8=12$
- bottom-left: $0\cdot2+4\cdot0=0$
- bottom-right: $0\cdot1+4\cdot2=8$
Hence,

$$
A^3=\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

#### Step 6 — Observe the pattern
The powers are:

$$
A=\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix},
$$

$$
A^2=\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix},
$$

$$
A^3=\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

A pattern emerges:

$$
A^n=\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

This is because the matrix has the form

$$
A=2I+N,\quad N=\begin{pmatrix}
0 & 1 \\
0 & 0 \\
\end{pmatrix},\quad N^2=0,
$$

which leads to a predictable power pattern.

### Final Answer

$$
AI=A,\qquad IA=A,\qquad A+0=A,
$$

$$
A^2=\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix},\qquad A^3=\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

The general pattern is

$$
A^n=\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

### Key Takeaways
- The identity matrix behaves like the number $1$ for multiplication.
- The zero matrix behaves like the number $0$ for addition.
- Repeated multiplication can reveal a clear pattern, especially in triangular matrices.

---

## Exercise 8 — Row Operations and Their Reversibility

### Problem Statement
For

$$
A=\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix},
$$

perform, in order:
1. $R_2\leftarrow R_2-2R_1$
2. $R_3\leftarrow R_3+R_1$
3. interchange $R_2$ and $R_3$

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

### Objective
Apply the elementary row operations and identify the inverse of each operation.

### Concepts and Formulas
Elementary row operations:
- replace a row by a multiple of itself plus a multiple of another row,
- add a multiple of one row to another,
- swap two rows.

Each of these operations is reversible, which is why Gaussian elimination works.

### Step-by-Step Solution

#### Step 1 — Start with the original matrix

$$
A=\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}.
$$

#### Step 2 — Apply $R_2\leftarrow R_2-2R_1$
Compute:

$$
R_2-2R_1=(2,4,1)-2(1,2,-1)=(2-2,4-4,1-2(-1))=(0,0,3).
$$

So the matrix becomes:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}.
$$

#### Step 3 — Apply $R_3\leftarrow R_3+R_1$
Compute:

$$
R_3+R_1=(-1,1,3)+(1,2,-1)=(0,3,2).
$$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}.
$$

#### Step 4 — Interchange $R_2$ and $R_3$
Swap the second and third rows:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}.
$$

#### Step 5 — Reverse each operation
- For $R_2\leftarrow R_2-2R_1$, the reverse is

$$
R_2\leftarrow R_2+2R_1.
$$

Because adding back the quantity that was removed restores the original row.

- For $R_3\leftarrow R_3+R_1$, the reverse is

$$
R_3\leftarrow R_3-R_1.
$$

- For interchanging $R_2$ and $R_3$, the reverse is exactly the same operation again:

$$
R_2\leftrightarrow R_3.
$$

### Final Answer
After the three operations, the matrix is

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}.
$$

The reverse operations are:
- $R_2\leftarrow R_2+2R_1$
- $R_3\leftarrow R_3-R_1$
- $R_2\leftrightarrow R_3$

### Key Takeaways
- Row operations are controlled transformations of a matrix.
- They are reversible, which is essential in elimination methods and determinant computations.
- The reversibility is what lets us undo steps and recover an earlier matrix.

---

## Exercise 9 — Composing Transformations

### Problem Statement
Let

$$
S=\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$
x=\begin{pmatrix}
1 \\
2 \\
\end{pmatrix},
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

### Objective
Apply the transformations in both orders and compare the resulting vectors.

### Concepts and Formulas
- Scaling matrix $S$ changes the $x$-coordinate by a factor 2 and leaves the $y$-coordinate unchanged.
- Rotation matrix $R$ rotates vectors by $90^\circ$ counterclockwise.
- Order matters because matrix multiplication is not commutative.

### Step-by-Step Solution

#### Step 1 — Compute $Sx$

$$
Sx=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
= \begin{pmatrix}
2\cdot1+0\cdot2 \\
0\cdot1+1\cdot2 \\
\end{pmatrix}
= \begin{pmatrix}
2 \\
2 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $RSx$
Apply the rotation matrix $R$ to the result:

$$
R(Sx)=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
2 \\
\end{pmatrix}
= \begin{pmatrix}
0\cdot2+(-1)\cdot2 \\
1\cdot2+0\cdot2 \\
\end{pmatrix}
= \begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}.
$$

So,

$$
RSx=\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix}.
$$

#### Step 3 — Compute $Rx$
First rotate the original vector:

$$
Rx=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
= \begin{pmatrix}
0\cdot1+(-1)\cdot2 \\
1\cdot1+0\cdot2 \\
\end{pmatrix}
= \begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}.
$$

#### Step 4 — Compute $SRx$
Apply the scaling matrix $S$ to the rotated vector:

$$
S(Rx)=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}
= \begin{pmatrix}
2(-2)+0\cdot1 \\
0\cdot(-2)+1\cdot1 \\
\end{pmatrix}
= \begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

Thus,

$$
SRx=\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

#### Step 5 — Compare and interpret
We have

$$
RSx=\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix},\qquad SRx=\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

These are not the same.

Geometrically:
- $S$ scales the vector in the $x$-direction by 2.
- $R$ rotates it by $90^\circ$.
- Applying $S$ first and then $R$ gives a different final result than applying $R$ first and then $S$.

This happens because matrix multiplication is not commutative: in general,

$$
RS\ne SR.
$$

The order of transformations matters because the scaling changes the direction of the vector before the rotation, while the rotation changes the direction before the scaling.

### Final Answer

$$
RSx=\begin{pmatrix}
-2 \\
2 \\
\end{pmatrix},\qquad SRx=\begin{pmatrix}
-4 \\
1 \\
\end{pmatrix}.
$$

They are different because the transformations are applied in different orders.

### Key Takeaways
- Composition of geometric transformations corresponds to matrix multiplication.
- The order of composition changes the result.
- This is a key reason matrix multiplication is not commutative.

---

## Exercise 10 — Columns of a Matrix Product

### Problem Statement
Given

$$
A=\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

### Objective
Compute the images of the columns of $B$ under $A$ and compare them with the columns of $AB$.

### Concepts and Formulas
If

$$
B=[b_1\ b_2],
$$

then

$$
AB=[Ab_1\ Ab_2].
$$

This is a very important fact: each column of a product is the product of the left matrix with the corresponding column of the right matrix.

### Step-by-Step Solution

#### Step 1 — Write the columns of $B$
The columns of $B$ are

$$
b_1=\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix},\qquad b_2=\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $Ab_1$

$$
Ab_1=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3 \\
\end{pmatrix}.
$$

Compute:
- first entry: $1\cdot1+2(-1)+0\cdot3=1-2=-1$
- second entry: $0\cdot1+1(-1)+1\cdot3=-1+3=2$
Thus,

$$
Ab_1=\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}.
$$

#### Step 3 — Compute $Ab_2$

$$
Ab_2=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1 \\
\end{pmatrix}.
$$

Compute:
- first entry: $1\cdot2+2\cdot0+0\cdot1=2$
- second entry: $0\cdot2+1\cdot0+1\cdot1=1$
Thus,

$$
Ab_2=\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}.
$$

#### Step 4 — Compute $AB$
The full matrix product is:

$$
AB=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

The first column, $Ab_1$, is

$$
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}
$$

The second column, $Ab_2$, is

$$
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
$$

Hence,

$$
AB=\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

#### Step 5 — Compare and explain
The product matrix has columns $Ab_1$ and $Ab_2$, respectively:

$$
\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix}\qquad\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},
$$

This happens because matrix multiplication is carried out column by column: each column of the right-hand matrix is treated as a vector, and multiplying by the left matrix produces the corresponding column of the product.

### Final Answer

$$
Ab_1=\begin{pmatrix}
-1 \\
2 \\
\end{pmatrix},\qquad Ab_2=\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},
$$

$$
AB=\begin{pmatrix}
-1 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

The columns of $AB$ are exactly $Ab_1$ and $Ab_2$.

### Key Takeaways
- A matrix product can be understood column by column.
- Each column of the product is the left matrix acting on the corresponding column of the right matrix.
- This viewpoint makes matrix multiplication easier to interpret conceptually.

---

## Exercise 11 — When Do Matrices Commute?

### Problem Statement
Given

$$
A=\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

### Objective
Solve $AB=BA$ for the entries of $B$ and describe the matrices that commute with $A$.

### Concepts and Formulas
Two matrices commute if their products in either order are equal.
We compute $AB$ and $BA$ and compare entries.

### Step-by-Step Solution

#### Step 1 — Compute $AB$

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
= \begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix}.
$$

#### Step 2 — Compute $BA$

$$
BA=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
= \begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}.
$$

#### Step 3 — Set them equal
For $AB=BA$, we require

$$
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix}=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}.
$$

Match entries:
- top-left: $a+c=a$ gives $c=0$.
- top-right: $b+d=a+b$ gives $d=a$.
- bottom-left: $c=c$ is automatic once $c=0$.
- bottom-right: $d=c+d$ gives $c=0$, consistent.

So the required conditions are

$$
c=0,\qquad d=a.
$$

#### Step 4 — General form of $B$
Thus any matrix of the form

$$
B=\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}
$$

commutes with $A$.

The parameter $b$ is free, while the diagonal entries must be equal.

### Final Answer
The matrices $B$ that commute with $A$ satisfy

$$
c=0,\\ d=a,
$$

so the general form is

$$
B=\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}.
$$

### Key Takeaways
- Commutativity is a special condition, not a general rule.
- The family of matrices that commute with a fixed matrix often has a simple structure.
- Here, the lower-left entry must vanish and the diagonal entries must be equal.

---

## Exercise 12 — Formula for a Matrix Power

### Problem Statement
Let

$$
A=\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

### Objective
Identify the pattern in the powers of $A$ and prove the formula by induction.

### Concepts and Formulas
- Repeated multiplication creates a pattern.
- Induction is a method of proving a formula for all positive integers.

### Step-by-Step Solution

#### Step 1 — Compute $A^2$

$$
A^2=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
= \begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $A^3$

$$
A^3=A^2A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
= \begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix}.
$$

#### Step 3 — Compute $A^4$

$$
A^4=A^3A=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
= \begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}.
$$

#### Step 4 — Form a conjecture
The powers are

$$
A^2=\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\quad
A^3=\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix},\quad
A^4=\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}.
$$

The pattern suggests

$$
A^n=\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

#### Step 5 — Prove it by induction
Assume the formula is true for some positive integer $n$:

$$
A^n=\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

Multiply by $A$ on the right:

$$
A^{n+1}=A^nA=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

The product is:
- top-left: $1\cdot1+n\cdot0=1$
- top-right: $1\cdot1+n\cdot1=n+1$
- bottom-left: $0\cdot1+1\cdot0=0$
- bottom-right: $0\cdot1+1\cdot1=1$
Therefore,

$$
A^{n+1}=\begin{pmatrix}
1 & n+1 \\
0 & 1 \\
\end{pmatrix}.
$$

This is exactly the same formula with $n+1$ in place of $n$. Hence the conjecture is correct.

### Final Answer

$$
A^2=\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\quad
A^3=\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix},\quad
A^4=\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix},
$$

and in general,

$$
A^n=\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}.
$$

### Key Takeaways
- Patterns in matrix powers can be guessed from a few examples.
- Induction gives a rigorous proof that the pattern continues forever.
- This is a standard way to prove formulas involving repeated matrix multiplication.

---

## Exercise 13 — A Recurrence Written in Matrix Form

### Problem Statement
Let

$$
F=\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

and describe the relationship you observe. Then compute

$$
F\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

### Objective
Relate powers of $F$ to Fibonacci numbers and interpret multiplication by $F$ as a recurrence step.

### Concepts and Formulas
The Fibonacci sequence is defined by

$$
F_0=0,\quad F_1=1,\quad F_{n+1}=F_n+F_{n-1}.
$$

The matrix

$$
F=\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
$$

encodes this recurrence.

### Step-by-Step Solution

#### Step 1 — Compute $F^2$

$$
F^2=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
= \begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $F^3$

$$
F^3=F^2F=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
= \begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

#### Step 3 — Compute $F^4$

$$
F^4=F^3F=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
= \begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix}.
$$

#### Step 4 — Compute $F^5$

$$
F^5=F^4F=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
= \begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}.
$$

#### Step 5 — Compare with the Fibonacci sequence
The Fibonacci sequence starts

$$
0,1,1,2,3,5,8,\ldots
$$

Notice that the entries of $F^n$ are consecutive Fibonacci numbers. For example:

$$
F^5=\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}.
$$

This fits the pattern

$$
F^n=\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1} \\
\end{pmatrix}
$$

for suitable indexing.

#### Step 6 — Compute the recurrence step

$$
F\begin{pmatrix}
a \\
b \\
\end{pmatrix}=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
= \begin{pmatrix}
a+b \\
a \\
\end{pmatrix}.
$$

This means the new vector is

$$
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}.
$$

The first entry is the sum of two consecutive terms, $a+b$. The second entry is the previous term $a$, which is exactly what we need to continue the recurrence.

If we start with

$$
\begin{pmatrix}
F_n \\
F_{n-1} \\
\end{pmatrix},
$$

then multiplying by $F$ gives

$$
\begin{pmatrix}
F_n+F_{n-1} \\
F_n \\
\end{pmatrix}=
\begin{pmatrix}
F_{n+1} \\
F_n \\
\end{pmatrix}.
$$

This is one Fibonacci recurrence step.

### Final Answer

$$
F^2=\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\quad
F^3=\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix},\quad
F^4=\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix},\quad
F^5=\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}.
$$

These entries match Fibonacci numbers.
Also,

$$
F\begin{pmatrix}
a \\
b \\
\end{pmatrix}=
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix},
$$

which performs one recurrence step by producing the next Fibonacci-like value and carrying the previous one forward.

### Key Takeaways
- Matrix multiplication can encode repeated recurrence relations.
- The matrix $F$ turns a pair of consecutive terms into the next pair.
- Powers of $F$ store Fibonacci numbers in their entries.

---

## Exercise 14 — Rotation Matrices

### Problem Statement
The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

Explain the result geometrically.

### Objective
Multiply the rotation matrices and use the angle-sum identities to verify the resulting rotation angle.

### Concepts and Formulas
The angle-sum formulas are:

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
$$

$$
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

The product of rotation matrices corresponds to composing rotations.

### Step-by-Step Solution

#### Step 1 — Write the two matrices

$$
R(\alpha)=\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha \\
\end{pmatrix},\qquad
R(\beta)=\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta \\
\end{pmatrix}.
$$

#### Step 2 — Multiply them

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha \\
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta \\
\end{pmatrix}.
$$

Compute each entry:
- top-left:

$$
\cos\alpha\cos\beta+(-\sin\alpha)(\sin\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta.
$$

- top-right:

$$
\cos\alpha(-\sin\beta)+(-\sin\alpha)\cos\beta=-(\cos\alpha\sin\beta+\sin\alpha\cos\beta).
$$

- bottom-left:

$$
\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

- bottom-right:

$$
\sin\alpha(-\sin\beta)+\cos\alpha\cos\beta=\cos\alpha\cos\beta-\sin\alpha\sin\beta.
$$

Thus,

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta & -(\cos\alpha\sin\beta+\sin\alpha\cos\beta) \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta & \cos\alpha\cos\beta-\sin\alpha\sin\beta \\
\end{pmatrix}.
$$

#### Step 3 — Use angle-sum formulas
Applying the angle-sum identities gives:
- first entry becomes $\cos(\alpha+\beta)$
- second entry becomes $-\sin(\alpha+\beta)$
- third entry becomes $\sin(\alpha+\beta)$
- fourth entry becomes $\cos(\alpha+\beta)$
Hence,

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}
=R(\alpha+\beta).
$$

#### Step 4 — Geometric interpretation
A rotation through angle $\alpha$ followed by a rotation through angle $\beta$ is the same as a single rotation through angle $\alpha+\beta$.

This matches the idea that rotating a point in the plane twice is equivalent to one rotation by the sum of the angles.

### Final Answer

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

### Key Takeaways
- Composition of rotations corresponds to addition of angles.
- Matrix multiplication encodes geometric transformations in a compact algebraic language.
- The result is consistent with the standard angle-sum formulas.

---

## Exercise 15 — Associativity of Multiplication and Different Calculation Paths

### Problem Statement
Given

$$
A=\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\quad B=\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},\quad C=\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

### Objective
Compare the two groupings of the matrix product and verify that they give the same result.

### Concepts and Formulas
Matrix multiplication is associative:

$$
(AB)C=A(BC),
$$

provided the dimensions are compatible.
This means we may group matrix products in any convenient way.

### Step-by-Step Solution

#### Step 1 — Compute $AB$

$$
AB=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}.
$$

Compute each entry:
- first row, first col:

$$
1\cdot1+2\cdot2+0\cdot(-1)=1+4=5
$$

- first row, second col:

$$
1\cdot0+2\cdot1+0\cdot3=2
$$

- second row, first col:

$$
0\cdot1+1\cdot2+1\cdot(-1)=1
$$

- second row, second col:

$$
0\cdot0+1\cdot1+1\cdot3=4
$$

Thus,

$$
AB=\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}.
$$

#### Step 2 — Compute $(AB)C$
The product with $C$ is:

$$
(AB)C=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute:
- first row, first col: $5\cdot2+2\cdot0=10$
- first row, second col: $5\cdot1+2\cdot(-1)=5-2=3$
- second row, first col: $1\cdot2+4\cdot0=2$
- second row, second col: $1\cdot1+4\cdot(-1)=1-4=-3$
Hence,

$$
(AB)C=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

#### Step 3 — Compute $BC$
For the alternative grouping:

$$
BC=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute:
- first row: $(1\cdot2+0\cdot0,\;1\cdot1+0\cdot(-1))=(2,1)$
- second row: $(2\cdot2+1\cdot0,\;2\cdot1+1\cdot(-1))=(4,1)$
- third row: $((-1)\cdot2+3\cdot0,\;(-1)\cdot1+3\cdot(-1))=(-2,-4)$
So,

$$
BC=\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}.
$$

#### Step 4 — Compute $A(BC)$
The product of $A$ and $BC$ is:

$$
A(BC)=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}.
$$

Compute:
- first row, first col: $1\cdot2+2\cdot4+0\cdot(-2)=10$
- first row, second col: $1\cdot1+2\cdot1+0\cdot(-4)=3$
- second row, first col: $0\cdot2+1\cdot4+1\cdot(-2)=2$
- second row, second col: $0\cdot1+1\cdot1+1\cdot(-4)=-3$
Hence,

$$
A(BC)=\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

#### Step 5 — Compare the results
We get

$$
(AB)C=A(BC)=\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

The final answer is the same.

#### Step 6 — Explain associativity
Associativity means that when matrices are compatible, we can group the multiplication in any way we like without changing the final product.

In this example, we can either:
- multiply $A$ and $B$ first, then multiply by $C$, or
- multiply $B$ and $C$ first, then multiply by $A$.

Both produce the same answer.

### Final Answer

$$
(AB)C=\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix},\qquad A(BC)=\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

So

$$
(AB)C=A(BC).
$$

### Key Takeaways
- Matrix multiplication is associative.
- The grouping of factors does not change the result when all products are defined.
- Although different groupings may require different numbers of intermediate calculations, the final product is the same.

---

# What I Learned and How I Would Explain It to My Professor and Class

Matrix algebra is built around a few essential ideas that I used throughout these exercises:
- matrix size and entries,
- compatible dimensions,
- addition, subtraction, and scalar multiplication,
- multiplication of matrices and vectors,
- transpose and its identity,
- identity and zero matrices,
- row operations and reversibility,
- geometric meaning of transformations,
- and the associative structure of multiplication.

What I learned is that matrix work is not just about doing calculations. It is about understanding what the numbers mean and why the operations are valid. For example, I had to check dimensions before multiplying, because a product only exists when the inner dimensions match. I also learned that matrix multiplication is not commutative, so the order matters, and this is a big difference from ordinary arithmetic.

When I explain this to my professor and classmates, I would say that matrix operations are meaningful because they model transformations, repeated operations, and structured data. The rules are not random: each rule comes from the way rows and columns interact, and once I understood that, the calculations became much easier to follow.

This work helped me see that a matrix is not just a grid of numbers; it is a tool for describing linear relationships and geometric transformations. I am more confident now that I can solve these problems by reasoning through each step instead of only memorizing formulas.
