## Exercise 8 — Intersection Point of a Line and a Plane

### Problem Statement
Find the intersection of $(x,y,z)=(1,0,2)+t(1,2,-1)$ with the plane $x+y+z=4$. Check the point in both descriptions.

### Objective
Find a line-plane intersection by substituting the line's coordinate expressions into the plane equation.

### Concepts and Formulas
- A line-plane intersection is found by inserting the parametric coordinates into the plane equation.
- A nonzero coefficient of the parameter gives one unique intersection.

### Step-by-Step Solution

#### Step 1 — Write the line coordinates
The line gives

$$
x=1+t,\qquad y=2t,\qquad z=2-t.
$$

#### Step 2 — Solve for the parameter
Substitute into $x+y+z=4$:

$$
(1+t)+2t+(2-t)=4.
$$

This simplifies to $3+2t=4$, so $t=\frac12$.

#### Step 3 — Calculate the point
At $t=\frac12$,

$$
(x,y,z)=\left(1+\frac12,1,2-\frac12\right)
=\left(\frac32,1,\frac32\right).
$$

### Verification
On the line this point corresponds to $t=\frac12$. In the plane,

$$
\frac32+1+\frac32=4.
$$

Both conditions hold.

### Final Answer
The intersection point is $\left(\frac32,1,\frac32\right)$.

### Key Takeaways
- Substitution converts the geometric intersection question into a one-variable equation.
- Verify the resulting point against both the line and the plane.