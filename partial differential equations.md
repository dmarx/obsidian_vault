see also: 
- [[Fundamental Partial Differential Equations]]
- [[Ordinary Differential Equations]]

Partial Differential Equations (PDEs) are mathematical equations that involve functions of multiple variables and their partial derivatives. They are fundamental in expressing a wide range of physical phenomena where change occurs in more than one direction, such as the propagation of sound or heat, fluid flow, and the behavior of electromagnetic fields. PDEs are crucial in engineering, physics, finance, and many other disciplines for modeling complex systems and understanding dynamical processes.

### Basic Concepts

A PDE is an equation involving a function of several independent variables (e.g., time, spatial coordinates) and its partial derivatives with respect to those variables. The order of a PDE is determined by the highest-order partial derivative that appears in the equation.

- **First-Order PDE**: Involves only first-order derivatives of the unknown function. A general form for a first-order PDE in two variables is: $$a(x, y) \frac{\partial u}{\partial x} + b(x, y) \frac{\partial u}{\partial y} = c(x, y)$$ where $u = u(x, y)$ is the unknown function, and $a$, $b$, and $c$ are given functions of $x$ and $y$.
- **Second-Order PDE**: Involves second-order derivatives. A widely studied second-order PDE is the [[Laplace equation]]: $$\nabla^2 u = 0$$ where $\nabla^2$ denotes the Laplacian operator, indicating a sum of second-order partial derivatives.

### Classification of Second-Order PDEs

Second-order PDEs can be classified based on the form of their highest-order terms into three main types:

1. **Elliptic PDEs**: Characterized by having no real characteristic curves that solutions can propagate along, implying steady-state or equilibrium conditions. The Laplace equation $\nabla^2 u = 0$ and the Poisson equation $\nabla^2 u = f$ are classic examples, important in electrostatics, fluid dynamics, and steady-state heat transfer.

2. **Parabolic PDEs**: These describe phenomena where there is a time-dependent diffusion process, such as heat conduction. The [[heat equation]], given by $$u_t = \alpha\nabla^2 u$$ where $u_t$ denotes the partial derivative of $u$ with respect to time $t$ and $\alpha$ is a positive constant, is a fundamental example.

3. **Hyperbolic PDEs**: Govern wave propagation and dynamics in systems where speeds are finite and can be associated with characteristic lines. The [[wave equation]], $$u_{tt} = c^2 \nabla^2 u$$ where $u_{tt}$ is the second partial derivative of $u$ with respect to time, models the displacement of a wave at a point in space over time.

### Methods of Solution

Solving PDEs involves finding functions that satisfy the equations, subject to given boundary and initial conditions. The complexity of PDEs means that analytical solutions are not always possible, leading to the development of various numerical methods for their approximation, including:

- **[[Finite Difference Method]] (FDM)**: Approximates derivatives by differences and solves the PDE over a discrete grid.
- **[[Finite Element Method]] (FEM)**: Decomposes the domain into elements and approximates the solution by piecewise functions.
- **[[Boundary Element Method]] (BEM)**: Focuses on solving boundary integral equations, reducing the dimensionality of the problem.

### Applications

- **Fluid Dynamics**: The [[Navier-Stokes equations]], a set of nonlinear PDEs, describe the motion of fluid substances and are fundamental in aerodynamics, oceanography, and meteorology.
- **Quantum Mechanics**: The Schrödinger equation is a second-order partial differential equation that describes how the quantum state of a physical system changes over time.
- **General Relativity**: The Einstein field equations, a system of nonlinear PDEs, form the core of Einstein's general theory of relativity, relating the geometry of spacetime to the distribution of matter within it.
- **Economics and Finance**: The [[Black-Scholes equation]] models the price evolution of financial derivatives, helping in options pricing and risk management.

The study of PDEs is a vast and deeply developed field within mathematics and applied sciences, continuously expanding its reach and applications in understanding and designing complex systems across disciplines.