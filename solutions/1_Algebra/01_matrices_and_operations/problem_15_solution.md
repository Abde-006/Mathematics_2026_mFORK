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
