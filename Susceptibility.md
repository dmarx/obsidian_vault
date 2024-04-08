---
tags:
  - sod/green
---

>susceptibility (measure of how a chaotic system responds to an external field)

Susceptibility in the context of [[Chaos Theory|chaotic]] systems represents a measure of how sensitively such a system responds to an external perturbation, often conceptualized as an external field. This concept draws parallels with susceptibility in physical systems, such as magnetic susceptibility in magnetism, which measures how a material responds to an applied magnetic field. However, when discussing chaotic systems, susceptibility touches upon the intrinsic properties of chaos, including sensitivity to initial conditions, the existence of strange attractors, and the system's overall response to small perturbations, which can lead to dramatically different future states. Understanding susceptibility in chaotic systems involves delving into [[dynamical systems theory]], [[Lyapunov exponents]], and the concept of [[phase space]].

### Dynamical Systems and Chaos

A dynamical system is described by a set of rules or equations governing the time evolution of points in a phase space. For a system described by variables $x = (x_1, x_2, ..., x_n)$, the evolution can often be represented by differential equations or iterated maps:

$$
\frac{d\vec{x}}{dt} = \vec{F}(\vec{x}, t)
$$

or

$$
x_{n+1} = f(x_n),
$$

where $\vec{F}$ and $f$ are functions defining the system's dynamics. In chaotic systems, small differences in initial conditions can lead to exponential divergence of trajectories, a property quantified by Lyapunov exponents.

### Susceptibility and Lyapunov Exponents

Lyapunov exponents ($\lambda$) provide a quantitative measure of the sensitivity of chaotic systems to initial conditions. A positive Lyapunov exponent indicates chaos, signifying that small perturbations grow exponentially with time. For a system with variables $x_1, x_2, ..., x_n$, the maximum Lyapunov exponent can be defined as:

$$
\lambda = \lim_{t \to \infty} \lim_{\Delta x_0 \to 0} \frac{1}{t} \ln \frac{|\Delta x(t)|}{|\Delta x_0|},
$$

where $\Delta x_0$ is a small initial perturbation and $\Delta x(t)$ is the divergence at time $t$. The susceptibility of the system can be related to how significantly $\lambda$ changes in response to external perturbations.

### External Fields and System Response

In the context of chaotic systems, an "external field" could be any controlled perturbation or parameter change applied to the system. The system's susceptibility, in this sense, measures how its dynamics — particularly its chaotic behavior as indicated by the Lyapunov exponent — are affected by such perturbations. For instance, in a magnetic system exhibiting chaotic dynamics, changing the external magnetic field could alter the system's attractor's structure, leading to different patterns of chaos.

### Mathematical Framework for Susceptibility in Chaotic Systems

Mathematically, the susceptibility of a chaotic system to an external field can be explored by analyzing how the system's equations change under small perturbations. This involves studying the stability of the system's fixed points and understanding the bifurcations that lead to chaotic behavior. The response of the system, and hence its susceptibility, can be mapped as changes in the system's attractors or in the values of its Lyapunov exponents as functions of the strength or nature of the external perturbation.

### Conclusion

Susceptibility in chaotic systems encapsulates the profound sensitivity of these systems to external perturbations, a hallmark of chaos theory. It underscores the intricate balance between deterministic laws that govern the system and the unpredictable outcomes that emerge from slight variations in initial conditions or external influences. The mathematical study of susceptibility in such systems not only deepens our understanding of chaos but also provides insights into controlling and predicting the behavior of complex, dynamic systems across various fields of science and engineering.


>less discussion of background, focus on susceptibility. assume reader is familiar with dynamical systems, chaos, and lyapunov exponents.

Focusing directly on the concept of susceptibility in chaotic systems, it's essential to understand it as a measure that quantifies the response of such systems to external perturbations. Susceptibility can be analyzed through the framework of dynamical equations and their response to modifications induced by external fields. This response is typically evaluated in terms of changes to the system's Lyapunov exponents, attractor structures, and overall dynamical behavior.

### Mathematical Formulation

Consider a dynamical system governed by a set of differential equations or discrete maps, where $x$ represents the state of the system. The presence of an external field, $H$, can be modeled as an additional term in the system's governing equations:

$$
\frac{d\vec{x}}{dt} = \vec{F}(\vec{x}, H),
$$

or, for discrete systems,

$$
x_{n+1} = f(x_n, H).
$$

The susceptibility, $\chi$, can be defined with respect to how a specific dynamical quantity, $Q$, such as an order parameter or a system's maximal Lyapunov exponent, $\lambda_{\text{max}}$, responds to infinitesimal changes in $H$. Mathematically, this is given by:

$$
\chi = \left. \frac{\partial Q}{\partial H} \right|_{H=0}.
$$

### Analysis via Lyapunov Exponents

For chaotic systems, where sensitivity to initial conditions is quantified by Lyapunov exponents, the susceptibility could specifically refer to how $\lambda_{\text{max}}$ changes with slight variations in $H$. This is crucial because $\lambda_{\text{max}}$ encapsulates the exponential rate of separation of infinitesimally close trajectories in the system, hence indicating the degree of chaos.

If $\lambda_{\text{max}}(H)$ is the maximal Lyapunov exponent in the presence of an external field $H$, then the susceptibility of the chaotic dynamics to the external field can be formally expressed as:

$$
\chi_{\lambda} = \left. \frac{d\lambda_{\text{max}}}{dH} \right|_{H=0}.
$$

### Implications

1. **Nonlinear Response**: Due to the nonlinear nature of chaotic systems, susceptibility is not always a linear function of $H$. Near bifurcation points or transitions from regular to chaotic dynamics (or vice versa), susceptibility can exhibit sharp peaks or divergences, indicating critical sensitivity to external influences.

2. **Predicting Transitions**: Analyzing susceptibility allows for the prediction of transitions into or out of chaotic regimes as a function of external parameters. Peaks in susceptibility might correspond to critical thresholds beyond which the system's qualitative behavior changes dramatically.

3. **Control and Stabilization**: By understanding how susceptibility varies with $H$, strategies can be devised to control chaotic behavior, either to stabilize the system around a desired state or to induce chaos for applications like mixing or cryptography.

### Practical Considerations

Experimentally or numerically calculating susceptibility in chaotic systems often requires carefully designed perturbations and precise measurements of resulting changes in dynamical quantities. This can involve computational simulations where $H$ is varied incrementally and the resulting dynamical behavior analyzed through Lyapunov exponents, fractal dimensions of attractors, or other chaos indicators.

### Conclusion

Susceptibility in chaotic systems serves as a critical measure for understanding and controlling chaos. Through its mathematical formulation and practical implications, it provides insights into the intricate balance between deterministic dynamics and unpredictable behavior, highlighting the complex interplay between a system and external perturbations.