# Solution 9 — Area and the Determinant

### Problem Statement
Find the area of the parallelogram spanned by

$$
u=\begin{pmatrix}3\\1\end{pmatrix},\qquad
v=\begin{pmatrix}1\\4\end{pmatrix},
$$

and describe what happens when their order is reversed.

### Objective
Interpret the absolute value of a determinant as area.

### Concepts and Formulas
For two vectors in the plane, the parallelogram area is the absolute value of the determinant formed using the vectors as columns.

### Step-by-Step Solution
Place $u$ and $v$ in the columns:

$$
\det\begin{pmatrix}3&1\\1&4\end{pmatrix}
=3\cdot4-1\cdot1=11.
$$

Thus the area is $|11|=11$ square units. Reversing the columns gives

$$
\det\begin{pmatrix}1&3\\4&1\end{pmatrix}
=1\cdot1-3\cdot4=-11.
$$

The signed determinant changes sign under a column swap, but its absolute value—and therefore the area—remains $11$.

### Final Answer
The parallelogram has area

$$
\boxed{11\text{ square units}}.
$$

Reversing the vector order changes the determinant from $11$ to $-11$, not the area.

### Key Takeaways
- The determinant gives signed area; the geometric area is its absolute value.