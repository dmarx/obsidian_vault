---
tags:
  - gold
---

see also:
- [[Group Representation Theory]]
- [[Decomposition]]

The group algebra is a unifying structure in mathematics that blends [[group theory]] with [[linear algebra]], providing a powerful framework for studying groups and their representations. It plays a crucial role in [[representation theory]], [[harmonic analysis]], and other areas where groups and [[Vector Space|vector spaces]] intersect.

### Definition

Given a group $G$ and a field $F$, the group algebra $F[G]$ is a [[vector space]] over $F$ with a [[basis]] consisting of the elements of $G$. This vector space is also equipped with a multiplication operation that extends the group operation linearly.

Formally, elements of $F[G]$ are formal sums of the form
$$
\sum_{g \in G} a_g g,
$$
where $a_g \in F$ for all $g \in G$, and only finitely many $a_g$ are non-zero. The addition in $F[G]$ is defined component-wise, and the multiplication is defined by distributively extending the group operation, making $F[G]$ an algebra over $F$.

### Properties

- **Algebra Structure**: $F[G]$ is an [[associative algebra]] with the identity element being the identity of the group $G$ with a coefficient of 1. It's associative because the group operation is associative, and it respects the scalar multiplication of the field $F$.

- **Dimensionality**: If $G$ is a finite group of [[Order of a Group|order]] $n$, then $F[G]$ is an $n$-dimensional vector space over $F$. Each group element corresponds to a basis vector in this vector space.

- **Center of $F[G]$**: The [[Center Of The Group Algebra]], denoted $Z(F[G])$, consists of all elements in $F[G]$ that commute with every element of $F[G]$. These often correspond to sums over conjugacy classes in $G$ and have special significance in the study of representations.

### Applications

- **Representation Theory**: The group algebra forms the foundational setting for studying group representations. Representations of $G$ can be equivalently viewed as [[algebra homomorphisms]] from $F[G]$ to the algebra of matrices over $F$. This perspective is particularly useful for classifying and decomposing representations.

- **[[Harmonic Analysis]]**: In harmonic analysis, especially when $G$ is a [[finite group]] or a [[compact Lie group]], the group algebra serves as a domain for the Fourier transform on $G$, allowing for the analysis and synthesis of functions on $G$.

- **Non-commutative Geometry and Quantum Groups**: In more advanced settings, group algebras, especially those associated with infinite or quantum groups, play a role in [[non-commutative geometry]], where they help generalize geometric concepts to algebraic settings lacking a conventional space.

### Example

For a simple example, consider the group $\mathbb{Z}/2\mathbb{Z} = \{0, 1\}$ with addition modulo 2, and let $F = \mathbb{R}$. The group algebra $\mathbb{R}[\mathbb{Z}/2\mathbb{Z}]$ consists of all real linear combinations of the elements $0$ and $1$, which can be thought of as the set of all vectors $\{a\cdot0 + b\cdot1 | a, b \in \mathbb{R}\}$. Multiplication in this algebra reflects the group structure, so, for example, $1\cdot1 = 0$ because $1 + 1 = 0 \mod 2$.

The group algebra encapsulates both the algebraic structure of the group and the linear structure of the field, serving as a bridge between abstract group theory and the more concrete world of linear algebra and vector spaces.