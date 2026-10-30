## Exercise 14 — Closest Point on a Line

### Problem Statement
For $P=(4,1)$ and the line through the origin with direction $v=(1,2)$, use projection to find the closest point on the line, the distance from $P$ to the line, and verify perpendicularity.

### Objective
Solve a minimum-distance problem by projecting onto a line and checking that the residual is perpendicular to the line.

### Concepts and Formulas
- The line through the origin with direction $v$ consists of scalar multiples of $v$.
- Denote this line by $\ell$.
- The closest point on that line to $P$ is the projection $\frac{P\cdot v}{v\cdot v}v$.
- The distance is the length of the residual from the projected point to $P$.

### Step-by-Step Solution

#### Step 1 — Find the projection coefficient

$$
P\cdot v=4(1)+1(2)=6,\qquad v\cdot v=1^2+2^2=5
$$

#### Step 2 — Find the closest point

$$
Q=\mathrm{proj}_v\,P=\frac{6}{5}(1,2)=\left(\frac{6}{5},\frac{12}{5}\right)
$$

The shortest displacement from the line to $P$ is

$$
P-Q=\left(4-\frac{6}{5},1-\frac{12}{5}\right)
=\left(\frac{14}{5},-\frac{7}{5}\right)
$$

#### Step 3 — Compute the distance

$$
d(P,\ell)=\|P-Q\|
=\sqrt{\left(\frac{14}{5}\right)^2+\left(-\frac{7}{5}\right)^2}
=\sqrt{\frac{245}{25}}=\frac{7\sqrt{5}}{5}
$$

#### Step 4 — Verify perpendicularity

$$
(P-Q)\cdot v=\frac{14}{5}(1)-\frac{7}{5}(2)=0
$$

### Verification
The residual is perpendicular to the line direction. Therefore, moving from $Q$ along the line cannot reduce the distance to $P$; $Q$ is the closest point.

### Final Answer
The closest point is $Q=(6/5,12/5)$, and the distance is $7\sqrt{5}/5$.

### Key Takeaways
- Projection identifies the point on a line closest to a given point.
- At the closest point, the connecting displacement is perpendicular to the line.
