# Exercise 15 — Classifying Three Systems

## Problem Statement

Use only as much elimination as needed to classify each system as having one solution, infinitely many solutions, or no solution:

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0. \\
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4. \\
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5. \\
\end{cases}
$$

## Objective

Recognize the three possible solution types from the equations' relationships after elimination.

## Concepts and Formulas

- A unique solution results when independent equations determine all variables.
- A redundant equation leaves a free variable and gives infinitely many solutions.
- A contradiction such as $0=c$, $c\ne0$, means no solution.

## Step-by-Step Solution

### System 1

Subtract the second equation from the first:

$$
(x+y)-(x-y)=2-0\quad\Longrightarrow\quad 2y=2,
$$

so $y=1$. Then $x-y=0$ gives $x=1$. Both variables are determined; there is one solution.

### System 2

The second equation is exactly twice the first, so it adds no new constraint. The remaining equation $x+y=2$ has infinitely many solutions, for example

$$
(x,y)=(2-t,t),\qquad t\in\mathbb R.
$$

### System 3

Twice the first equation gives $2x+2y=4$, but the second requires $2x+2y=5$. Subtraction produces $0=1$, so the system is inconsistent.

## Verification

System 1's point $(1,1)$ satisfies both equations. Every parametrized point for System 2 has sum $2$, satisfying both proportional equations. System 3 demands different values for the same expression, which cannot be satisfied.

## Final Answer

- System 1 has one solution: $(x,y)=(1,1)$.
- System 2 has infinitely many solutions: $(x,y)=(2-t,t)$ for $t\in\mathbb R$.
- System 3 has no solution.

## Key Takeaways

- Independent constraints can pin down a unique point.
- A redundant equation leaves freedom.
- Proportional left sides with incompatible right sides create a contradiction.
