The Euler-Lagrange equation is a fundamental equation in the calculus of variations, offering a method to find the stationary points of a functional, which often represents the action in classical mechanics. These stationary points correspond to the paths or configurations of a system for which the action is extremized (minimized or maximized), which, in physical terms, corresponds to the natural motion of the system under the given forces.

### Derivation of the Euler-Lagrange Equation

Consider a functional $S$ defined by an integral of the form:

$$
S[q] = \int_{t_1}^{t_2} L(q(t), \dot{q}(t), t) \, dt
$$

where $L$ is the Lagrangian, $q(t)$ represents the generalized coordinates describing the system's state, and $\dot{q}(t)$ is the derivative of $q(t)$ with respect to time $t$. The aim is to find the function $q(t)$ that makes $S$ stationary (i.e., a minimum, maximum, or saddle point) under small variations.

To find this stationary point, we consider a small variation $\delta q(t)$ of the function $q(t)$, where $\delta q(t_1) = \delta q(t_2) = 0$ (the variations vanish at the endpoints). The variation of the action $\delta S$ due to this small change in $q(t)$ is given by:

$$
\delta S = S[q + \delta q] - S[q] = \int_{t_1}^{t_2} \left( L(q + \delta q, \dot{q} + \delta \dot{q}, t) - L(q, \dot{q}, t) \right) dt
$$

Expanding $L$ to first order in $\delta q$ and $\delta \dot{q}$, and requiring that $\delta S = 0$ for any arbitrary variation $\delta q(t)$, leads to the Euler-Lagrange equation:

$$
\frac{d}{dt} \left( \frac{\partial L}{\partial \dot{q}} \right) - \frac{\partial L}{\partial q} = 0
$$

### Interpretation and Applications

- **Classical Mechanics**: In the context of classical mechanics, the Euler-Lagrange equation derives the equations of motion for a system described by a Lagrangian $L(q,\dot{q},t)$. It encapsulates [[Newton's second law]] in a form that is directly applicable to a wide variety of mechanical systems, including those with constraints or non-Cartesian coordinates.

- **[[Field Theory]]**: The Euler-Lagrange equation generalizes to fields in physics, where $q(t)$ becomes a field $\phi(x,t)$ depending on both space and time, and the integral extends over space and time. The resulting Euler-Lagrange equation for fields is used to derive the field equations governing the dynamics of fields in classical and quantum field theories.

- **Optimization and Control**: Beyond physics, the Euler-Lagrange equation finds applications in optimization and control theory, where it helps in finding optimal paths or strategies subject to certain constraints or dynamics.

### Conclusion

The Euler-Lagrange equation is a cornerstone of theoretical physics and the calculus of variations, bridging the gap between abstract mathematical principles and the concrete laws governing the physical world. It provides a systematic approach to finding the laws of motion for a wide array of systems, from simple mechanical setups to complex field theories, embodying the principle that the dynamics of a system are determined by the [[Principle of Stationary Action]].