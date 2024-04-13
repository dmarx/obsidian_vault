Controllability is a fundamental concept in control theory that describes the ability to steer the state of a dynamical system to a desired final state within a finite time span, using an appropriate input or control signal. The concept of controllability is pivotal in designing controllers for dynamical systems because it delineates whether a system can achieve a desired performance or not.

### Mathematical Formulation

Consider a linear time-invariant (LTI) system described by the state-space equations:

$$\dot{\mathbf{x}}(t) = \mathbf{A}\mathbf{x}(t) + \mathbf{B}\mathbf{u}(t)$$
$$\mathbf{y}(t) = \mathbf{C}\mathbf{x}(t) + \mathbf{D}\mathbf{u}(t)$$

where:
- $\mathbf{x}(t) \in \mathbb{R}^n$ is the state vector of the system at time $t$.
- $\mathbf{u}(t) \in \mathbb{R}^m$ is the input (or control) vector.
- $\mathbf{y}(t) \in \mathbb{R}^p$ is the output vector.
- $\mathbf{A}, \mathbf{B}, \mathbf{C}, \mathbf{D}$ are matrices of appropriate dimensions that define the system dynamics, input, output, and feedthrough, respectively.

#### Criteria for Controllability

The system is said to be controllable if it is possible to transfer the state of the system from any initial state $\mathbf{x}(0)$ to any final state $\mathbf{x}_f$ in a finite time $T > 0$, using an appropriate control input $\mathbf{u}(t)$.

For an LTI system, a common method to assess controllability is through the [[Controllability Matrix|controllability matrix]] $\mathbf{C}_c$, defined as:

$$\mathbf{C}_c = [\mathbf{B}, \mathbf{A}\mathbf{B}, \mathbf{A}^2\mathbf{B}, \ldots, \mathbf{A}^{n-1}\mathbf{B}]$$

The system is controllable if and only if the controllability matrix $\mathbf{C}_c$ is of full rank, i.e., $\text{rank}(\mathbf{C}_c) = n$, where $n$ is the dimension of the state vector $\mathbf{x}(t)$.

### Implications of Controllability

- **Full State Control**: If a system is controllable, it implies that we can design control inputs that can drive the system to any desired state, making it possible to achieve various control objectives.
- **Design of Controllers**: Controllability is a precondition for the design of certain types of controllers, such as state feedback controllers, where the control input $\mathbf{u}(t)$ is designed as a function of the current state $\mathbf{x}(t)$ to achieve desired closed-loop behavior.
- **Observability and Duality**: The dual concept to controllability is [[Observability (Control Theory)|observability]], which concerns the ability to infer the complete state of the system from its outputs. The mathematical tools used to analyze controllability and observability are closely related due to this duality.

### Beyond Linear Systems

While the concept of controllability originally arose in the context of linear systems, it has been extended to nonlinear systems. For nonlinear systems, controllability is analyzed using more complex tools, such as Lie algebra and differential geometry. The main idea remains the same: assessing whether it is possible to drive the state of the system to a desired configuration using suitable controls. However, the criteria and methods for verification become significantly more complex due to the nonlinear nature of the system dynamics.

In summary, controllability is a core concept in control theory that plays a critical role in understanding the potential of a system to be controlled and in designing effective control strategies. Its analysis forms the foundation for further steps in control system design, including the synthesis of controllers that can achieve desired specifications and performances.