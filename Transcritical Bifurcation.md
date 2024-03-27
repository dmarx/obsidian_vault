---
tags:
  - green
  - needs-outlinks
---

A transcritical bifurcation is a type of bifurcation in dynamical systems where two equilibrium points exchange their stability as a parameter crosses a critical value. Unlike the saddle-node and pitchfork bifurcations, where equilibrium points appear or disappear, or split, in a transcritical bifurcation, the equilibria persist across the bifurcation point but swap their stability characteristics.

### Mathematical Description

Consider a dynamical system described by the differential equation:

$$
\frac{dx}{dt} = f(x, \mu),
$$

where $x$ represents the state of the system, $\mu$ is the bifurcation parameter, and $f(x, \mu)$ is a smooth function defining the system's dynamics. A transcritical bifurcation occurs at a parameter value $\mu = \mu_c$ if the function $f$ and its derivatives satisfy the following conditions at some point $x = x_c$:

1. **Bifurcation Condition**: $f(x_c, \mu_c) = 0$.
2. **Exchange of Stability**: At $\mu = \mu_c$, the derivative $\frac{\partial f}{\partial x}(x_c, \mu_c) = 0$, indicating that the slope of $f$ with respect to $x$ at the critical point is zero, a condition for exchange of stability.
3. **Non-Degeneracy Conditions**: $\frac{\partial^2 f}{\partial x \partial \mu}(x_c, \mu_c) \neq 0$ and $\frac{\partial^2 f}{\partial x^2}(x_c, \mu_c) \neq 0$, ensuring the bifurcation is non-degenerate and that there is a qualitative change in the system’s dynamics.

### Dynamics Near the Bifurcation

In a transcritical bifurcation, two equilibrium points intersect at the bifurcation point. As the parameter $\mu$ crosses the critical value $\mu_c$:

- One equilibrium point, which was stable before the bifurcation, becomes unstable after the bifurcation.
- The other equilibrium point, which was unstable before the bifurcation, becomes stable after the bifurcation.

This exchange of stability is the hallmark of the transcritical bifurcation, with both equilibria coexisting on either side of the bifurcation point but exchanging their stability properties.

### Examples and Applications

- **Population Dynamics**: A classic example is a simple population model where the growth rate changes sign at a critical population level, leading to a transcritical bifurcation. This can model scenarios where a population transitions from decline to growth as environmental conditions or resources improve.

- **Epidemiological Models**: In models for the spread of infectious diseases, a transcritical bifurcation can represent the threshold condition (basic reproduction number $R_0 = 1$) where the disease-free equilibrium exchanges stability with an endemic equilibrium, indicating the onset of an epidemic.

- **Chemical Reaction Dynamics**: In certain chemical reactions, the system may transition from one stable state to another as the concentration of a reactant or the rate of a reaction crosses a threshold, modeled by a transcritical bifurcation.

### Significance

The transcritical bifurcation provides insight into systems that undergo stability switching without the disappearance of equilibrium states. It is crucial for understanding threshold phenomena, where the system's qualitative behavior changes dramatically as parameters are varied, such as tipping points in ecological or climate systems. Identifying transcritical bifurcations in models helps predict critical transitions and devise strategies for controlling or avoiding undesirable states in complex systems.