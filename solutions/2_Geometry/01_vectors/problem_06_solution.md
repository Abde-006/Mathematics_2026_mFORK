## Exercise 6 — Projection and Perpendicular Component

### Problem Statement
Find the projection of $u=(4,2)$ onto the direction $v=(1,1)$. Then compute $r=u-\mathrm{proj}_v\,u$, verify that $r\cdot v=0$, and interpret the result geometrically.

### Objective
Decompose a vector into its part parallel to a given direction and its perpendicular remainder.

### Concepts and Formulas
- The projection of $u$ onto nonzero $v$ is $\mathrm{proj}_v\,u=\frac{u\cdot v}{v\cdot v}v$.
- Subtracting the projection leaves a component perpendicular to $v$.

### Step-by-Step Solution

#### Step 1 — Calculate the projection coefficient

$$
u\cdot v=4(1)+2(1)=6,\qquad v\cdot v=1^2+1^2=2
$$

Thus the coefficient is $6/2=3$.

#### Step 2 — Find the projection and remainder

$$
\mathrm{proj}_v\,u=3(1,1)=(3,3)
$$

$$
r=u-\mathrm{proj}_v\,u=(4,2)-(3,3)=(1,-1)
$$

#### Step 3 — Check perpendicularity

$$
r\cdot v=(1,-1)\cdot(1,1)=1-1=0
$$

### Verification
The result splits $u$ as $(3,3)+(1,-1)=(4,2)$, and the remainder has zero dot product with $v$.

### Final Answer

$$
\mathrm{proj}_v\,u=(3,3),\qquad r=(1,-1)
$$

Geometrically, $(3,3)$ is the part of $u$ along the line in direction $v$, and $r$ is the perpendicular offset from that line to the tip of $u$.

### Key Takeaways
- Projection extracts the component parallel to a direction.
- The leftover component is perpendicular to that direction.
