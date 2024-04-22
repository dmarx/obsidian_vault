### Phase Plane Analysis: Overview

**Phase plane analysis** is a powerful qualitative tool used in the study of dynamical systems described by differential equations, particularly those involving two variables. This analysis involves plotting the trajectories of the system in a plane defined by its variables, usually referred to as the state variables. These plots help visualize how the system evolves over time from different initial conditions, revealing the nature of fixed points, stability, and the occurrence of phenomena such as limit cycles, bifurcations, and other complex behaviors.

### Mathematical Background

In a two-dimensional system, let's consider a general form of a system of first-order ordinary differential equations (ODEs):

$$\frac{dx}{dt} = f(x, y), \quad \frac{dy}{dt} = g(x, y)$$

where \( x \) and \( y \) are the state variables, and \( f \) and \( g \) are functions that describe the system's dynamics.

### Key Concepts in Phase Plane Analysis

1. **[[Nullclines]]**: These are curves in the phase plane where the derivative of either state variable is zero. The nullclines are given by \( f(x, y) = 0 \) and \( g(x, y) = 0 \). They are useful because their intersections typically indicate [[fixed points]] (equilibria) of the system.
   
2. **Fixed Points**: Points in the phase plane where \( \frac{dx}{dt} = 0 \) and \( \frac{dy}{dt} = 0 \) simultaneously. At these points, the system does not change, indicating possible steady states or equilibria.

3. **[[Stability Analysis]]**: By [[Linear Stability Analysis|linearizing]] the system near the fixed points and examining the [[eigenvalues]] of the [[Jacobian matrix]], one can determine the stability of these points. 
   - **Stable**: If all eigenvalues have negative real parts.
   - **Unstable**: If any eigenvalue has a positive real part.
   - **Saddle Point**: If eigenvalues have opposite signs.

4. **Vector Field**: A plot of the direction field (vectors) showing the direction of the system's trajectory at each point in the phase plane, which helps in visualizing the flow of the system.

5. **Trajectories and Orbits**: Solutions to the differential equations can be plotted in the phase plane as trajectories showing how the state of the system evolves over time from different initial conditions.

6. **Limit Cycles**: Closed trajectories representing periodic solutions. Stability of limit cycles can also be analyzed to determine if they are attracting or repelling.

### Example: Phase Plane of the FitzHugh-Nagumo Model

To apply phase plane analysis to the FitzHugh-Nagumo model, recall the system:

$$\frac{dv}{dt} = c(v - \frac{v^3}{3} - w + I), \quad \frac{dw}{dt} = \frac{v + a - bw}{\tau}$$

1. **Nullclines**:
   - \( v \)-nullcline: \( v - \frac{v^3}{3} - w + I = 0 \)
   - \( w \)-nullcline: \( v + a - bw = 0 \)

2. **Fixed Points**: Solve \( v - \frac{v^3}{3} - w + I = 0 \) and \( v + a - bw = 0 \) simultaneously to find the fixed points.

3. **Stability**: Analyze the Jacobian matrix evaluated at each fixed point to determine their stability.

4. **Vector Field and Trajectories**: Plotting these elements can reveal behaviors like excitable dynamics, where a small perturbation leads to a large excursion in the phase space before returning to rest, and potential oscillatory behaviors depending on parameter values.

### Conclusion

Phase plane analysis is invaluable for understanding the qualitative behavior of dynamical systems without solving the differential equations analytically. It is particularly useful in fields such as neuroscience, ecology, economics, and any area where non-linear systems are studied. For deeper insights, computational tools or symbolic computation can be employed to perform and visualize this analysis.