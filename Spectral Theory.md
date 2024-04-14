---
tags:
  - sod/gold
  - empty-hub
---
see also:
- [[Calculus of Variations]]
- [[Spectral Theory of Graphs]]
- [[Harmonic Analysis]]

Spectral theory is a fundamental branch of mathematics that studies the spectrum of operators, particularly linear operators acting on function spaces. Originating from the [[Analysis]] of [[differential operators]] and [[matrix theory]], spectral theory has grown to encompass a broad range of mathematical disciplines, including [[Functional Analysis]], [[partial differential equations]] (PDEs), and quantum mechanics. The "spectrum" of an operator includes values such as eigenvalues, around which the operator exhibits certain characteristic behavior, analogous to the way physical systems have natural frequencies at which they resonate.

### Core Concepts

- **[[Linear Operators]] and [[Eigenvalues]]:** At the heart of spectral theory is the study of linear operators, which are functions between vector spaces that preserve vector addition and scalar multiplication. An eigenvalue of a linear operator $A$ acting on a vector space is a scalar $\lambda$ such that there exists a non-zero vector $v$ (an eigenvector) for which $Av = \lambda v$. The set of all eigenvalues of $A$ is known as the spectrum of $A$.

- **[[Spectral Decomposition]]:** For certain classes of operators, it is possible to decompose the space into a direct sum or integral of subspaces that are invariant under the operator. This decomposition is closely related to the operator's spectrum and provides a way to understand the operator's action in terms of simpler, often one-dimensional, transformations.

- **[[Functional Calculus]]:** Spectral theory allows the extension of functions defined on numbers to functions of operators. For instance, if $f$ is a function and $A$ is an operator, one can define a new operator $f(A)$ in a manner that generalizes the polynomial calculus.

- **Self-Adjoint and [[Normal Operators]]:** In [[Hilbert Space]], operators that are equal to their [[adjoint]] (self-adjoint) or that commute with their adjoint (normal) have particularly well-understood spectral properties. For example, [[Hermitian Operators|self-adjoint operators]] have real spectra, and their [[Eigenvalues|eigenvectors]] corresponding to different eigenvalues are [[Orthogonality|orthogonal]].

### Applications

- **Quantum Mechanics:** Spectral theory is crucial in quantum mechanics, where operators on Hilbert spaces represent physical observables, and their spectra correspond to the possible measurement outcomes. The spectral decomposition of these operators is fundamental to the formulation and interpretation of the theory.

- **PDEs:** In the study of PDEs, spectral theory provides methods for solving linear PDEs by decomposing the space of functions into simpler components associated with the eigenvalues of an operator. This approach is instrumental in the analysis of wave, heat, and Schrödinger equations.

- **[[Signal Processing]]:** The [[Fourier transform]], a key tool in signal processing, can be understood through the spectral theory of the translation operator, with the frequency spectrum of a signal being directly related to the spectral properties of this operator.

- **[[Numerical Analysis]]:** Spectral methods for numerical analysis involve approximating the solution to [[Differential Equations]] by considering the [[spectral decomposition of operators]]. These methods are highly effective for certain classes of problems due to their accuracy and stability.

### Modern Developments

Spectral theory continues to evolve, with research extending into areas such as the spectral theory of non-self-adjoint operators, random matrix theory, and the study of spectral properties of operators on graphs and networks. The interplay between spectral theory and other areas of mathematics, as well as physics, engineering, and even computer science, demonstrates its foundational importance and broad applicability.