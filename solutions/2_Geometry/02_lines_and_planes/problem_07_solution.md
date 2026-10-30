## Exercise 7 — A Line Relative to a Plane

### Problem Statement
For

$$
L:(x,y,z)=(1,1,0)+t(1,-1,0),\qquad \Pi:x+y+z=2,
$$

determine whether the line intersects the plane at one point, is parallel to it, or lies in it. Explain the role of the direction-normal dot product.

### Objective
Apply the direction-vector and plane-normal test to classify a line relative to a plane.

### Concepts and Formulas
- The plane normal is the coefficient vector of its equation.
- If line direction $v$ satisfies $n\cdot v\neq0$, the line meets the plane once.
- If $n\cdot v=0$, the line is parallel to the plane or contained in it; test a point on the line to distinguish these cases.

### Step-by-Step Solution

#### Step 1 — Test the direction
The plane normal is $n=(1,1,1)$ and the line direction is $v=(1,-1,0)$. Their dot product is

$$
n\cdot v=1-1+0=0.
$$

Thus motion along the line does not change the plane's left-hand side, so the line is parallel to the plane or contained in it.

#### Step 2 — Test the line's base point
The base point is $p=(1,1,0)$. It satisfies $1+1+0=2$, so it lies on the plane. Since one point of this parallel line is in the plane, the whole line is in the plane.

### Verification
At every point of the line, $x+y+z=(1+t)+(1-t)+0=2$. This confirms that every line point satisfies the plane equation.

### Final Answer
The line lies in the plane.

### Key Takeaways
- A zero dot product means the line's direction is parallel to the plane.
- A single point substitution then distinguishes containment from a disjoint parallel line.