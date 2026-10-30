## Exercise 6 — Angle Between Planes

### Problem Statement
Given $\Pi_1:x+y+z=1$ and $\Pi_2:x-y=2$, determine whether the planes are parallel. If not, compute their angle and explain why the normal vectors suffice.

### Objective
Use plane normals to classify the planes and find their angle.

### Concepts and Formulas
- For $ax+by+cz=d$, a normal vector is $(a,b,c)$.
- Planes are parallel exactly when their nonzero normals are proportional.
- The acute angle between planes is the acute angle between their normals, with cosine given by the absolute dot product divided by the product of their lengths.

### Step-by-Step Solution

#### Step 1 — Identify and compare the normals
The normals are $n_1=(1,1,1)$ and $n_2=(1,-1,0)$. They are not proportional, so the planes are not parallel.

#### Step 2 — Compute their angle
The dot product is

$$
n_1\cdot n_2=1-1+0=0.
$$

Therefore the normals are perpendicular. Equivalently,

$$
\cos\theta=\frac{|n_1\cdot n_2|}{\lVert n_1\rVert\lVert n_2\rVert}
=\frac{0}{\sqrt{3}\sqrt{2}}=0,
$$

so $\theta=90^\circ$.

### Verification
The planes are not parallel because their normals have different directions. Their zero dot product establishes perpendicular normals and therefore perpendicular planes.

### Final Answer
The planes are not parallel; they intersect at a right angle. The angle between them is $90^\circ$.

### Key Takeaways
- A plane's normal determines its orientation, independent of its position.
- Dot products of normals give the angle between the planes.