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
