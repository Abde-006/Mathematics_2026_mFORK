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
