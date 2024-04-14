---
aliases:
  - Linearity
  - linearity
---

**Linear operators** are a fundamental concept in linear algebra, functional analysis, and many areas of mathematics and engineering. They generalize the notion of linear transformations between vector spaces, extending their application to spaces of functions and other mathematical objects. Linear operators are critical in understanding structures and solving equations in many mathematical contexts, including differential equations, transformations in physics, and systems theory in engineering.

### Definition

A linear operator \( T \) is a mapping between two vector spaces \( V \) and \( W \) over the same field \( \mathbb{F} \) (typically \( \mathbb{R} \) or \( \mathbb{C} \)), such that for all vectors \( x, y \in V \) and all scalars \( a \in \mathbb{F} \), the following conditions hold:

1. **Additivity:** \( T(x + y) = T(x) + T(y) \)
2. **Homogeneity:** \( T(ax) = aT(x) \)

These properties ensure that the operator \( T \) preserves the vector space structure.

### Examples and Types

1. **Matrix Operators:** In finite dimensions, any linear operator \( T: \mathbb{R}^n \to \mathbb{R}^m \) can be represented by a matrix \( A \in \mathbb{R}^{m \times n} \). The action of \( T \) on a vector \( x \in \mathbb{R}^n \) is given by matrix multiplication \( Ax \).

2. **Differential Operators:** In functional analysis, differential operators such as \( \frac{d}{dx} \) are linear operators on function spaces like \( C^1(\mathbb{R}) \) (the space of continuously differentiable functions). These operators play a critical role in solving differential equations.

3. **Integral Operators:** Operators defined by an integral, such as \( (Tf)(x) = \int_{a}^{b} K(x, y) f(y) dy \), where \( K \) is a kernel function, are integral linear operators. They are essential in solving integral equations and in the study of kernels in machine learning.

### Properties

- **Kernel and Image:** For a linear operator \( T: V \to W \),
  - The **kernel** (or null space) of \( T \), denoted \( \ker T \), is the set of all vectors in \( V \) that map to the zero vector in \( W \): \( \ker T = \{ x \in V : T(x) = 0 \} \).
  - The **image** (or range) of \( T \), denoted \( \text{im} T \), is the set of all vectors in \( W \) that are images of vectors in \( V \): \( \text{im} T = \{ T(x) : x \in V \} \).

- **Invertibility:** A linear operator \( T \) is invertible if there exists an operator \( S: W \to V \) such that \( ST = I_V \) and \( TS = I_W \), where \( I_V \) and \( I_W \) are the identity operators on \( V \) and \( W \), respectively. Invertibility requires that \( T \) is bijective (one-to-one and onto).

- **Adjoints:** In the context of Hilbert spaces, the adjoint of a linear operator \( T \) is another operator \( T^* \) that satisfies \( \langle Tx, y \rangle = \langle x, T^*y \rangle \) for all \( x \in V \) and \( y \in W \), where \( \langle \cdot, \cdot \rangle \) denotes the inner product.

### Applications

Linear operators are ubiquitous in both theoretical and applied mathematics:
- In quantum mechanics, observables are represented by self-adjoint linear operators on Hilbert spaces.
- In control theory, systems are often modeled by linear operators defining the relationship between inputs and outputs.
- In image processing, transformations applied to images can be represented as linear operators, especially in the context of filtering and reconstruction.

Understanding linear operators and their properties is crucial for advanced studies in mathematics, physics, and engineering, providing tools for both analysis and synthesis of models in numerous applications.