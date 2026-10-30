## Exercise 11 — Decomposition into Parallel and Perpendicular Components

### Problem Statement
Decompose $u=(3,4)$ into components parallel and perpendicular to $v=(1,2)$. Check that $u=u_{\parallel}+u_{\perp}$ and $u_{\perp}\cdot v=0$, and explain why these are two independent checks.

### Objective
Construct an orthogonal decomposition by projection and verify both its sum and perpendicularity properties.

### Concepts and Formulas
- The parallel component is $u_{\parallel}=\frac{u\cdot v}{v\cdot v}v$.
- The perpendicular component is $u_{\perp}=u-u_{\parallel}$.
- A correct decomposition must both add to $u$ and have its remainder perpendicular to $v$.

### Step-by-Step Solution

#### Step 1 — Find the projection coefficient

$$
u\cdot v=3(1)+4(2)=11,\qquad v\cdot v=1^2+2^2=5
$$

#### Step 2 — Compute both components

$$
u_{\parallel}=\frac{11}{5}(1,2)=\left(\frac{11}{5},\frac{22}{5}\right)
$$

$$
u_{\perp}=u-u_{\parallel}
=\left(3-\frac{11}{5},4-\frac{22}{5}\right)
=\left(\frac{4}{5},-\frac{2}{5}\right)
$$

#### Step 3 — Check the sum and perpendicularity

$$
u_{\parallel}+u_{\perp}
=\left(\frac{11}{5}+\frac{4}{5},\frac{22}{5}-\frac{2}{5}\right)
=(3,4)=u
$$

$$
u_{\perp}\cdot v=\frac{4}{5}(1)-\frac{2}{5}(2)=0
$$

### Verification
The sum check confirms that the two components reconstruct $u$. The dot-product check separately confirms that the remainder is perpendicular to the specified direction. Either condition alone would not ensure both properties.

### Final Answer

$$
u_{\parallel}=\left(\frac{11}{5},\frac{22}{5}\right),\qquad
u_{\perp}=\left(\frac{4}{5},-\frac{2}{5}\right)
$$

### Key Takeaways
- Projection gives the component parallel to a direction.
- Verify a decomposition by checking both reconstruction and orthogonality.
