## Exercise 3 — Plane Through a Point with a Given Normal Vector

### Problem Statement
Find the equation of the plane through $P=(1,-2,3)$ and perpendicular to $n=(2,1,-1)$. Check the result by substituting $P$ and explain the role of the normal vector.

### Objective
Build a plane equation from one point and a normal vector.

### Concepts and Formulas
- A plane through $P$ with normal vector $n$ consists of points $X$ for which $n\cdot(X-P)=0$.
- The normal vector is perpendicular to every direction lying in the plane.

### Step-by-Step Solution

#### Step 1 — Apply the point-normal equation
Write $X=(x,y,z)$. Then

$$
(2,1,-1)\cdot(x-1,y+2,z-3)=0.
$$

Expanding the dot product gives

$$
2(x-1)+(y+2)-(z-3)=0.
$$

#### Step 2 — Simplify
Collecting terms,

$$
2x+y-z+3=0.
$$

The coefficients $(2,1,-1)$ are precisely the components of the normal vector.

### Verification
Substitute $P=(1,-2,3)$:

$$
2(1)+(-2)-3+3=0.
$$

Thus $P$ lies on the plane. Any displacement within the plane has dot product zero with $n$, which is why $n$ is normal to it.

### Final Answer

$$
2x+y-z+3=0.
$$

### Key Takeaways
- A plane is determined by a point and a nonzero normal vector.
- The normal vector is the coefficient vector of the plane's Cartesian equation.