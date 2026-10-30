## Exercise 5 — Relative Position of Two Lines

### Problem Statement
Analyze the lines

$$
L_1:(x,y,z)=(1,1,0)+t(1,2,1),
$$

$$
L_2:(x,y,z)=(2,0,1)+s(0,1,-1).
$$

If they intersect, give the intersection point. Otherwise determine whether they are parallel or skew.

### Objective
Classify two spatial lines by comparing their directions, testing for a common point, and checking coplanarity.

### Concepts and Formulas
- Parallel lines have proportional direction vectors.
- Intersecting lines have a common point.
- Two nonparallel, nonintersecting lines in space are skew.
- A coplanarity test for directions $u,v$ and displacement $w$ is $w\cdot(u\times v)=0$.

### Step-by-Step Solution

#### Step 1 — Compare the directions
The direction vectors are $u=(1,2,1)$ and $v=(0,1,-1)$. They are not proportional: the first component of $u$ is nonzero while that of $v$ is zero. Thus the lines are not parallel.

#### Step 2 — Test whether they intersect
Equating the coordinate representations gives

$$
1+t=2,\qquad 1+2t=s,\qquad t=1-s.
$$

The first equation forces $t=1$. The third then forces $s=0$, but the second would require $s=3$. The system is inconsistent, so there is no intersection.

#### Step 3 — Confirm the lines are skew
The displacement from the base point of $L_1$ to that of $L_2$ is $w=(1,-1,1)$. Compute

$$
u\times v=(-3,1,1),\qquad
w\cdot(u\times v)=-3-1+1=-3.
$$

The nonzero scalar triple product shows the directions and displacement are not coplanar. Thus the lines are skew.

### Verification
The lines are nonparallel and the coordinate equations admit no common parameter pair. The nonzero coplanarity test independently rules out intersection.

### Final Answer
$L_1$ and $L_2$ are skew lines. They do not intersect, and they are not parallel.

### Key Takeaways
- In three dimensions, nonparallel lines need not intersect.
- Distinguish skew lines from intersecting ones by solving the coordinate equations or checking coplanarity.