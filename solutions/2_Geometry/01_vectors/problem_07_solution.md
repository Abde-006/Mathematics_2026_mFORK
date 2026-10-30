## Exercise 7 — Linear Dependence Without Heavy Computation

### Problem Statement
Given $u=(1,2,3)$, $v=(2,4,6)$, and $w=(0,1,1)$, identify a relation between $u$ and $v$, decide whether the three vectors can be linearly independent, and explain why no long calculation is needed.

### Objective
Recognize linear dependence by inspecting the vectors for scalar multiples.

### Concepts and Formulas
- A set is linearly dependent if a nontrivial combination of its vectors equals zero.
- One vector being a scalar multiple of another immediately gives such a relation.
- If a subset is dependent, the entire set is dependent.

### Step-by-Step Solution

#### Step 1 — Compare $u$ and $v$

$$
2u=2(1,2,3)=(2,4,6)=v
$$

Equivalently, $v-2u=0$ is a nontrivial relation between the vectors.

#### Step 2 — Decide independence of all three
Since the pair $u,v$ is already dependent, adding $w$ cannot make the full set independent. The same relation $v-2u+0w=0$ still holds.

### Verification
The equality $v=2u$ holds in all three coordinates, so it directly certifies dependence without computing a determinant or solving a larger system.

### Final Answer
The relation is $v=2u$, or $v-2u=0$. The three vectors are linearly dependent.

### Key Takeaways
- Check for scalar multiples before using a more involved dependence test.
- A dependent subset ensures that any larger set containing it is dependent.
