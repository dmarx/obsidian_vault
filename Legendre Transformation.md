The Legendre transformation is a mathematical operation that transforms one function into another, capturing the essence of a [[Change of Variables]] in optimization problems and in the formulation of physical theories. Named after the French mathematician [[Adrien-Marie Legendre]], this transformation is pivotal in moving between different formulations of classical mechanics (from [[Lagrangian Mechanics]] to [[Hamiltonian mechanics]]) and in [[thermodynamics]], where it facilitates the transition between different [[potential functions]].

### Definition and Mathematical Formulation

Given a function $f(x)$ that is convex and differentiable, the Legendre transform $g(p)$ of $f(x)$ is defined as:

$$
g(p) = \sup_{x} (px - f(x))
$$

where $\sup$ denotes the supremum, and $p = f'(x)$ is the derivative of $f$ with respect to $x$. The function $g(p)$ is a new function expressed in terms of the variable $p$, which is the slope of the tangent to the curve $y = f(x)$ at each point $x$.

In the context of classical mechanics, the Legendre transformation is used to switch between the [[Lagrangian]] $L(q,\dot{q},t)$, a function of the generalized coordinates $q$, their time derivatives $\dot{q}$, and time $t$, to the [[Hamiltonian]] $H(q,p,t)$, where $p$ is the conjugate momentum defined by $p = \partial L / \partial \dot{q}$.

### Key Properties

- **Invertibility**: The Legendre transformation is its own inverse (under suitable convexity conditions), meaning that applying it twice returns the original function (up to conventions).

- **Duality**: It establishes a duality between the variables $x$ and $p$, and between the functions $f(x)$ and $g(p)$. This duality is central in optimization and in the Hamiltonian formulation of mechanics, where it relates position and momentum.

### Applications in Physics

- **Classical Mechanics**: The Legendre transformation allows the transition from the Lagrangian, which is a function of positions and velocities, to the Hamiltonian, a function of positions and momenta. This transformation is essential for deriving Hamilton's equations of motion, which provide a powerful framework for analyzing the dynamics of physical systems.

- **Thermodynamics**: In thermodynamics, the Legendre transform is used to move between different thermodynamic potentials, such as moving from the internal energy to the Helmholtz free energy or the Gibbs free energy. Each potential is most useful for describing systems under different sets of conditions (e.g., constant temperature vs. constant entropy).

### Example in Mechanics

If the Lagrangian of a system is given by $L = T - V$, where $T$ is the kinetic energy and $V$ is the potential energy, the Hamiltonian $H$, representing the total energy, is obtained by the Legendre transform:

$$
H = p\dot{q} - L
$$

where $p = \partial L / \partial \dot{q}$ is the conjugate momentum to $q$. The Hamiltonian thus formulated is a function of $q$, $p$, and $t$, and serves as the starting point for Hamilton's equations.

The Legendre transformation's ability to bridge different mathematical descriptions of physical systems underscores its fundamental role in physics and mathematics, providing a unified approach to exploring and solving a wide range of problems across disciplines.