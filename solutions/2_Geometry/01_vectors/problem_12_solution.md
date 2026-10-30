## Exercise 12 — A Normal Vector to a Plane

### Problem Statement
Given $A=(1,0,2)$, $B=(2,1,0)$, and $C=(0,3,1)$, construct two vectors in the plane, find a vector perpendicular to both, and check perpendicularity using dot products.

### Objective
Find a normal vector to the plane through three given points.

### Concepts and Formulas
- Differences between points in a plane give direction vectors in that plane.
- The cross product of two nonparallel direction vectors is perpendicular to both.
- A dot product of zero verifies perpendicularity.

### Step-by-Step Solution

#### Step 1 — Construct two in-plane vectors

$$
\overrightarrow{AB}=B-A=(1,1,-2),\qquad
\overrightarrow{AC}=C-A=(-1,3,-1)
$$

#### Step 2 — Take their cross product

$$
\overrightarrow{AB}\times\overrightarrow{AC}
=(1(-1)-(-2)(3),\;(-2)(-1)-1(-1),\;1(3)-1(-1))
=(5,3,4)
$$

Set $n=(5,3,4)$.

#### Step 3 — Verify both perpendicularities

$$
n\cdot\overrightarrow{AB}=5(1)+3(1)+4(-2)=5+3-8=0
$$

$$
n\cdot\overrightarrow{AC}=5(-1)+3(3)+4(-1)=-5+9-4=0
$$

### Verification
Both dot products vanish, so $n$ is perpendicular to the two in-plane directions and hence is a normal vector to the plane.

### Final Answer
Two vectors in the plane are $\overrightarrow{AB}=(1,1,-2)$ and $\overrightarrow{AC}=(-1,3,-1)$. One normal vector is

$$
n=(5,3,4)
$$

### Key Takeaways
- Point differences construct directions in a plane.
- The cross product of two in-plane directions produces a normal.
