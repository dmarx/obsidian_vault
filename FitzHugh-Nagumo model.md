### Overview of the FitzHugh-Nagumo Model

The **FitzHugh-Nagumo model** is a simplified version of the [[Hodgkin-Huxley model]] that was formulated to describe the electrical activity of neurons through a pair of differential equations. It captures the essential qualitative features of neuron dynamics, such as excitability and spiking behavior, with fewer variables and simplified kinetics. The model was independently proposed by Richard FitzHugh (1961) and by J. Nagumo et al. (1962) as a two-dimensional simplification of the four-dimensional Hodgkin-Huxley model.

### Mathematical Formulation

The FitzHugh-Nagumo model consists of two differential equations that describe the dynamics of the membrane potential and a recovery variable. The model equations are given by:

1. **Voltage Equation**:
   $$\frac{\partial v}{\partial t} = c(v - \frac{v^3}{3} - w + I)$$

2. **Recovery Equation**:
   $$\frac{\partial w}{\partial t} = \frac{v + a - bw}{\tau}$$

Here, $v(t)$ represents the membrane potential, $w(t)$ is a recovery variable that models the effects of ion channels that are slow to activate and deactivate (akin to a refractory period), and $I$ represents a constant external current input. The parameters $a$, $b$, $c$, and $\tau$ are constants that need to be tuned based on experimental data or specific modeling needs.

### Dynamics and Features

- **Excitability**: Just like actual neurons, the FitzHugh-Nagumo model exhibits excitability. If the membrane potential $v$ is perturbed beyond a certain threshold, the system will emit a large excursion in phase space (a spike) before returning to its resting state.
- **[[Phase Plane Analysis]]**: The model's behavior can be analyzed using phase plane techniques, where $v$ and $w$ form a two-dimensional system. The nullclines (curves where the derivative of $v$ or $w$ with respect to time is zero) intersect at fixed points, whose stability determines the behavior of the system.
- **Bistability and Oscillations**: Depending on the parameter values, the model can show bistability (two stable steady states) and limit cycle oscillations (repetitive spiking).

### Parameter Impact

- **$a$ and $b$**: These parameters control the position and shape of the $w$ nullcline and thereby influence the stability and number of the fixed points.
- **$c$ and $\tau$**: These affect the time scales of the $v$ and $w$ dynamics, respectively. The ratio of these time scales can significantly affect the nature of the oscillations and the response speed of the system.

### Applications

- **Neuroscience**: It provides insights into the mechanisms of nerve impulse propagation and the role of various parameters in neuronal excitability.
- **Cardiac Dynamics**: Modifications of the model apply to understanding cardiac action potentials and arrhythmias.
- **Education and Research**: Due to its simplicity, the FitzHugh-Nagumo model is widely used in computational neuroscience education and in theoretical research for exploring the generic properties of excitable systems.

### Further Exploration

For more detailed explorations, looking into how the FitzHugh-Nagumo model is integrated into larger networks for simulating brain activity or how it's adapted for specific types of neuronal behavior would be of interest. Advanced studies might involve numerical simulations of the model under different conditions, or analytical studies focusing on bifurcation theory to understand how changes in parameters affect the system's dynamics.