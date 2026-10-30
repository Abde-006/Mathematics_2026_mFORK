## Exercise 13 — Do Four Points Lie in One Plane?

### Problem Statement
Given $A=(0,0,0)$, $B=(1,2,0)$, $C=(0,1,1)$, and $D=(2,5,1)$, construct $\overrightarrow{AB}$ and $\overrightarrow{AC}$, find their cross product $n$, construct $\overrightarrow{AD}$, check $\overrightarrow{AD}\cdot n$, and decide whether $D$ lies in the plane determined by $A,B,C$.

### Objective
Use a normal vector and a dot-product test to determine whether a point lies in a plane.

### Concepts and Formulas
- Two direction vectors in the plane determine a normal through their cross product.
- A displacement from a point in the plane lies in the plane exactly when it is perpendicular to the plane's normal.

### Step-by-Step Solution

#### Step 1 — Construct two directions in the plane

$$
\overrightarrow{AB}=B-A=(1,2,0),\qquad
\overrightarrow{AC}=C-A=(0,1,1)
$$

#### Step 2 — Find a normal vector

$$
n=\overrightarrow{AB}\times\overrightarrow{AC}
=(2\cdot1-0\cdot1,\;0\cdot0-1\cdot1,\;1\cdot1-2\cdot0)
=(2,-1,1)
$$

#### Step 3 — Test the fourth point

$$
\overrightarrow{AD}=D-A=(2,5,1)
$$

$$
\overrightarrow{AD}\cdot n=(2,5,1)\cdot(2,-1,1)=4-5+1=0
$$

Since this dot product is zero, $\overrightarrow{AD}$ lies in the plane's directions. In fact,

$$
\overrightarrow{AD}=2\overrightarrow{AB}+\overrightarrow{AC}
$$

which also directly shows that $D$ is reached by a combination of the two in-plane directions from $A$.

### Verification
The normal test gives zero, and the explicit linear combination reproduces $(2,5,1)$. Both confirm that $D$ lies in the plane through $A,B,C$.

### Final Answer
$D$ lies in the plane determined by $A,B,C$ because $\overrightarrow{AD}\cdot n=0$ for $n=(2,-1,1)$.

### Key Takeaways
- A normal vector converts plane membership into a dot-product test.
- An in-plane displacement can also be expressed as a combination of two in-plane directions.
