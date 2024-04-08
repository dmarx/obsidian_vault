---
tags:
  - sod/gold
---
see also:
- [[Singularities]]

The term "singular behavior" in the context of [[Critical Phenomena]] and phase transitions refers to the dramatic changes in physical properties that occur as a system approaches a critical point. At the critical point, certain thermodynamic quantities exhibit singularities, meaning they diverge (become infinite) or go to zero in a manner that cannot be described by standard analytic functions. This singular behavior is a hallmark of [[Second-Order Phase Transitions|continuous (second-order) phase transitions]] and is characterized by [[Power Laws]] governed by [[critical exponents]].

### Examples of Singular Behavior

1. **Divergence of the [[Correlation Length]] (\(\xi\))**: As the critical point is approached, the correlation length, which measures the spatial extent over which particles or spins are correlated, diverges:
   $$ \xi \sim |T - T_c|^{-\nu} $$
   Here, \(T_c\) is the critical temperature, and \(\nu\) is a critical exponent. The divergence of \(\xi\) signifies that fluctuations occur over all spatial scales, and the system becomes scale-invariant at the critical point.

2. **Divergence of the Susceptibility (\(\chi\))**: The [[Susceptibility]], a measure of how the system responds to an external field, also diverges near the [[Critical Points|critical point]]:
   $$ \chi \sim |T - T_c|^{-\gamma} $$
   For example, in a ferromagnetic system, the magnetic susceptibility diverges as it approaches the Curie temperature from above. The exponent \(\gamma\) describes this singular behavior.

3. **[[Specific Heat]] (\(C\))**: The specific heat, which measures the amount of heat required to change the system's temperature, can diverge or exhibit a [[Cusp-Like Behavior]] as the system approaches \(T_c\):
   $$ C \sim |T - T_c|^{-\alpha} $$
   The exponent \(\alpha\) characterizes the singularity in the specific heat. In some systems, \(\alpha\) can be negative, indicating a less pronounced, but still singular, cusp-like behavior rather than a divergence.

4. **[[Order Parameter]] (\(M\))**: The order parameter, which measures the degree of order across the transition (e.g., magnetization in a magnet), vanishes as the critical point is approached from below according to:
   $$ M \sim (T_c - T)^{\beta} $$
   The disappearance of the order parameter in a continuous manner as \(T\) approaches \(T_c\) from below is another example of singular behavior, described by the critical exponent \(\beta\).

### Theoretical Implications

- **[[Scale Invariance]]**: At the critical point, the system exhibits scale invariance, meaning that its behavior looks the same at all length scales. This is directly related to the divergence of the correlation length, which implies that fluctuations of all sizes contribute to the system's properties.
  
- **[[Fluctuation Theory|Fluctuations]]**: The singular behavior near critical points is driven by the enhanced fluctuations that occur across the entire system. These fluctuations are not merely local but are correlated over long distances due to the diverging correlation length.

- **[[Renormalization Group Theory]]**: RG theory provides a powerful framework for understanding singular behavior near critical points. It explains how the coarse-graining and rescaling of a system reveal self-similar structures at different scales and lead to the universality of critical phenomena. The RG approach helps calculate critical exponents and predict the [[scaling laws]] that describe the singular behavior of thermodynamic quantities.

The singular behavior near critical points challenges classical thermodynamics and statistical mechanics, requiring advanced mathematical tools and concepts to describe and understand. These phenomena underscore the complexity and richness of phase transitions, revealing deep insights into the [[collective behavior]] of many-body systems.