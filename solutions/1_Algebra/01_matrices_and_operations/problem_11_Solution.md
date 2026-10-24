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
