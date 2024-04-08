---
tags:
  - needs-outlinks
  - sod/green
---
Critical points are a fundamental concept in calculus and mathematical [[analysis]], particularly in the study of functions from $\mathbb{R}^n$ to $\mathbb{R}$. They play a crucial role in [[Optimization]], [[dynamical systems]], and the qualitative study of [[differential equations]] and [[manifolds]]. Understanding critical points allows us to analyze the behavior of functions, such as identifying local and global maxima or minima, and understanding the shape and [[topology]] of graphs and surfaces.

### Definition

For a function $f: \mathbb{R}^n \rightarrow \mathbb{R}$, a point $\mathbf{x}_0 \in \mathbb{R}^n$ is called a **critical point** if either:

1. The gradient of $f$ at $\mathbf{x}_0$ does not exist, or
2. The gradient of $f$ at $\mathbf{x}_0$ is equal to the zero vector, i.e., $\nabla f(\mathbf{x}_0) = \mathbf{0}$.

In simpler terms, critical points occur where the function doesn't change direction, meaning the rate of change (the derivative in one-dimensional cases, the gradient in multidimensional cases) is zero or undefined. 

### Classification of Critical Points

Once critical points are identified, they can be classified into various types based on the second derivative test (in one dimension) or the Hessian matrix (in higher dimensions):

- **Local Maxima:** The point at which $f$ attains a local maximum value, meaning $f$ decreases in every direction from that point.
- **Local Minima:** The point at which $f$ attains a local minimum value, meaning $f$ increases in every direction from that point.
- **[[Saddle Points]]:** In the multidimensional case, these are points where $f$ does not attain a local maximum or minimum but still has a flat slope. The function increases in some directions and decreases in others.

### Mathematical Formalism

For a function $f(x)$ in one dimension, the second derivative test involves examining $f''(x_0)$. If $f''(x_0) > 0$, then $f(x_0)$ is a local minimum; if $f''(x_0) < 0$, then $f(x_0)$ is a local maximum.

In higher dimensions, for a function $f: \mathbb{R}^n \rightarrow \mathbb{R}$, the classification is based on the [[Hessian]] matrix $H(f)$ at the critical point $\mathbf{x}_0$. The [[Hessian matrix]] is defined as a square matrix of second-order partial derivatives of $f$:

$$H(f)_{ij} = \frac{\partial^2 f}{\partial x_i \partial x_j}.$$

The nature of the critical point is determined by the eigenvalues of $H(f)$ at $\mathbf{x}_0$:

- If all [[Eigenvalues]] are positive, $\mathbf{x}_0$ is a local minimum.
- If all eigenvalues are negative, $\mathbf{x}_0$ is a local maximum.
- If eigenvalues are of mixed signs, $\mathbf{x}_0$ is a saddle point.
- If any eigenvalue is zero, the test is inconclusive, and further analysis is required.

### Applications

Critical points are used in various fields and applications:

- **Optimization:** Identifying the optimal values (maxima or minima) of functions in engineering, economics, and sciences.
- **Physics:** Analyzing [[potential energy surfaces]], stability of equilibria in dynamical systems.
- **[[Geometry]]:** Studying the topology and geometry of surfaces and manifolds, such as identifying points of [[Tangent Space|tangency]] or [[curvature]] properties.
- **Machine Learning:** Optimization of loss functions in training algorithms for neural networks and other models.

Understanding the concept of critical points is essential for analyzing and interpreting the behavior of mathematical functions and models across disciplines.