see also:
- [[Orthogonality]]
- [[Basis]]
- [[Harmonic Analysis]]

An orthonormal basis is a fundamental concept in linear algebra and functional analysis, representing a set of vectors in a vector space or elements in a Hilbert space that are both orthogonal to each other and of unit length. This concept extends the intuitive geometric notion of perpendicular axes in Euclidean space to more abstract vector spaces, including infinite-dimensional spaces.

### Definition

In a vector space equipped with an inner product (an inner product space), a set of vectors $\{u_1, u_2, \ldots, u_n\}$ forms an **orthonormal basis** if:

1. **Orthogonality**: Each pair of distinct vectors is orthogonal, meaning the [[inner product]] $\langle u_i, u_j \rangle = 0$ for all $i \neq j$.
2. **Normality**: Each vector has a unit length, so $\langle u_i, u_i \rangle = 1$ for all $i$.

In the context of Euclidean spaces $\mathbb{R}^n$ with the standard dot product as the inner product, these conditions simplify to:

- $\mathbf{u}_i \cdot \mathbf{u}_j = 0$ for $i \neq j$,
- $\|\mathbf{u}_i\| = 1$ for all $i$,
where $\cdot$ denotes the dot product and $\|\cdot\|$ the Euclidean norm.

### Properties and Importance

- **Simplification**: Computations involving vectors or functions become significantly simpler in terms of an orthonormal basis due to the directness and independence of the basis elements.
- **[[Decomposition]]**: Any vector (or element) in the space can be uniquely expressed as a linear combination of the orthonormal basis vectors, with coefficients given by the inner product of the vector with each basis element. This is known as Fourier or spectral decomposition in more general contexts.
- **Stability**: In numerical computations, using orthonormal bases reduces issues related to numerical instability and improves the [[conditioning]] of problems.

### Applications

- **[[Fourier Series]]**: In the context of functions on an interval, the set of sines and cosines (or complex exponentials) forms an orthonormal basis for the space of square-integrable functions under the $L^2$ inner product, leading to the development of Fourier series.
- **Quantum Mechanics**: The state space of a quantum system is described by a [[Hilbert space]], where an orthonormal basis corresponds to a complete set of states that can be used to describe any state of the system.
- **[[Signal Processing]]**: Orthonormal bases of [[wavelets]] and other functions are used for analyzing and processing signals, facilitating efficient compression and noise reduction.
- **Computer Graphics**: In 3D computer graphics, orthonormal bases are used to describe the orientation and position of objects and cameras, simplifying calculations involving rotations and translations.

### Examples

- **[[Euclidean Space]]**: In $\mathbb{R}^3$, the standard basis vectors $e_1 = (1, 0, 0)$, $e_2 = (0, 1, 0)$, and $e_3 = (0, 0, 1)$ form an orthonormal basis.
- **Function Spaces**: In the space of square-integrable functions on the interval $[-\pi, \pi]$, the functions $\{\frac{1}{\sqrt{2\pi}}e^{inx}\}_{n=-\infty}^{\infty}$ form an orthonormal basis.

Orthonormal bases thus provide a powerful tool for analyzing and working within vector spaces and Hilbert spaces, offering clarity, efficiency, and insight across a wide spectrum of mathematical and physical disciplines.