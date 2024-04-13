see also:
	- [[Observability (Systems Engineering)]]

Observability is a fundamental concept in control theory that assesses the ability to infer the full internal state of a system from its outputs over a finite time interval. In other words, a system is observable if, given the history of its outputs and inputs, one can determine the system's current state. This concept is crucial for the design and implementation of control systems, especially when the internal states of the system are not directly measurable but need to be estimated for effective control.

### Mathematical Formulation

Consider a linear time-invariant (LTI) system described by the state-space representation:

$$\dot{\mathbf{x}}(t) = \mathbf{A}\mathbf{x}(t) + \mathbf{B}\mathbf{u}(t)$$
$$\mathbf{y}(t) = \mathbf{C}\mathbf{x}(t) + \mathbf{D}\mathbf{u}(t)$$

where:
- $\mathbf{x}(t) \in \mathbb{R}^n$ is the state vector of the system at time $t$.
- $\mathbf{u}(t) \in \mathbb{R}^m$ is the input vector.
- $\mathbf{y}(t) \in \mathbb{R}^p$ is the output vector.
- $\mathbf{A}, \mathbf{B}, \mathbf{C}, \mathbf{D}$ are matrices of appropriate dimensions that define the system dynamics, input, output, and direct feedthrough, respectively.

#### Criteria for Observability

The system is said to be observable if, for any initial state $\mathbf{x}(0)$, the current state $\mathbf{x}(t)$ can be determined uniquely over a finite time interval by observing the output $\mathbf{y}(t)$ and knowing the input $\mathbf{u}(t)$.

For an LTI system, observability is commonly assessed using the [[Observability Matrix|observability matrix]] $\mathbf{O}$, defined as:

$$\mathbf{O} = \begin{bmatrix}
\mathbf{C} \\
\mathbf{C}\mathbf{A} \\
\mathbf{C}\mathbf{A}^2 \\
\vdots \\
\mathbf{C}\mathbf{A}^{n-1}
\end{bmatrix}$$

The system is observable if and only if the observability matrix $\mathbf{O}$ is of full rank, i.e., $\text{rank}(\mathbf{O}) = n$, where $n$ is the dimension of the state vector $\mathbf{x}(t)$.

### Implications of Observability

- **State Estimation**: Observability is a prerequisite for designing observers or estimators, such as the [[Kalman Filter]], which are algorithms that estimate the internal state of the system based on its outputs and inputs. These estimations are crucial for implementing state feedback control when some or all of the state variables are not directly measurable.
- **System Analysis and Design**: Understanding whether a system is observable is essential for system analysis and controller design, ensuring that the controller can effectively respond to the system's state.
- **Duality with Controllability**: Observability has a duality relationship with [[Controllability|controllability]]. Specifically, a system's observability can be analyzed through the controllability of its dual system, where the roles of the state, input, and output matrices are interchanged. This duality simplifies the analysis and design of control systems in many cases.

### Beyond Linear Systems

While the definitions and criteria provided above apply to linear systems, the concept of observability extends to nonlinear systems. In nonlinear systems, the criteria for observability are more complex and often require the use of differential geometry and Lie derivatives to assess whether the state can be inferred from the outputs. The analysis becomes more intricate due to the nonlinear dependencies between the state, input, and output.

In summary, observability is a critical concept in control theory, indicating the ability to deduce the entire state of a system from its outputs. This capability is fundamental for the successful design of state estimators and controllers, especially in complex or safety-critical systems where direct measurement of all state variables is impractical or impossible.