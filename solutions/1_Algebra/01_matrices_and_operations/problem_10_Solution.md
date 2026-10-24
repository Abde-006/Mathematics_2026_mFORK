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
