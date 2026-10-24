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
