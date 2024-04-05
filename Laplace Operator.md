---
tags:
  - empty-hub
  - green
---

see also:
- [[Laplacian]] (aka)
- [[Graph Laplacian]]

The Laplace operator, denoted by $\Delta$, is a second-order [[differential operator]] that plays a central role in mathematics, particularly in the fields of [[differential geometry]], [[analysis]], and [[mathematical physics]]. It is defined as the [[divergence]] of the [[gradient]] of a function, encapsulating a measure of the rate at which the average value of the function diverges from its value at a point. The Laplace operator provides critical insights into the behavior of scalar fields and appears in numerous physical laws and equations, including [[Laplace's equation]], the [[heat equation]], and the [[Schrödinger equation]].

### Definition

In Cartesian coordinates for a function $f(x, y, z)$ of three variables, the Laplace operator is defined as:

$$\Delta f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2}$$

This extends naturally to $n$ dimensions for a function $f(x_1, x_2, ..., x_n)$:

$$\Delta f = \sum_{i=1}^{n} \frac{\partial^2 f}{\partial x_i^2}$$

### Laplace's Equation

A fundamental application of the Laplace operator is in Laplace's equation:

$$\Delta f = 0$$

This equation describes [[stationary]] (time-independent) situations in which there is [[Conservation Laws|no change in the quantity]] described by $f$ at the point where the equation is evaluated. It arises in contexts such as electrostatics, gravitational fields, and fluid dynamics, where it characterizes potential fields in free space.

### Properties and Applications

- **[[Harmonic Functions]]:** Functions that satisfy Laplace's equation are known as harmonic functions. They have numerous nice properties, including the mean value property, which states that the value of a harmonic function at a point is equal to the average of its values on any sphere centered at that point.

- **[[Heat Equation]]:** The Laplace operator also appears in the heat equation, which describes the distribution of heat (or variation in temperature) in a given region over time:

  $$\frac{\partial u}{\partial t} = \Delta u$$

  where $u$ is the temperature distribution function.

- **Quantum Mechanics:** In quantum mechanics, the Laplace operator appears in the Schrödinger equation, governing the behavior of quantum particles:

  $$i\hbar \frac{\partial \psi}{\partial t} = -\frac{\hbar^2}{2m}\Delta \psi + V \psi$$

  where $\psi$ is the wave function of the particle, $\hbar$ is the reduced Planck constant, $m$ is the mass of the particle, and $V$ is the potential energy.

- **Generalizations:** In more general spaces, such as on surfaces or in manifolds, the Laplacian can be defined in terms of the [[intrinsic geometry]] of the space, using the [[metric tensor]]. In these cases, the [[Laplace-Beltrami operator]] generalizes the notion of the Laplace operator.

The Laplace operator encapsulates the essence of [[diffusion processes]], [[potential theory]], and [[wave propagation]], among others. Its ubiquity across the mathematical sciences underscores its fundamental importance in describing natural phenomena and the behavior of functions across space.

---

The Laplacian operator is a fundamental differential operator in mathematics, particularly in the fields of calculus, differential equations, and physics. It is denoted by $\nabla^2$ and represents the divergence of the gradient of a function. The Laplacian provides a measure of the rate at which the average value of a function changes around a point, relative to changes in the function at that point. It plays a critical role in various physical laws and equations, including those describing electromagnetism, heat transfer, and fluid dynamics.

### Definition

In a three-dimensional Euclidean space with coordinates $(x, y, z)$, the Laplacian of a scalar function $f(x, y, z)$ is defined as:

$$
\nabla^2 f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2}
$$

This expression involves the second partial derivatives of the function with respect to each of its variables, summing them up to get the Laplacian. The operation measures the difference between the value of $f$ at a point and the average value of $f$ around that point, indicating how $f$ "curves" in space.

### Generalizations

The Laplacian can be generalized to other coordinate systems and higher dimensions:

- **In Two Dimensions**: For a function $f(x, y)$, the Laplacian is $\nabla^2 f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2}$.
- **In Polar Coordinates**: The Laplacian takes the form $\nabla^2 f = \frac{1}{r}\frac{\partial}{\partial r}\left(r\frac{\partial f}{\partial r}\right) + \frac{1}{r^2}\frac{\partial^2 f}{\partial \theta^2}$.
- **On Surfaces or Manifolds**: The Laplace-Beltrami operator generalizes the Laplacian to curved spaces, incorporating the geometry of the space into the operator.

### Applications

#### Physics and Engineering

- **Heat Equation**: The Laplacian appears in the heat equation, $\frac{\partial u}{\partial t} - \alpha \nabla^2 u = 0$, describing how heat diffuses through a medium over time.
- **Poisson's Equation**: In electrostatics, Poisson's equation, $\nabla^2 \phi = -\frac{\rho}{\epsilon_0}$, relates the electric potential $\phi$ to the charge density $\rho$, where $\epsilon_0$ is the vacuum permittivity.
- **Wave Equation**: The Laplacian is found in the wave equation, describing how waves propagate through a medium.

#### Mathematics

- **Harmonic Functions**: Functions that satisfy Laplace's equation, $\nabla^2 f = 0$, are called harmonic functions and are crucial in potential theory and complex analysis.
- **Eigenvalue Problems**: The Laplacian operator is central to solving eigenvalue problems in mathematical physics and spectral geometry.

### Properties

- **Linearity**: The Laplacian is a linear operator, meaning that $\nabla^2 (af + bg) = a\nabla^2 f + b\nabla^2 g$ for any scalar functions $f$ and $g$, and constants $a$ and $b$.
- **Rotation Invariance**: The Laplacian of a function is invariant under rotations of the coordinate system, reflecting its geometric nature.

The Laplacian operator encapsulates the essence of diffusion, wave propagation, and potential theory across mathematics and physics, serving as a bridge between the geometry of a space and the behavior of functions within that space.