---
tags:
  - sod/gold
---
see also:
- [[Harmonic Analysis]]

Character theory is a cornerstone of [[representation theory]], particularly for finite groups, providing a powerful and elegant way to study and classify group representations through the use of characters. A character is a complex-valued function defined on a group that encapsulates significant information about the representation from which it is derived.

### Definition and Basic Concepts

- **[[Group Representation]]**: A representation of a group $G$ on a [[vector space]] $V$ over a field $F$ (commonly $\mathbb{C}$, the [[complex numbers]]) is a [[homomorphism]] $\rho: G \to GL(V)$, where $GL(V)$ is the group of invertible linear transformations from $V$ to itself. In simpler terms, it is a way of representing group elements as matrices such that the group operation corresponds to matrix multiplication.

- **Character**: The character $\chi$ associated with a representation $\rho$ of a group $G$ is a function $\chi: G \to \mathbb{C}$ defined by $\chi(g) = \text{Tr}(\rho(g))$, where $\text{Tr}$ denotes the trace of a matrix (the sum of its diagonal elements). Characters are constant on conjugacy classes of $G$, making them class functions.

### Properties

- **[[Orthogonality relations for the characters of irreducible representations of finite groups|Orthogonality Relations]]**: The characters of irreducible representations of a finite group satisfy certain orthogonality relations, which are instrumental in their study. These relations allow for the decomposition of representations and the counting of irreducible representations.

- **Dimension**: The value of a character at the identity element of $G$ is equal to the dimension of the representation space. This provides a straightforward way to determine the dimension from the character.

- **Irreducibility**: A representation is irreducible if its only invariant subspaces are trivial (the zero space and the entire space). The irreducibility of a representation can be determined by its character, using the inner product of characters.

### Applications and Significance

- **Classification of Representations**: Character theory allows for the classification of all irreducible representations of a finite group up to [[isomorphism]]. This classification is crucial for understanding the structure of groups and for applications in physics, chemistry, and beyond.

- **[[Group Decomposition]]**: Through the study of characters, it's possible to decompose any representation of a finite group into irreducible components. This decomposition is fundamental in the analysis of [[symmetry]] and the structure of physical systems.

- **Theorems and Results**: Various important theorems in representation theory are stated and proved using character theory, including [[Burnside's lemma]], [[Frobenius-Schur indicators]], and more.

- **Chemistry and Physics**: Character theory is used in quantum chemistry and physics to analyze the symmetry properties of molecules and to predict physical properties like the selection rules for spectral lines.

- **Number Theory and Algebra**: Character theory has applications in number theory, algebraic geometry, and other areas of algebra, where the structure of groups and their actions on other objects are of interest.

Character theory provides a unifying language for studying representations of finite groups, elucidating the connection between group structure and linear algebraic actions. It's a testament to the depth and beauty of mathematical structures, showcasing how abstract algebraic concepts can have wide-ranging applications in understanding the symmetries of the natural world.