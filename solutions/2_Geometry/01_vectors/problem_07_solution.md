## Exercise 7 — Linear Dependence Without Heavy Computation

### Problem statement

Given

$$
u=(1,2,3),\qquad v=(2,4,6),\qquad w=(0,1,1)
$$

identify a relation between $u$ and $v$, decide whether the three vectors are linearly independent, and explain why no long calculation is needed.

### Formula used

A set of vectors is linearly dependent if there is a nontrivial linear relation

$$
c_1u+c_2v+c_3w=0
$$

where at least one coefficient is nonzero.

A vector pair is automatically dependent if one vector is a scalar multiple of the other.

### Solution

Compare $u$ and $v$ coordinate by coordinate:

$$
2u=2(1,2,3)=(2,4,6)=v
$$

Thus $v$ is twice $u$. The corresponding nontrivial relation is

$$
v-2u=0
$$

The coefficient of $u$ is $-2$ and the coefficient of $v$ is $1$, so this is a nontrivial relation.

To include $w$, add its coefficient as zero:

$$
-2u+1v+0w=0
$$

Since at least one coefficient is nonzero, the complete set $\{u,v,w\}$ is linearly dependent.

### Explanation

Dependence was visible immediately because $v=2u$. Adding a third vector cannot remove the relation that already exists among $u$ and $v$. Therefore no determinant or linear-system calculation is necessary.

### Final answer

$$
v=2u,\qquad v-2u=0
$$

The vectors $u$, $v$, and $w$ are linearly dependent.
