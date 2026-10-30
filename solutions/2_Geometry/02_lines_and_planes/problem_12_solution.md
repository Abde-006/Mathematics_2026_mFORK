## Exercise 12 — Intersection Line of Two Planes

### Problem Statement
Find a parametric equation of the intersection of $x+y+z=3$ and $x-y+z=1$. Find its direction vector both from the system and from the cross product of the normals, and compare the results.

### Objective
Construct the common line of two nonparallel planes using algebraic elimination and plane normals.

### Concepts and Formulas
- Points on the intersection satisfy both plane equations.
- The direction of the intersection is perpendicular to both plane normals.
- A cross product of the normals gives such a direction.

### Step-by-Step Solution

#### Step 1 — Solve the plane system
Subtract the second equation from the first:

$$
2y=2,
$$

so $y=1$. Substitution into either plane equation gives $x+z=2$. Let $x=t$, which gives $z=2-t$.

#### Step 2 — Write the line
The intersection line is

$$
(x,y,z)=(0,1,2)+t(1,0,-1),\qquad t\in\mathbb R.
$$

Its direction from the parameterization is $(1,0,-1)$.

#### Step 3 — Obtain the direction from the normals
The plane normals are $n_1=(1,1,1)$ and $n_2=(1,-1,1)$. Expanding the cross product gives

$$
n_1\times n_2=
\begin{pmatrix}
1\cdot1-1\cdot(-1) \\
1\cdot1-1\cdot1 \\
1\cdot(-1)-1\cdot1 \\
\end{pmatrix}
=(2,0,-2).
$$

Thus the cross-product direction is $(2,0,-2)=2(1,0,-1)$, a nonzero scalar multiple of the system-derived direction.

### Verification
At the base point $(0,1,2)$, the first plane gives $0+1+2=3$ and the second gives $0-1+2=1$. The direction $(1,0,-1)$ is perpendicular to both normals: its dot products are $1-1=0$ and $1-1=0$. Therefore every point on the parameterized line satisfies both plane equations.

### Final Answer
The intersection line is $(x,y,z)=(0,1,2)+t(1,0,-1)$. Both methods produce direction $(1,0,-1)$ up to a nonzero scalar.

### Key Takeaways
- Eliminating variables gives a direct parameterization of the intersection.
- The cross product of plane normals gives the same line direction geometrically.