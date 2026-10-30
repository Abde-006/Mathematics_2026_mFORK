## Exercise 4 — Plane Through Three Points

### Problem Statement
Find the plane through $A=(1,0,0)$, $B=(0,1,0)$, and $C=(0,0,1)$. Construct two vectors in the plane, use their cross product, and check the equation on all three points.

### Objective
Construct a plane normal from two independent directions within the plane.

### Concepts and Formulas
- Differences of points on a plane give direction vectors in the plane.
- The cross product of two nonparallel plane directions is perpendicular to both and hence is a normal vector.
- For a plane through $A$ with normal $n$, use $n\cdot(X-A)=0$.

### Step-by-Step Solution

#### Step 1 — Construct two plane directions
Using $A$ as the base point,

$$
\overrightarrow{AB}=B-A=(-1,1,0),\qquad
\overrightarrow{AC}=C-A=(-1,0,1).
$$

These are not scalar multiples, so they determine the plane's two independent directions.

#### Step 2 — Compute a normal vector
Their cross product is

$$
\overrightarrow{AB}\times\overrightarrow{AC}=
\begin{pmatrix}
1 \\
1 \\
1 \\
\end{pmatrix}.
$$

For example, its first component is $1\cdot1-0\cdot0=1$, its second is $0\cdot(-1)-(-1)\cdot1=1$, and its third is $(-1)\cdot0-1\cdot(-1)=1$. Thus take $n=(1,1,1)$.

#### Step 3 — Form the plane equation
The point-normal equation through $A$ is

$$
(1,1,1)\cdot(x-1,y,z)=0,
$$

which simplifies to

$$
x+y+z=1.
$$

### Verification
At $A$, $1+0+0=1$; at $B$, $0+1+0=1$; and at $C$, $0+0+1=1$. Hence all three points satisfy the equation.

### Final Answer
The plane is $x+y+z=1$, with normal vector $(1,1,1)$.

### Key Takeaways
- The cross product provides a normal from two nonparallel vectors in a plane.
- A point-normal equation then determines the plane.