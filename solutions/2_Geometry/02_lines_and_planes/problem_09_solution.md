## Exercise 9 — Distances

### Problem Statement
Compute the distance from $P=(2,3)$ to $3x+4y-10=0$, and the distance from $Q=(2,-1,3)$ to $2x-2y+z-4=0$. Compare the formulas and explain their connection with the normal direction.

### Objective
Apply the point-to-hyperplane distance formula in two and three dimensions.

### Concepts and Formulas
- For $ax+by+c=0$, the point-to-line distance is $|ax_0+by_0+c|/\sqrt{a^2+b^2}$.
- For $ax+by+cz+d=0$, the point-to-plane distance is $|ax_0+by_0+cz_0+d|/\sqrt{a^2+b^2+c^2}$.
- The denominator is the length of the normal vector; the numerator measures the point's signed displacement in the normal equation.

### Step-by-Step Solution

#### Step 1 — Distance to the line
For the line $3x+4y-10=0$, the normal is $(3,4)$, of length $5$. At $P=(2,3)$, the equation's left side is $3(2)+4(3)-10=8$. Hence

$$
d(P,\ell)=\frac{|8|}{\sqrt{3^2+4^2}}=\frac85.
$$

#### Step 2 — Distance to the plane
For the plane $2x-2y+z-4=0$, the normal is $(2,-2,1)$, of length $3$. At $Q=(2,-1,3)$, the left side is $2(2)-2(-1)+3-4=5$. Therefore

$$
d(Q,\Pi)=\frac{|5|}{\sqrt{2^2+(-2)^2+1^2}}=\frac53.
$$

### Verification
The denominators are nonzero normal lengths. Taking absolute values ensures distances are nonnegative, regardless of which side of the line or plane contains the point.

### Final Answer
- Distance from $P$ to the line: $\frac85$.
- Distance from $Q$ to the plane: $\frac53$.

### Key Takeaways
- The same geometric formula works for a line in the plane and a plane in space.
- The normal direction identifies the shortest path, and normalizing by its length converts the equation residual into distance.