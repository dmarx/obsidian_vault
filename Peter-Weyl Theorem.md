---
tags:
  - gold
---

see also:
- [[Decomposition]]
- [[Harmonic Analysis]]
- [[Group Theory]]
- [[Stone–Weierstrass theorem]]
- [[Symmetry]]

The Peter-Weyl Theorem is a foundational result in the field of [[harmonic analysis on groups]], specifically focusing on [[compact topological groups]]. Named after mathematicians Hermann Weyl and Fritz Peter, the theorem provides a profound generalization of classical [[Fourier series]] to the setting of [[Compactness|compact]] groups. It plays a crucial role in understanding the structure of functions on these groups and in the development of [[representation theory]].

### Statement of the Peter-Weyl Theorem

Let $G$ be a compact topological group. The Peter-Weyl Theorem asserts that:

1. **Completeness**: The set of matrix coefficients of all finite-dimensional irreducible unitary representations of $G$ forms a [[complete orthogonal basis]] in the [[Hilbert space]] $L^2(G)$, the space of square-integrable functions on $G$ with respect to the Haar measure.

2. **Separability and Decomposition**: Every function in $L^2(G)$ can be decomposed into a (possibly infinite) sum of these matrix coefficients. This decomposition parallels the Fourier series expansion of periodic functions on the circle group $\mathbb{T}$, where functions are decomposed into sums of sines and cosines.

3. **Existence of Unitary Representations**: For every compact topological group $G$, there exists a rich family of finite-dimensional irreducible unitary representations. Moreover, each irreducible representation appears with multiplicity equal to its dimension in the regular representation of $G$.

### Implications and Applications

- **[[Orthogonality]] and [[Completeness]]**: The Peter-Weyl Theorem ensures that the space of square-integrable functions on a compact group can be understood in terms of the group's representations. This result is akin to saying that classical [[Fourier analysis]], which decomposes functions into sines and cosines, is just a special case of a more general phenomenon.

- **Harmonic Analysis on Compact Groups**: The theorem lays the foundation for harmonic analysis on compact groups, providing tools for analyzing functions on these groups, studying their symmetries, and solving differential equations invariant under group actions.

- **Representation Theory**: By demonstrating the existence and completeness of irreducible unitary representations, the Peter-Weyl Theorem is pivotal in the development of the representation theory of compact groups. It highlights the importance of these representations in understanding the structure and properties of groups.

- **Quantum Mechanics and Physics**: In theoretical physics, especially in quantum mechanics and quantum field theory, the representations of symmetry groups (often compact Lie groups) are essential for describing the states and behaviors of physical systems. The Peter-Weyl Theorem ensures that such descriptions can be systematically understood and classified.

- **Fourier Analysis and Signal Processing**: In a broader sense, the theorem underlines the [[universality]] of Fourier analysis techniques, extending their applicability from classical settings like $\mathbb{R}^n$ and the circle to arbitrary [[compact groups]]. This has implications for signal processing, data analysis, and other fields where symmetry and periodicity play a role.

The Peter-Weyl Theorem is a cornerstone of modern mathematics, bridging the worlds of algebra, analysis, and geometry, and providing a deep understanding of the harmonic analysis and representation theory of compact topological groups.


>how does the Pontryagin Duality relate to the Peter-Weyl theorem

The relationship between [[Pontryagin Duality]] and the [[Peter-Weyl Theorem]] reveals deep insights into the structure of locally compact groups and their representations. To understand this relationship, it's essential first to grasp the foundational concepts of both theorems within the realm of harmonic analysis and representation theory.

### Pontryagin Duality

Pontryagin Duality offers a profound perspective on the duality between locally compact abelian groups and their characters. A character of a locally compact abelian group $G$ is a continuous homomorphism from $G$ to the circle group $T = \{z \in \mathbb{C} : |z| = 1\}$. The collection of all such characters forms a group, denoted as $\hat{G}$, known as the dual group of $G$. Pontryagin Duality states that for any locally compact abelian group $G$, the double dual $\hat{\hat{G}}$ is isomorphic to $G$ itself, symbolically represented as $G \cong \hat{\hat{G}}$.

### Peter-Weyl Theorem

On the other hand, the [[Peter-Weyl Theorem]] concerns the representation theory of compact groups, not limited to abelian groups. It asserts that for any compact topological group $G$, the matrix elements of its irreducible unitary representations form a dense subset in the space of square-integrable functions on $G$, denoted $L^2(G)$. This theorem illustrates that compact groups can be "fully understood" through their representations, providing a comprehensive toolkit for analyzing their structure and symmetries.

### Relationship

The connection between Pontryagin Duality and the Peter-Weyl Theorem lies in their mutual exploration of group representations and duality principles, although in somewhat different settings. Here are the key points of intersection:

1. **Generalization of Fourier Analysis**: Both theorems can be viewed as far-reaching generalizations of classical Fourier analysis. Pontryagin Duality extends Fourier analysis to arbitrary locally compact abelian groups, while the Peter-Weyl Theorem does so for compact (possibly non-abelian) groups. In both scenarios, the group's dual (characters in the case of Pontryagin, irreducible representations in Peter-Weyl) plays a crucial role in decomposing functions into simpler, harmonically related components.

2. **Harmonic Analysis and Decomposition**: At their core, both theorems deal with the decomposition of functions into "harmonics" or basic building blocks associated with the group's structure. In Pontryagin Duality, this decomposition involves characters of the group. In contrast, the Peter-Weyl Theorem utilizes matrix coefficients of irreducible representations.

3. **Completeness and Duality**: Pontryagin Duality emphasizes a form of completeness or closure under duality, asserting that a group can be recovered from its dual. Similarly, the Peter-Weyl Theorem implies a completeness in the representation theory of compact groups, as every square-integrable function on the group can be approximated by linear combinations of matrix elements of its representations.

4. **Extension to Non-Abelian Groups**: While Pontryagin Duality is restricted to abelian groups, the Peter-Weyl Theorem extends some of these duality concepts to non-abelian groups, specifically compact ones. This transition showcases the broader applicability of duality and representation principles across different classes of groups.

In summary, Pontryagin Duality and the Peter-Weyl Theorem both illuminate the fundamental role of group representations in understanding the structure and functions on groups, albeit in complementary settings. Their relationship underscores the unity and diversity within harmonic analysis and representation theory, providing powerful tools for studying groups through their actions and symmetries.