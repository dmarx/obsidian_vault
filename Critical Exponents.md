---
tags:
  - sod/root
---

> Near the critical temperature, the behavior of the order parameter can be used to define critical exponents that describe how quantities like the order parameter, specific heat, and susceptibility diverge or go to zero. These critical exponents are universal within universality classes defined by the dimensionality and symmetry properties of the system.

[[Criticality|Critical]] exponents play a key role in the study of phase transitions and [[Critical Phenomena]], providing a universal description of how physical quantities behave as a system approaches its critical point. These exponents are determined by the behavior of the order parameter, specific heat, susceptibility, and correlation length near the critical temperature (\(T_c\)). Despite the diversity of physical systems and the details of their microscopic interactions, systems within the same universality class share the same set of critical exponents. This universality is a powerful concept, allowing for the prediction of behavior across different systems based on their symmetry properties and dimensionality. Let's delve into some of these critical exponents and what they describe:

### Critical Exponents

- **[[Order Parameter]] Exponent (\(\beta\))**: This exponent describes how the order parameter (\(\phi\)) behaves as the temperature approaches \(T_c\) from below. Mathematically, \(\phi \sim (T_c - T)^\beta\) for \(T < T_c\). It characterizes the onset of order as the system cools down through the critical temperature.

- **[[Susceptibility]] Exponent (\(\gamma\))**: Susceptibility (\(\chi\)) measures the response of the order parameter to a field conjugate to it (like magnetic field for magnetization). Near \(T_c\), \(\chi \sim |T_c - T|^{-\gamma}\), indicating how the system's response diverges as it approaches the critical point.

- **[[Specific Heat]] Exponent (\(\alpha\))**: The specific heat (\(C\)) shows how the energy stored in the system changes with temperature. Near \(T_c\), \(C \sim |T_c - T|^{-\alpha}\). This exponent describes the divergence (or cusp) in specific heat at the critical point.

- **[[Correlation Length]] Exponent (\(\nu\))**: The correlation length (\(\xi\)) measures the size of regions over which parts of the system are correlated with each other. As \(T\) approaches \(T_c\), \(\xi \sim |T_c - T|^{-\nu}\), reflecting how fluctuations at the critical point occur over all scales, leading to scale invariance.

- **[[Correlation Function]] Exponent (\(\eta\))**: The correlation function describes how correlations between parts of the system decay with distance at \(T_c\). At the critical point, the decay is slower than exponential, often following a power law \(r^{-d+2-\eta}\), where \(r\) is the distance and \(d\) is the dimensionality of the system.

### [[Universality]]

The concept of universality asserts that these critical exponents depend only on a few key features:
- **[[Dimensionality]] of the System**: The number of spatial dimensions significantly influences the values of the critical exponents.
- **[[Symmetry]] of the Order Parameter**: The type of symmetry breaking that occurs at the phase transition affects which universality class the system belongs to.
- **Range of Interactions**: The nature (short-range vs. long-range) of interactions in the system can also determine its universality class.

### Implications

The universality of critical exponents means that very different systems can exhibit the same critical behavior if they share the same dimensionality, symmetry properties of the order parameter, and range of interactions. This has profound implications for theoretical and experimental physics, as it allows for the classification of phase transitions beyond the specifics of material composition or microscopic details, focusing instead on more fundamental, shared properties.


> tell me more about the correlation exponents nu and eta and their relationship with range of interactions in a system that exhibits critical phenomena

The critical exponents $\nu$ and $\eta$ describe how the correlation length and correlation function behave near the critical point of a phase transition, respectively. Their values, and the relationship between them and the range of interactions in a system exhibiting critical phenomena, offer deep insights into the nature of those phenomena and the universality classes to which the system belongs.

### Correlation Length Exponent ($\nu$)

The correlation length $\xi$ measures the size over which fluctuations in the system are correlated. Near the critical temperature $T_c$, the correlation length diverges, following the relationship:

$$\xi \sim |T_c - T|^{-\nu}$$

This means that as the system approaches the critical point, fluctuations occur over increasingly larger scales, and at the critical point itself, these correlations span the entire system, leading to scale invariance. The exponent $\nu$ characterizes how quickly the correlation length diverges as the critical point is approached.

### Correlation Function Exponent ($\eta$)

The correlation function describes how the correlation between parts of the system decays with distance. At the critical point, where the correlation length is infinite, the correlation function $G(r)$ between two points separated by distance $r$ typically follows a [[Power-Law Distributions|power-law]] decay:

$$G(r) \sim \frac{1}{r^{d-2+\eta}}$$

