## Exercise 1 — Line Through Two Points

### Problem Statement
Find the equation of the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation.

### Objective
Construct equivalent vector and Cartesian descriptions of a line, and connect its direction and normal vectors.

### Concepts and Formulas
- A line through $A$ with direction vector $v$ has parametric form $x=A+tv$.
- In the plane, a normal vector $n=(a,b)$ gives a line equation $ax+by+c=0$.
- A direction vector is perpendicular to every normal vector of the line.

### Step-by-Step Solution

#### Step 1 — Find a direction vector
Subtract the coordinates of $A$ from those of $B$:

$$
B-A=(4-1,-1-2)=(3,-3).
$$

Any nonzero scalar multiple is also a direction vector, so choose the simpler vector $v=(1,-1)$.

#### Step 2 — Write the parametric equation
Using $A$ as the point on the line gives

$$
(x,y)=(1,2)+t(1,-1),\qquad t\in\mathbb R.
$$

Equivalently, $x=1+t$ and $y=2-t$.

#### Step 3 — Find a normal vector and general equation
A vector perpendicular to $(1,-1)$ is $n=(1,1)$ because $(1,-1)\cdot(1,1)=0$. Thus the line has form $x+y=c$. Substitution of $A$ gives $c=1+2=3$, so

$$
x+y-3=0.
$$

### Verification
For $A=(1,2)$, the left side is $1+2-3=0$. For $B=(4,-1)$, it is $4-1-3=0$. Both points also appear on the parametric line: $t=0$ gives $A$, and $t=3$ gives $B$.

### Final Answer
- Parametric form: $(x,y)=(1,2)+t(1,-1)$.
- General form: $x+y-3=0$.
- Direction vector: $(1,-1)$.
- One normal vector: $(1,1)$.

### Key Takeaways
- Subtracting two points gives a direction vector.
- The coefficients in a line's general equation form a normal vector, perpendicular to its direction.