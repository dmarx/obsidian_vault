---
tags:
  - green
  - gold
---

The principle of stationary action, also known as the principle of least action, is a foundational concept in physics and the calculus of variations, serving as the bedrock for classical mechanics, optics, quantum mechanics, and quantum field theory. It posits that the path taken by a physical system between two points in its configuration space is the one for which the action is stationary—meaning it is at a local minimum, maximum, or saddle point.

### Definition of Action

The [[action]], $S$, is a [[functional]], which means it takes a function (the system's path through its configuration space) as input and returns a scalar. It is defined as the [[integral]] over time of the [[Lagrangian]], $L$, of the system:

$$
S[q] = \int_{t_1}^{t_2} L(q(t), \dot{q}(t), t) \, dt
$$

Here, $q(t)$ represents the generalized coordinates of the system (which can be positions, angles, or field values), $\dot{q}(t)$ are their time derivatives, and $L$ is the difference between the kinetic and potential energies for classical systems.

### Statement of the Principle

The principle of stationary action states that the actual path taken by a system between two points in time, $t_1$ and $t_2$, is the one that makes the action, $S$, stationary with respect to variations of the path $q(t)$. That is, if you make a small change $\delta q(t)$ to the path, with the condition that $\delta q(t_1) = \delta q(t_2) = 0$ (the endpoints are fixed), the first variation of the action $\delta S$ is zero:

$$
\delta S = 0
$$

### Implications and Applications

- **Equations of Motion**: The requirement that $\delta S = 0$ for arbitrary variations leads directly to the [[Euler-Lagrange equations]], which are the equations of motion for the system. This demonstrates how the dynamics of a system are derived from a variational principle rather than postulated directly.
  
- **Generalization**: The principle applies not just to mechanical systems but also to fields in physics. For field theories, the [[Lagrangian]] depends on field values and their derivatives, and the action involves an integral over space and time. The principle of stationary action leads to field equations that govern the dynamics of these fields.

- **Quantum Mechanics**: In quantum mechanics, the principle of stationary action underlies the path integral formulation, where the probability amplitude for a particle to transition from one state to another is given by a sum (or integral) over all possible paths, weighted by $\exp(iS/\hbar)$, where $S$ is the action for each path, and $\hbar$ is the reduced Planck constant. This highlights the fundamental role of the action in quantum as well as classical physics.

- **[[Symmetry|Symmetries]] and [[Conservation Laws]]**: Noether's theorem connects symmetries of the action to [[Conservation Laws]]. For each [[Continuity|continuous]] symmetry of the [[Action]], there is a corresponding conserved quantity. This profound link shows that the conservation laws of physics are not arbitrary but arise from the symmetrical properties of the underlying action.

### Conclusion

The principle of stationary action is a unifying concept in physics, encapsulating the dynamics of a vast range of physical systems in a single, elegant mathematical statement. It illustrates how the laws of motion and field equations can be derived from a principle of optimality, with far-reaching implications across many areas of theoretical physics.