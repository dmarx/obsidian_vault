---
tags:
  - sod/gold
---
see also:
- [[Rank]]

> Central to Landau theory is the concept of an order parameter, a quantity that measures the degree of order across a phase transition. 

The order parameter is a fundamental concept in Landau theory and in the study of phase transitions and critical phenomena. It serves as a quantitative measure that distinguishes between different phases of a system, especially near critical points where phase transitions occur. The order parameter typically changes in a characteristic way as the system undergoes a transition from one phase to another, providing a clear signal of the transition and its nature. Let's explore this concept in more detail:

### Defining the Order Parameter

- **Nature and Examples**: The order parameter can be a scalar, vector, or even tensor quantity, depending on the system and the type of [[Phase Transitions|phase transition]]. For example, in a ferromagnetic phase transition, the order parameter is the net magnetization of the system, which goes from zero in the disordered phase (above the Curie temperature) to non-zero in the ordered phase (below the Curie temperature). In a superfluid transition, the order parameter might be the complex amplitude of the macroscopic wave function of the superfluid component.

- **Role in [[Symmetry Breaking]]**: The choice of the order parameter is closely related to the [[Symmetry]] that is broken during the phase transition. In the ferromagnetic example, the symmetry of rotational invariance is broken when the system chooses a specific direction of magnetization. The order parameter (net magnetization) reflects this broken symmetry.

### How the Order Parameter Changes

- **[[Continuity|Continuous]] (Second-Order) Transitions**: For continuous, or second-order, phase transitions, the order parameter changes smoothly and continuously from zero in the high-temperature (disordered) phase to a finite value as the system is cooled below the [[Critical Points|critical temperature]]. This gradual change is indicative of a continuous transition.

- **[[Discrete|Discontinuous]] (First-Order) Transitions**: For first-order phase transitions, the order parameter changes abruptly at the [[transition point]]. The system jumps from one value of the order parameter to another, reflecting a discontinuous change in the system's phase. This can be accompanied by [[latent heat]] and other phenomena not present in second-order transitions.

### Mathematical Description

In Landau theory, the [[free energy]] of a system near a phase transition is expanded as a [[power series]] in terms of the order parameter. The coefficients of this expansion depend on temperature and other relevant physical parameters. By minimizing the free energy with respect to the order parameter, one can determine the [[Equilibrium]] value of the order parameter as a function of temperature and thus describe the phase transition.

### Critical Phenomena and Universality

- **Critical Exponents**: Near a critical point, the behavior of the order parameter (as well as other physical quantities) follows power laws characterized by critical exponents. These exponents are universal within a universality class, meaning they depend only on certain features like the system's dimensionality and symmetry, not on the microscopic details.

- **Universality Classes**: Systems with different microscopic details but similar "macroscopic" features (like dimensionality and symmetry properties related to the order parameter) can exhibit the same critical behavior. This forms the basis for the concept of universality classes in phase transitions.

In summary, the order parameter is a central concept in the study of phase transitions, embodying the changes in symmetry and order that occur as a system transitions between different phases. Its behavior provides deep insights into the nature of phase transitions and the underlying principles governing critical phenomena.


> By minimizing the free energy with respect to the order parameter, one can determine the equilibrium value of the order parameter as a function of temperature and thus describe the phase transition.

see also:
- [[Activation Energy]]

The process of minimizing the free energy with respect to the order parameter to describe phase transitions is a central aspect of Landau's theory. This method provides a way to understand how the equilibrium state of a system changes as external conditions, like temperature, vary. Here's a simplified explanation of how this works and its implications for describing phase transitions:

### [[Landau Free Energy]]

In [[Landau Theory]], the free energy \( F \) of a system near a [[Phase Transitions|phase transition]] is expressed as a function of the order parameter \( \phi \) and temperature \( T \). For simplicity, consider a second-order phase transition where the free energy can be expanded in a [[Taylor Series]] around \( \phi = 0 \), leading to an expression like:

\[ F(\phi, T) = F_0 + a(T) \phi^2 + b \phi^4 + \ldots \]

- \( F_0 \) is the reference free energy, independent of the order parameter.
- \( a(T) \) and \( b \) are coefficients that depend on temperature and other system parameters. Typically, \( b > 0 \) to ensure the stability of the free energy.
- The quadratic and quartic terms in \( \phi \) represent the simplest non-trivial expansion that captures the essence of second-order transitions. Higher-order terms may be included if necessary for more complex transitions.

### Minimizing the Free Energy

To find the equilibrium value of the order parameter, you minimize \( F(\phi, T) \) with respect to \( \phi \), leading to conditions that \( \phi \) must satisfy. This involves taking the derivative of \( F \) with respect to \( \phi \) and setting it to zero:

\[ \frac{dF}{d\phi} = 2a(T) \phi + 4b \phi^3 = 0 \]

Solving this equation gives the values of \( \phi \) that minimize the free energy. The solutions depend critically on the sign and magnitude of \( a(T) \):

- **Above the Critical Temperature (\( T > T_c \))**: If \( a(T) > 0 \), the only solution is \( \phi = 0 \), corresponding to the disordered phase where the symmetry is intact.

- **Below the Critical Temperature (\( T < T_c \))**: If \( a(T) < 0 \), non-zero solutions for \( \phi \) become possible, corresponding to the ordered phase where the symmetry is broken. The non-zero solutions indicate that the system has chosen a particular "direction" in the space of possible states, breaking the original symmetry.

### Phase Transition

The temperature at which \( a(T) \) changes sign (typically from positive to negative as the system cools) is the critical temperature \( T_c \). At this point, the system undergoes a phase transition from a disordered state (\( \phi = 0 \)) to an ordered state (\( \phi \neq 0 \)).

### Critical Behavior and Universality

Near the critical temperature, the behavior of the order parameter can be used to define [[Critical Exponents]] that describe how quantities like the order parameter, specific heat, and susceptibility diverge or go to zero. These critical exponents are universal within universality classes defined by the dimensionality and symmetry properties of the system.

This minimization of free energy to find the equilibrium value of the order parameter beautifully illustrates how macroscopic phenomena, like phase transitions, emerge from microscopic interactions. It provides a powerful framework for understanding the complex behavior of many-body systems near critical points.