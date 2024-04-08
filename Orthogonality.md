---
tags:
  - sod/green
  - needs-outlinks
---

see also:
- [[Orthogonality relations for the characters of irreducible representations of finite groups]]
- [[Independence]]

Orthogonality is a fundamental concept in mathematics and physics that signifies a form of independence or perpendicularity under a given inner product. Originating from geometry, where it describes perpendicular lines or planes, the concept has been vastly generalized to various branches of mathematics, including linear algebra, functional analysis, and beyond. In these broader contexts, orthogonality plays a crucial role in understanding the structure of spaces, simplifying problems, and developing efficient computational algorithms.

### In Euclidean Geometry

In classical Euclidean geometry, two vectors in $\mathbb{R}^n$ are orthogonal if their dot product is zero. For vectors $\mathbf{a} = (a_1, a_2, \ldots, a_n)$ and $\mathbf{b} = (b_1, b_2, \ldots, b_n)$, this means:
$$
\mathbf{a} \cdot \mathbf{b} = a_1b_1 + a_2b_2 + \cdots + a_nb_n = 0.
$$
This definition captures the intuitive idea of "perpendicularity" in higher dimensions.

### In Linear Algebra

Orthogonality extends to the study of vector spaces over any field, equipped with an inner product—a bilinear form that generalizes the dot product. Two vectors $\mathbf{v}$ and $\mathbf{w}$ in an inner product space are orthogonal if their inner product $\langle \mathbf{v}, \mathbf{w} \rangle$ is zero. Orthogonality is central to many concepts in linear algebra, including:

- **Orthogonal Sets and Bases**: A set of vectors is orthogonal if every pair of distinct vectors in the set is orthogonal. If, in addition, each vector in the set is non-zero, the set is orthonormal if it's orthogonal and each vector has a unit length. An orthonormal set that spans a vector space forms an [[Orthonormal Basis]], which simplifies computations and analyses within the space.
- **Orthogonal Matrices**: A square matrix $A$ is orthogonal if its rows and columns form an orthonormal basis of $\mathbb{R}^n$, implying $AA^T = A^TA = I$, where $I$ is the identity matrix, and $A^T$ is the transpose of $A$.

### In Functional Analysis

In functional analysis, which extends the concepts of linear algebra to infinite-dimensional spaces, orthogonality is defined similarly using the inner product of the space. It is crucial in the study of Hilbert spaces and Banach spaces, providing the foundation for Fourier series, orthogonal polynomials, and the spectral theory of operators.

### Applications

- **Signal Processing**: Orthogonal functions and transforms, such as the Fourier transform and orthogonal polynomials, are used to analyze and process signals and data, facilitating compression, noise reduction, and efficient information retrieval.
- **Quantum Mechanics**: The state space of a quantum system is a Hilbert space, where orthogonality of state vectors represents states with distinct measurements, reflecting the probabilistic nature of quantum measurements.
- **Numerical Methods**: Orthogonal matrices and vectors are used in numerical linear algebra to stabilize computations, reduce rounding errors, and improve the efficiency of algorithms, such as in QR factorization and singular value decomposition.

Orthogonality, with its geometric roots, permeates through various domains of mathematics and physics, embodying a principle of independence that informs both theory and practice. Its generalizations and applications underscore the unity and diversity of mathematical concepts across disciplines.

