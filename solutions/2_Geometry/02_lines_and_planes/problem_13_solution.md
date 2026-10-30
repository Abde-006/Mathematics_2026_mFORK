## Exercise 13 — Closest Point on a Plane

### Problem Statement
Find the point on $x+2y+2z=4$ closest to $P=(3,0,0)$. Give the distance and check that the segment joining the points is perpendicular to the plane.

### Objective
Project a point onto a plane along its normal and determine the resulting minimum distance.

### Concepts and Formulas
- The normal to $n\cdot x=d$ is $n$.
- The closest point is the orthogonal projection $H=P-\frac{n\cdot P-d}{\lVert n\rVert^2}n$.
- The distance is $|n\cdot P-d|/\lVert n\rVert$.

### Step-by-Step Solution

#### Step 1 — Identify the normal and residual
Here $n=(1,2,2)$, $d=4$, and $\lVert n\rVert^2=1+4+4=9$. For $P=(3,0,0)$,

$$
n\cdot P-d=3-4=-1.
$$

#### Step 2 — Project onto the plane
Apply the projection formula:

$$
H=P-\frac{-1}{9}n
=(3,0,0)+\frac19(1,2,2)
=\left(\frac{28}{9},\frac29,\frac29\right).
$$

#### Step 3 — Find the distance
The distance is

$$
d(P,\Pi)=\frac{|-1|}{\sqrt9}=\frac13.
$$

### Verification
The candidate lies on the plane:

$$
\frac{28}{9}+2\left(\frac29\right)+2\left(\frac29\right)
=\frac{36}{9}=4.
$$

The displacement from $P$ to $H$ is $\frac19(1,2,2)$, a scalar multiple of the plane normal. Hence the segment is perpendicular to the plane, as required for the closest point.

### Final Answer
The closest point is $\left(\frac{28}{9},\frac29,\frac29\right)$, and the distance is $\frac13$.

### Key Takeaways
- The shortest path from a point to a plane follows its normal.
- Projection, plane membership, and distance are all verified by the same normal vector.