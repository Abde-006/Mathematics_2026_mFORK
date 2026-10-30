## Exercise 14 — Contrast: Intersection and Parallelism

### Problem Statement
From $P=(0,0,1)$, consider lines with directions $v_1=(2,1,-1)$ and $v_2=(2,1,0)$. Analyze each relative to $z=0$. Find the intersection for the line that intersects the plane, and recognize parallelism for the other without solving an equation.

### Objective
Compare line-plane behavior by testing each direction against the plane normal before calculating.

### Concepts and Formulas
- The plane $z=0$ has normal $n=(0,0,1)$.
- If $n\cdot v\neq0$, the line intersects the plane at one point.
- If $n\cdot v=0$, the line is parallel to the plane; a base point outside it means there is no intersection.

### Step-by-Step Solution

#### Step 1 — Analyze the line with direction $v_1$
The dot product is $n\cdot v_1=-1$, which is nonzero, so this line intersects the plane once. Its parameterization is

$$
(x,y,z)=(0,0,1)+t(2,1,-1)=(2t,t,1-t).
$$

Set $z=0$: $1-t=0$, so $t=1$. The intersection point is $(2,1,0)$.

#### Step 2 — Analyze the line with direction $v_2$
Now $n\cdot v_2=0$. Its $z$-coordinate remains equal to the base point's $z$-coordinate, $1$. Thus the line is parallel to $z=0$. The base point is not on the plane, so the line does not lie in it and has no intersection.

### Verification
For the first line at $t=1$, the point is $(2,1,0)$, which satisfies the plane equation. For the second line, every point has $z=1$, confirming it is disjoint from $z=0$.

### Final Answer
- Direction $v_1$: intersects $z=0$ at $(2,1,0)$.
- Direction $v_2$: parallel to $z=0$ with no common points.

### Key Takeaways
- The direction-normal dot product identifies whether the line can cross the plane.
- A parallel line is contained in the plane only if its base point lies in the plane.