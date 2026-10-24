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
