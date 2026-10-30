## Exercise 9 — Cross Product as a Perpendicular Direction

### Problem Statement
For $u=(1,2,0)$ and $v=(0,1,3)$, compute $u\times v$. Use dot products to verify perpendicularity to both vectors, compute $v\times u$, and compare the results.

### Objective
Compute a cross product, verify its perpendicularity, and observe the effect of reversing its order.

### Concepts and Formulas
- In $\mathbb R^3$, the cross product is perpendicular to both input vectors.
- Reversing the order changes its sign: $v\times u=-(u\times v)$.

### Step-by-Step Solution

#### Step 1 — Compute the cross product

$$
u\times v=(2\cdot3-0\cdot1,\;0\cdot0-1\cdot3,\;1\cdot1-2\cdot0)=(6,-3,1)
$$

#### Step 2 — Check it is perpendicular to each vector

$$
(u\times v)\cdot u=(6,-3,1)\cdot(1,2,0)=6-6+0=0
$$

$$
(u\times v)\cdot v=(6,-3,1)\cdot(0,1,3)=0-3+3=0
$$

#### Step 3 — Reverse the order

$$
v\times u=(-6,3,-1)=-(6,-3,1)=-(u\times v)
$$

### Verification
Both dot products are zero, confirming perpendicularity. The reversed cross product is the negative of the original.

### Final Answer

$$
u\times v=(6,-3,1),\qquad v\times u=(-6,3,-1)
$$

The cross product gives a perpendicular direction, and reversing the inputs reverses its orientation.

### Key Takeaways
- Dot products provide a direct check that a cross product is perpendicular.
- The cross product is anti-commutative: reversing the inputs changes the sign.
