# Repository Instructions

For all exercise sheets, hints, and solutions written or edited in this repository, follow the GitHub Markdown and mathematics rendering rules in `hints.md`.

In particular:

- Use `$...$` for inline math and standalone `$$` blocks for display math, with blank lines around display blocks.
- Format matrices with multiline `pmatrix` rows and systems with multiline `cases` rows.
- Do not use `\(...\)`, `\[...\]`, `\boxed`, `\text`, `\operatorname`, or other macros and environments disallowed by `hints.md`.
- Keep multiline environments out of inline math and avoid bare punctuation lines inside display math.
- Before finishing, check the rendered Markdown when feasible and run the formatting checks from `hints.md`.

## Solution Methodology

When writing or editing a solution for an exercise, use an explanation-first structure that makes every mathematical action understandable.

### Required structure

For each solution, include, where applicable:

1. A clear problem statement.
2. A named list of lettered quantities used in the solution.
3. Each formula, condition, or property introduced immediately before it is first used.
4. A numbered or clearly labeled step for each computation.
5. Formula substitution using the identified letters and coordinate components.
6. One or more result checks or independent verification steps.
7. A geometric or conceptual interpretation when the exercise has a geometric meaning.
8. A concise final answer.

### Lettered quantities

Before calculations begin, define the symbols used in the solution.

Examples:

- Define vectors such as $\vec p=\overrightarrow{AB}$ and $\vec q=\overrightarrow{AC}$.
- Define areas such as $A_{\mathrm{parallelogram}}$ and $A_{\triangle ABC}$.
- Define the components of a vector, for example $\vec p=(p_1,p_2,p_3)$.
- Define points, lengths, angles, coefficients, normals, or other quantities before substituting them.

Do not introduce an important symbol only in a formula without first stating what it represents.

### Formula usage

Do not put a detached catalogue of formulas before the solution steps. Introduce each formula, condition, or property directly before the computation or reasoning step where it is used. Give it a descriptive name when that helps the reader, and explain briefly:

- What mathematical quantity it computes or what condition it tests.
- What the lettered quantities mean in this use.
- Why it applies to the current step.

If a formula or property is used again in the same solution, give a short reminder of its role rather than restating the full explanation.

### Computation steps

Separate each main calculation into named steps. Immediately before a computation, state and explain the formula, condition, or property being applied, and identify the components that will be substituted.

Preferred pattern:

```markdown
#### Step 1 - Compute the requested vector

The vector from $X$ to $Y$ is $Y-X$, because subtracting the starting point's coordinates from the endpoint's coordinates gives the displacement. Use $X=A$ and $Y=B$:

$$
\overrightarrow{AB}=B-A=(...)
$$
```

Show intermediate algebra rather than only presenting the final number. This includes:

- Coordinate differences.
- Dot-product terms.
- Scalar-multiplication coefficients.
- Cross-product components.
- Length and area calculations.
- Equation substitutions.

### Verification

Whenever the exercise permits it, verify the result using an independent check. Examples include:

- Checking vector reconstruction.
- Checking perpendicularity with a dot product.
- Reconstructing a target vector from coefficients.
- Checking that a plane normal is perpendicular to two in-plane vectors.
- Checking that a residual is perpendicular to the line direction.

Explain briefly what each check proves.

### Commentary

Use concise commentary around formulas and calculations to explain:

- Why a formula applies.
- What each symbol means.
- What operation is being performed.
- What result the step proves.
- What geometric interpretation follows.

Avoid filler such as "Now", "As you can see", or "Let's solve this".
