## Exercise 2 — A Line in Space

### Problem Statement
Given

$$
L:(x,y,z)=(2,-1,3)+t(1,2,-2),
$$

state a point on the line and its direction vector, check whether $P=(4,3,-1)$ lies on $L$, and find the point corresponding to $t=-1$.

### Objective
Interpret a spatial parametric equation as a fixed point plus a scalar multiple of a direction vector.

### Concepts and Formulas
- In space, a line can be written as $r=p+tv$.
- The vector $p$ gives a point on the line, and $v$ gives its direction.
- A proposed point lies on the line if one common value of $t$ satisfies all three coordinate equations.

### Step-by-Step Solution

#### Step 1 — Read the defining point and direction
The fixed vector is $p=(2,-1,3)$, so it is a point on $L$. The direction vector is $v=(1,2,-2)$. In coordinates,

$$
x=2+t,\qquad y=-1+2t,\qquad z=3-2t.
$$

#### Step 2 — Test the point $P$
The $x$-coordinate requires $2+t=4$, so $t=2$. With this same parameter,

$$
y=-1+2(2)=3,\qquad z=3-2(2)=-1.
$$

These are the coordinates of $P$, so the point lies on $L$.

#### Step 3 — Evaluate the line at $t=-1$
Substitution gives

$$
(x,y,z)=(2,-1,3)-(1,2,-2)=(1,-3,5).
$$

### Verification
At $t=2$, the line gives $(2+2,-1+4,3-4)=(4,3,-1)$. At $t=-1$, it gives $(1,-3,5)$ as computed.

### Final Answer
A point on $L$ is $(2,-1,3)$, and a direction vector is $(1,2,-2)$. The point $P=(4,3,-1)$ lies on $L$ at $t=2$. The point at $t=-1$ is $(1,-3,5)$.

### Key Takeaways
- A parametric line specifies both a location and a direction.
- For a membership check, the same parameter must work in every coordinate.