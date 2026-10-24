## Exercise 14 — Rotation Matrices

### Problem Statement
The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

Explain the result geometrically.

### Objective
Multiply the rotation matrices and use the angle-sum identities to verify the resulting rotation angle.

### Concepts and Formulas
The angle-sum formulas are:

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
$$

$$
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

The product of rotation matrices corresponds to composing rotations.

### Step-by-Step Solution

#### Step 1 — Write the two matrices

$$
R(\alpha)=\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha \\
\end{pmatrix},\qquad
R(\beta)=\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta \\
\end{pmatrix}.
$$

#### Step 2 — Multiply them

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha \\
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta \\
\end{pmatrix}.
$$

Compute each entry:
- top-left:

$$
\cos\alpha\cos\beta+(-\sin\alpha)(\sin\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta.
$$

- top-right:

$$
\cos\alpha(-\sin\beta)+(-\sin\alpha)\cos\beta=-(\cos\alpha\sin\beta+\sin\alpha\cos\beta).
$$

- bottom-left:

$$
\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

- bottom-right:

$$
\sin\alpha(-\sin\beta)+\cos\alpha\cos\beta=\cos\alpha\cos\beta-\sin\alpha\sin\beta.
$$

Thus,

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta & -(\cos\alpha\sin\beta+\sin\alpha\cos\beta) \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta & \cos\alpha\cos\beta-\sin\alpha\sin\beta \\
\end{pmatrix}.
$$

#### Step 3 — Use angle-sum formulas
Applying the angle-sum identities gives:
- first entry becomes $\cos(\alpha+\beta)$
- second entry becomes $-\sin(\alpha+\beta)$
- third entry becomes $\sin(\alpha+\beta)$
- fourth entry becomes $\cos(\alpha+\beta)$
Hence,

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}
=R(\alpha+\beta).
$$

#### Step 4 — Geometric interpretation
A rotation through angle $\alpha$ followed by a rotation through angle $\beta$ is the same as a single rotation through angle $\alpha+\beta$.

This matches the idea that rotating a point in the plane twice is equivalent to one rotation by the sum of the angles.

### Final Answer

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

### Key Takeaways
- Composition of rotations corresponds to addition of angles.
- Matrix multiplication encodes geometric transformations in a compact algebraic language.
- The result is consistent with the standard angle-sum formulas.
