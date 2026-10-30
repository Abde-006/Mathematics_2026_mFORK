## Exercise 10 — Projection of a Point onto a Plane

### Problem Statement
Find the orthogonal projection of $P=(2,1,3)$ onto $x+y+z=3$, then find the reflection of $P$ across the plane. Check that the midpoint of the point and its reflection lies on the plane.

### Objective
Use the plane normal to construct the perpendicular projection and the corresponding reflection.

### Concepts and Formulas
- For plane $n\cdot x=d$, the projection of $P$ is $H=P-\frac{n\cdot P-d}{\lVert n\rVert^2}n$.
- The reflection across the plane is $R=P-2\frac{n\cdot P-d}{\lVert n\rVert^2}n=2H-P$.
- The projection-to-point segment is parallel to the normal.

### Step-by-Step Solution

#### Step 1 — Find the normal offset
Here $n=(1,1,1)$, $d=3$, and $\lVert n\rVert^2=3$. The signed plane residual at $P$ is

$$
n\cdot P-d=2+1+3-3=3.
$$

#### Step 2 — Compute the projection
The normal correction is $(3/3)n=n$. Thus

$$
H=P-n=(2,1,3)-(1,1,1)=(1,0,2).
$$

#### Step 3 — Compute the reflection
Reflecting doubles the correction:

$$
R=P-2n=(2,1,3)-(2,2,2)=(0,-1,1).
$$

### Verification
The projected point lies on the plane because $1+0+2=3$. The midpoint of $P$ and $R$ is

$$
\frac{P+R}{2}=\left(\frac{2+0}{2},\frac{1-1}{2},\frac{3+1}{2}\right)=(1,0,2),
$$

which is the projection and lies on the plane. Also, $P-H=(1,1,1)$ is parallel to the plane normal.

### Final Answer
The orthogonal projection is $H=(1,0,2)$, and the reflection is $R=(0,-1,1)$.

### Key Takeaways
- Projection moves a point along the normal until it reaches the plane.
- Reflection continues the same normal displacement by an equal amount on the other side.