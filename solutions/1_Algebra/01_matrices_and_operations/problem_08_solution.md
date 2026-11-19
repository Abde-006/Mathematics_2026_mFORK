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
