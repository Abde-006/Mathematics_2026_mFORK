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
