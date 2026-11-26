## Exercise 1 — Vector Operations and Their Meaning

### Problem statement

For $u=(2,-1,3)$ and $v=(-1,4,2)$, compute $u+v$, $u-v$, and $3u-2v$. Verify that $(u+v)-v=u$, and explain geometrically what adding two vectors means.

### Formula used

Vector addition and subtraction are coordinate-wise:

$$
(a_1,a_2,a_3)+(b_1,b_2,b_3)=(a_1+b_1,a_2+b_2,a_3+b_3)
$$

$$
(a_1,a_2,a_3)-(b_1,b_2,b_3)=(a_1-b_1,a_2-b_2,a_3-b_3)
$$

Scalar multiplication multiplies every coordinate by the scalar:

$$
k(a_1,a_2,a_3)=(ka_1,ka_2,ka_3)
$$

This formula is used because linear combinations combine scaling and coordinate-wise addition.

### Solution

First add the vectors:

$$
u+v=(2+(-1),-1+4,3+2)=(1,3,5)
$$

The first coordinates, second coordinates, and third coordinates are added independently.

Next subtract $v$ from $u$:

$$
u-v=(2-(-1),-1-4,3-2)=(3,-5,1)
$$

For $3u-2v$, first scale each vector:

$$
3u=(6,-3,9)
$$

$$
2v=(-2,8,4)
$$

Then subtract corresponding coordinates:

$$
3u-2v=(6-(-2),-3-8,9-4)=(8,-11,5)
$$

### Verification

Reversing the addition with $v$ should recover $u$:

$$
(u+v)-v=(1,3,5)-(-1,4,2)
=(1-(-1),3-4,5-2)
=(2,-1,3)
=u
$$

The check returns the original vector, so the calculation is consistent.

### Geometric interpretation

Place the tail of $v$ at the head of $u$. The sum $u+v$ is the displacement from the original tail to the final head. If both vectors start at the same point, their sum is the diagonal of the parallelogram they span.

### Final answer

$$
u+v=(1,3,5)
$$

$$
u-v=(3,-5,1)
$$

$$
3u-2v=(8,-11,5)
$$
