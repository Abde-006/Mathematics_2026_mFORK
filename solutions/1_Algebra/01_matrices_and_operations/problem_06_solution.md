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
