---
tags:
  - sod/root
---

see also:
- [[Liouville's Theorem]]


Hamiltonian mechanics is a reformulation of classical mechanics that provides a powerful and elegant framework for describing the evolution of physical systems. Introduced by [[William Rowan Hamilton]] in the 19th century, it extends the work of Lagrange and others, offering a sophisticated approach to dynamics that is particularly suited to systems with complex interactions and constraints. Hamiltonian mechanics is fundamental in areas ranging from celestial mechanics to quantum mechanics, where its principles underpin the formulation of quantum theory.

### Key Concepts

- **[[Phase Space]]**: Unlike Newtonian mechanics, which focuses on the acceleration and forces acting on particles, Hamiltonian mechanics operates in phase space, a space defined by the canonical coordinates $(q, p)$, where $q$ represents the generalized positions of the system, and $p$ represents the corresponding momenta.

- **Hamiltonian Function**: At the core of Hamiltonian mechanics is the [[Hamiltonian]] function, $H(q, p, t)$, which typically represents the total energy of the system (kinetic plus potential energy) but can be more generally thought of as the generator of time evolution for the system. The Hamiltonian function's form depends on the system being studied and the choice of coordinates.

### Hamilton's Equations

The dynamics of a system in Hamiltonian mechanics are governed by Hamilton's equations, a set of first-order differential equations:

$$
\frac{dq_i}{dt} = \frac{\partial H}{\partial p_i}, \quad \frac{dp_i}{dt} = -\frac{\partial H}{\partial q_i}
$$

for $i = 1, 2, ..., n$, where $n$ is the number of degrees of freedom of the system. These equations describe how the positions and momenta change over time, capturing the essence of the system's dynamics.

### Properties and Applications

- **Conservation and Symmetries**: A fundamental aspect of Hamiltonian mechanics is its connection to [[conservation laws]] through symmetries of the Hamiltonian function, elegantly described by [[Noether's theorem]]. For example, if the Hamiltonian does not explicitly depend on time, the total energy is conserved.

- **[[Canonical Transformations]]**: Transformations in phase space that leave the form of Hamilton's equations invariant are called canonical transformations. They are a powerful tool for simplifying problems and finding conserved quantities.

- **Quantum Mechanics**: Hamiltonian mechanics forms the basis for the transition to quantum mechanics. The Hamiltonian function becomes the Hamiltonian operator, and Hamilton's equations are replaced by the Schrödinger equation, with Poisson brackets becoming commutators.

- **[[Analytical Mechanics]]**: Hamiltonian mechanics is a part of analytical mechanics, which also includes Lagrangian mechanics. The two formulations are equivalent under certain conditions and can be transformed into each other through the [[Legendre transformation]].

- **[[Integrable Systems]]**: Hamiltonian mechanics provides a framework for understanding integrable systems, where the existence of sufficient conserved quantities allows for the exact solution of the system's equations of motion.

### Modern Perspectives

Hamiltonian mechanics is not just a reformulation of classical mechanics but provides deep insights into the nature of physical systems, their symmetries, and conservation laws. It is extensively used in theoretical physics, especially in statistical mechanics, field theory, and the study of nonlinear dynamical systems, demonstrating its foundational role in our understanding of the physical world.

---

Hamiltonian mechanics reformulates the principles of [[Lagrangian Mechanics]] in terms of [[Energy]] rather than action. The central quantity is the Hamiltonian, $H$, which is often interpreted as the total energy of the system (kinetic plus potential energy). It is obtained through a [[Legendre Transformation]] of the [[Lagrangian]], changing the variables from generalized coordinates and velocities ($q_i, \dot{q}_i$) to generalized coordinates and momenta ($q_i, p_i$), where $p_i = \partial L / \partial \dot{q}_i$ are the conjugate momenta.

The equations of motion in Hamiltonian mechanics, known as Hamilton's equations, are:

$$
\dot{q}_i = \frac{\partial H}{\partial p_i}, \quad \dot{p}_i = -\frac{\partial H}{\partial q_i}
$$