Here, $d$ is the dimensionality of the system, and $\eta$ modifies the decay rate, reflecting how the effective dimensionality of interactions changes due to critical fluctuations. The exponent $\eta$ is generally small but positive, indicating that correlations decay more slowly at the critical point than they would in a non-critical system.

### Relationship with Range of Interactions

The range of interactions in a system significantly affects the values of $\nu$ and $\eta$ and, consequently, the critical behavior of the system. Here's how:

- **Short-Range Interactions**: For systems with short-range interactions, the universality class (and thus the values of $\nu$ and $\eta$) is primarily determined by the dimensionality of the system and the symmetry of the order parameter. The critical behavior is well-described by models like the Ising model for magnetic systems.

- **Long-Range Interactions**: When interactions are long-range (decaying with distance $r$ as $r^{-\alpha}$ where $\alpha < d$), the critical behavior can be significantly different. The values of $\nu$ and $\eta$, and thus the nature of the phase transition, can change. For sufficiently long-range interactions, they can depend explicitly on the decay rate of the interactions. For example, systems with long-range interactions may exhibit mean-field behavior even in lower dimensions, where short-range interactions would not.

- **[[Crossover Phenomena]]**: In systems where both short-range and long-range interactions are present, crossover phenomena can occur. The critical behavior may start resembling one universality class (e.g., short-range) far from the critical point but switch to another (e.g., long-range) closer to the critical point. The values of $\nu$ and $\eta$ can reflect this crossover in their dependence on the temperature and interaction parameters.

The relationship between $\nu$, $\eta$, and the range of interactions underscores the importance of universality in critical phenomena. It illustrates how systems with vastly different microscopic details can exhibit similar critical behavior when viewed through the lens of these fundamental exponents.

---

Critical exponents are fundamental in characterizing the singular behavior of physical quantities near phase transitions. These exponents provide a quantitative description of how certain properties of a system diverge or go to zero as the system approaches a critical point, such as the critical temperature for a phase transition. Critical exponents are universal in the sense that they depend only on the dimensionality of the system and the symmetry of the order parameter, not on the microscopic details of the system. This universality allows different systems that share the same critical exponents to be classified into the same universality class.

### Common Critical Exponents

Here are some of the most commonly studied critical exponents, which describe the behavior near a critical point:

- **Exponent \(\alpha\)**: Describes the divergence of the specific heat \(C\) as \(C \sim |T - T_c|^{-\alpha}\), where \(T\) is the temperature and \(T_c\) is the critical temperature.
  
- **Exponent \(\beta\)**: Characterizes the behavior of the [[order parameter]] \(M\) (e.g., magnetization in a ferromagnetic material) as \(M \sim (T_c - T)^\beta\) for \(T < T_c\).
  
- **Exponent \(\gamma\)**: Describes the [[divergence of the susceptibility]] \(\chi\) (e.g., magnetic susceptibility) as \(\chi \sim |T - T_c|^{-\gamma}\).
  
- **Exponent \(\nu\)**: Relates to the [[divergence of the correlation length]] \(\xi\), which measures the size over which fluctuations are correlated, as \(\xi \sim |T - T_c|^{-\nu}\).
  
- **Exponent \(\delta\)**: Describes how the order parameter responds to an external field \(h\) at the critical temperature as \(M \sim h^{1/\delta}\) when \(T = T_c\).

### Scaling Laws

Critical exponents are not independent but are related through several [[scaling laws]], which are themselves a consequence of the [[scale invariance]] at the [[critical point]]. Some of these scaling laws include:

- **[[Rushbrooke's equality]]**: \(\alpha + 2\beta + \gamma = 2\)
- **[[Widom's scaling law]]**: \(\gamma = \beta(\delta - 1)\)
- **[[Fisher's Scaling Law]]**: \(\gamma = \nu(2 - \eta)\), where \(\eta\) describes the decay of the correlation function at the critical point.

These relationships are derived from the assumption that near the critical point, the free energy and other thermodynamic functions can be expressed in terms of scaling functions, which depend on dimensionless combinations of the relevant physical variables.

### Calculation and RG Theory

The RG theory provides a powerful framework for calculating critical exponents. By examining the flow of a system's parameters (e.g., coupling constants) under scale transformations, RG theory identifies fixed points of this flow, which correspond to phase transitions. The stability of these fixed points and the behavior of the RG flow in their vicinity determine the values of the critical exponents.

### Significance

Critical exponents and the associated scaling laws are crucial for understanding the nature of phase transitions and critical phenomena. They offer insights into the universality of phase transitions, indicating that systems with very different microscopic physics can exhibit similar macroscopic behavior near their critical points. This universality has profound implications, allowing for the classification of phase transitions into universality classes and enabling the prediction of phase transition behavior in complex systems based on the study of simpler models.