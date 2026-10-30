## Exercise 11 — Plane Containing a Line and a Point

### Problem Statement
Find the plane containing the line $(x,y,z)=(1,0,2)+t(1,1,-1)$ and the point $P=(0,2,1)$. Check that the whole line and the point lie in the plane.

### Objective
Construct a plane normal from a line direction and a second independent direction to a point.

### Concepts and Formulas
- A plane containing a line contains its direction vector.
- The vector from a point on the line to an additional point in the plane is another plane direction.
- The cross product of two independent plane directions is a normal.

### Step-by-Step Solution

#### Step 1 — Find two directions in the plane
Use the line's base point $A=(1,0,2)$ and direction $v=(1,1,-1)$. The vector toward $P$ is

$$
w=P-A=(-1,2,-1).
$$

#### Step 2 — Compute a normal vector
The cross product is

$$
v\times w=(1,2,3).
$$

Indeed, its components are $1$, $2$, and $3$, and it is perpendicular to both $v$ and $w$.

#### Step 3 — Write the plane equation
Using normal $n=(1,2,3)$ and point $A$,

$$
n\cdot((x,y,z)-A)=0.
$$

Therefore

$$
(x-1)+2y+3(z-2)=0,
$$

or

$$
x+2y+3z=7.
$$

### Verification
For $P=(0,2,1)$, the left side is $0+4+3=7$. The line's base point gives $1+0+6=7$, and its direction satisfies $n\cdot v=1+2-3=0$. Thus moving by any $t v$ preserves the plane equation, so the entire line is contained.

### Final Answer
The plane is $x+2y+3z=7$.

### Key Takeaways
- A line and an external point determine a plane when the point does not lie on the line.
- A plane normal can be built from two independent directions using a cross product.