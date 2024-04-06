---
tags:
  - gold
  - green
---

see also:
- [[Continuous Phase Transitions]] - redirect here if created

Second-order [[phase transitions]], also known as continuous phase transitions, are a category of phase transitions in which some derivatives of the [[free energy]] are discontinuous. These transitions are characterized by the absence of latent heat and a gradual change in order, making them fundamentally different from [[first-order phase transitions]], where the change is abrupt and often involves latent heat. The theory of second-order phase transitions and [[critical phenomena]] is a central topic in statistical physics, condensed matter physics, and materials science.

### Key Features

1. **Order Parameter:** The transition is marked by the continuous change of an order parameter from zero in one phase to a nonzero value in the other. The order parameter, which is often denoted by $\phi$, is a measure of the degree of order across the transition. In a magnetic system, for example, the magnetization serves as the order parameter.

2. **Critical Point:** The point at which the phase transition occurs is called the critical point. At this point, physical properties such as correlation length, susceptibility, and specific heat exhibit critical behavior, often diverging to infinity or dropping to zero.

3. **Symmetry Breaking:** Second-order transitions frequently involve a change in symmetry, where a higher symmetry state transitions to a lower symmetry state as the order parameter changes.

### Mathematical Description

The [[Landau theory]] of phase transitions provides a phenomenological framework to describe second-order phase transitions. In this theory, the free energy $F$ of a system near the critical point is expanded as a power series in the order parameter $\phi$:

$$F(\phi, T) = F_0(T) + a(T)\phi^2 + b(T)\phi^4 + \cdots,$$

where $T$ is the temperature, $F_0(T)$ is the free energy at $\phi=0$, and $a(T)$, $b(T)$ are temperature-dependent coefficients. The term in $\phi^4$ is necessary to ensure the stability of the free energy. The coefficient $a(T)$ changes sign at the critical temperature $T_c$, leading to the onset of order (i.e., $\phi \neq 0$) below $T_c$.

### [[Critical Exponents]] and [[Scaling Laws]]

Second-order phase transitions are described by critical exponents that characterize the behavior of physical quantities near the critical point. These exponents are universal in the sense that they depend only on the [[dimensionality]] of the [[Systems|system]] and the [[symmetry]] of the [[order parameter]], not on the microscopic details. Important critical exponents include:

- $\alpha$: Governs the divergence of the [[specific heat]], $C \sim |T-T_c|^{-\alpha}$.
- $\beta$: Describes the onset of the [[order parameter]], $\phi \sim |T-T_c|^\beta$ for $T < T_c$.
- $\gamma$: Describes the divergence of the [[susceptibility]], $\chi \sim |T-T_c|^{-\gamma}$.
- $\nu$: Governs the divergence of the [[correlation length]], $\xi \sim |T-T_c|^{-\nu}$.

### [[Renormalization Group Theory]]

The renormalization group (RG) theory provides a powerful framework for understanding the [[universality]] and scaling behavior near second-order phase transitions. RG theory involves iteratively "zooming out" of the system to observe how the system's parameters transform under changes in scale. This approach explains why microscopic details become irrelevant near critical points and provides a method for calculating critical exponents.

### Applications

Second-order phase transitions are observed in a wide range of physical systems, including:

- Magnetic systems, where the transition involves the onset of magnetization.
- Superfluid transitions, such as the transition of helium-4 at low temperatures.
- The superconducting transition, where electrical resistance drops to zero.
- [[Critical opalescence]] in fluids near the critical point of the liquid-gas transition.

Understanding second-order phase transitions is crucial for the development of materials with novel properties and the exploration of fundamental principles in physics.