## Exercise 15 — Complete Classification of a Line Relative to a Plane

### Problem Statement
Let $L:p+tv$ and $\Pi:n\cdot x=d$. State the conditions for one intersection point, parallelism with no common points, and containment. Give a numerical example of each case.

### Objective
Formulate a general line-plane classification using the direction-normal dot product and the plane residual at a point on the line.

### Concepts and Formulas
- Substitute $x=p+tv$ into $n\cdot x=d$ to get $n\cdot p+t(n\cdot v)=d$.
- The coefficient $n\cdot v$ determines whether the line direction crosses the plane.
- If $n\cdot v=0$, the value $n\cdot p-d$ determines whether the line is outside the plane or contained in it.

### Step-by-Step Solution

#### Step 1 — Derive the parameter equation
Substitution gives

$$
n\cdot p+t(n\cdot v)=d.
$$

Equivalently,

$$
t(n\cdot v)=d-n\cdot p.
$$

#### Step 2 — Classify the cases
1. **One intersection point:** If $n\cdot v\neq0$, there is exactly one parameter,

$$
t=\frac{d-n\cdot p}{n\cdot v}.
$$

2. **Parallel with no common points:** If $n\cdot v=0$ and $n\cdot p\neq d$, the left side of the substituted equation is constant and unequal to $d$. No point of the line lies in the plane.

3. **Line contained in the plane:** If $n\cdot v=0$ and $n\cdot p=d$, the base point is in the plane and the direction remains within it. Every point of the line is therefore in the plane.

#### Step 3 — Give numerical examples
Use the plane $z=0$, with normal $n=(0,0,1)$ and $d=0$.

- **One intersection:** Take $p=(0,0,1)$ and $v=(1,0,-1)$. Then $n\cdot v=-1\neq0$, and the line $(t,0,1-t)$ meets $z=0$ at $t=1$, or $(1,0,0)$.
- **Parallel, disjoint:** Take $p=(0,0,1)$ and $v=(1,2,0)$. Then $n\cdot v=0$ while $n\cdot p=1\neq0$. The line stays at $z=1$.
- **Contained:** Take $p=(1,0,0)$ and $v=(1,1,0)$. Then $n\cdot v=0$ and $n\cdot p=0=d$. Every point stays in $z=0$.

### Verification
In the first example, the line's $z$-coordinate vanishes at exactly one parameter. In the second it is always $1$, and in the third it is always $0$. These coordinate checks confirm each criterion.

### Final Answer
- $n\cdot v\neq0$: exactly one intersection, at $t=(d-n\cdot p)/(n\cdot v)$.
- $n\cdot v=0$ and $n\cdot p\neq d$: parallel, no common points.
- $n\cdot v=0$ and $n\cdot p=d$: the line is contained in the plane.

### Key Takeaways
- The dot product $n\cdot v$ detects whether the line crosses the plane.
- When it vanishes, checking one point distinguishes a disjoint parallel line from a contained line.