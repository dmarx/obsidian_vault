---
tags:
  - needs-outlinks
---
see also:
- [[Decomposition]]
- [[Factorization]]
- [[Matrix Factorization]]
- [[Sparsity]]
- [[Sparse Representation]]
- [[Representation Space]]
- [[Representation Learning]]
- [[Function Spaces]]
- [[Functional Analysis]]
- [[Harmonic Analysis]]

In mathematics, particularly in linear algebra, a basis is a set of vectors in a given vector space that is linearly independent and spans the space. This means two things: first, none of the vectors in the set can be written as a linear combination of the others (linear independence); and second, any vector in the vector space can be expressed as a linear combination of the vectors in the set (spanning property).

### Formal Definition

A set of vectors $\{v_1, v_2, ..., v_n\}$ in a vector space $V$ over a field $F$ (commonly the real numbers $\mathbb{R}$ or the complex numbers $\mathbb{C}$) is a basis of $V$ if:

1. **Linear Independence**: The only way to express the zero vector $\mathbf{0}$ as a combination of the basis vectors $\{v_1, v_2, ..., v_n\}$ is by scaling each vector by the zero scalar in $F$, i.e., if $a_1v_1 + a_2v_2 + ... + a_nv_n = \mathbf{0}$ implies that $a_1 = a_2 = ... = a_n = 0$.

2. **Spanning Property**: Every vector $v$ in $V$ can be expressed as a linear combination of the basis vectors, i.e., for every $v \in V$, there exist scalars $a_1, a_2, ..., a_n$ in $F$ such that $v = a_1v_1 + a_2v_2 + ... + a_nv_n$.

### Examples

- **Standard Basis for $\mathbb{R}^n$**: The standard basis for the Euclidean space $\mathbb{R}^n$ is given by the set of vectors where each vector has a $1$ in one coordinate and $0$ in all others. For $\mathbb{R}^2$, this is $\{(1, 0), (0, 1)\}$; for $\mathbb{R}^3$, it is $\{(1, 0, 0), (0, 1, 0), (0, 0, 1)\}$, and so on.

- **Polynomial Basis**: The set $\{1, x, x^2, x^3, ..., x^n\}$ forms a basis for the space of polynomials of degree at most $n$.

### Properties

- **Uniqueness of Representation**: Given a basis, every vector in the vector space can be uniquely represented as a linear combination of the basis vectors.

- **Change of Basis**: It's possible to transition between different bases of the same vector space. This transformation is facilitated by a matrix that relates the coordinates of vectors in one basis to their coordinates in another basis.

- **Dimension**: The number of vectors in a basis for a vector space $V$ is called the dimension of $V$, denoted as $\dim(V)$. All bases for a given vector space have the same number of elements, which is a fundamental theorem of linear algebra.

### Importance

The concept of a basis is central to the study of linear algebra and vector spaces because it provides a way to systematically describe and analyze the structure and properties of the space. Bases are used extensively in applied mathematics, physics, engineering, and computer science, for tasks ranging from solving systems of linear equations to performing transformations in graphics and data compression in signal processing.

Understanding and choosing an appropriate basis can significantly simplify the analysis of linear transformations, eigenvalue problems, and many other theoretical and practical problems in science and engineering.

>does the notion of "basis" only apply to vectors? what about a function basis? or maybe a basis over more abstract algebraic structures

The notion of a "basis" extends beyond just vectors in vector spaces; it is also a fundamental concept in the context of function spaces and more abstract algebraic structures. The unifying theme across these different contexts is that a basis provides a minimal set of elements from which any element of the space can be uniquely constructed through a linear combination (in vector spaces) or an analogous composition method relevant to the space in question.

### Function Spaces

In function spaces, a basis is a set of functions such that any function in the space can be expressed as a unique combination of these basis functions. Function spaces are vector spaces where the elements are functions, and the operations of vector addition and scalar multiplication are defined in terms of function addition and scalar multiplication of function values.

- **Example**: The set of functions $\{1, \cos(x), \sin(x), \cos(2x), \sin(2x), \ldots\}$ forms a basis for the space of square-integrable periodic functions on the interval $[-\pi, \pi]$ (i.e., the functions that can be expanded in a Fourier series). This is an example of an infinite-dimensional vector space, where the basis consists of infinitely many elements.

### Abstract Algebraic Structures

The concept of a basis can also be generalized to more abstract algebraic structures, such as free groups and free modules.

- **Free Groups**: In the context of group theory, a basis for a free group is a set of generators from which every element of the group can be uniquely constructed (up to the group's relations, which, in the case of a free group, are minimal). For example, the set $\{a, b\}$ can serve as a basis for the free group generated by two elements, where every element of the group can be written as a unique word in letters $a$, $a^{-1}$, $b$, and $b^{-1}$.

- **Free Modules**: A basis of a free module over a ring is a set of elements of the module such that every element of the module can be uniquely expressed as a linear combination of these basis elements, with coefficients from the ring. This generalizes the notion of a vector space basis, with the field of scalars replaced by a more general ring.

### Key Properties Across Contexts

Regardless of the context, the key properties that define a basis include:

- **Spanning Property**: The basis elements span the entire space, meaning every element of the space can be constructed from them.
- **Independence**: The basis elements are independent in a sense appropriate to the structure (linear independence in vector spaces, algebraic independence in abstract algebraic structures, etc.), meaning no basis element can be constructed from the others.

### Significance

Expanding the notion of a basis to function spaces and abstract algebraic structures enriches our ability to analyze and understand these spaces. It provides a systematic way to deconstruct and reconstruct elements of the space, simplifying the study of their properties and the operations defined on them. In each case, choosing an appropriate basis is crucial for effectively working within the space, whether for computational purposes, theoretical analysis, or applications to physics, engineering, and beyond.