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

---

> basis for a topology

see also:
- [[Metric Space]]

The concept of a **basis** for a topology is fundamental in the field of topology, serving as a building block from which a topology on a set can be constructed and understood. A basis provides a systematic way to generate all open sets of a topology, offering a simpler and more intuitive means of defining [[Topological Space|topological spaces]].

### Definition

Given a set $X$, a **basis** for a topology on $X$ is a collection $\mathcal{B}$ of subsets of $X$ (called **basis elements**) that satisfies the following two conditions:

1. **[[Covering]]**: For each $x \in X$, there is at least one basis element $B \in \mathcal{B}$ such that $x \in B$. In other words, the basis elements cover $X$.

2. **[[Intersection]] Property**: If $x$ belongs to the intersection of two basis elements, $B_1$ and $B_2$, then there is a basis element $B_3$ such that $x \in B_3$ and $B_3 \subseteq B_1 \cap B_2$.

### Generating a Topology from a Basis

Once a basis $\mathcal{B}$ for a topology on a set $X$ is specified, the topology $\mathcal{T}$ generated by $\mathcal{B}$ is defined as the collection of all subsets $U$ of $X$ for which, for each $x \in U$, there exists a basis element $B \in \mathcal{B}$ such that $x \in B$ and $B \subseteq U$. In essence, a set is open in the topology $\mathcal{T}$ if and only if it is a [[union]] of basis elements.

### Examples

1. **Standard Topology on $\mathbb{R}$**: The collection of all open intervals $(a, b)$, where $a < b$, serves as a basis for the standard topology on $\mathbb{R}$. This topology is equivalent to saying a set is open if, for every point in the set, there is an interval containing the point that is entirely within the set.

2. **Discrete Topology**: In any set $X$, the collection of all singletons $\{\{x\} : x \in X\}$ forms a basis for the discrete topology, the topology in which every subset of $X$ is open.

3. **Product Topology**: Given two topological spaces $(X_1, \mathcal{T}_1)$ and $(X_2, \mathcal{T}_2)$, the product topology on $X_1 \times X_2$ can be defined using the basis consisting of all products $U_1 \times U_2$, where $U_1 \in \mathcal{T}_1$ and $U_2 \in \mathcal{T}_2$.

### Properties and Significance

- **Efficiency**: Not every open set needs to be described individually; they can be generated from a simpler collection of sets.
- **Flexibility**: Different bases can generate the same topology, providing flexibility in how topologies are defined and studied.
- **Foundational**: Understanding the basis of a topology is crucial for exploring more advanced topological concepts such as continuity, compactness, and connectedness. It is also essential in the study of manifolds, where local properties are described in terms of bases of open sets.

The concept of a basis for a topology simplifies the study and understanding of topological spaces by focusing on a core collection of "building block" sets from which all open sets can be constructed. This approach not only streamlines the definition of topological spaces but also facilitates the exploration of their properties and the relationships between different spaces.