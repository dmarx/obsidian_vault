---
tags:
  - sod/green
  - sod/root
---

See Also:
- [[Group Theory]]
- [[Discrete Symmetry Groups]]
- [[Lie Groups]]
- [[Symmetry Breaking]]
- [[Conservation Laws]]
- [[Noether's Theorem]]
- [[Dimensional Analysis]]
- [Kunin et al - Neural Mechanics: Symmetry and Broken Conservation Laws in Deep Learning Dynamics](https://arxiv.org/abs/2012.04728)

> The types of symmetry that a system exhibits can dictate the kinds of phase transitions it can undergo and thus its universality class.

The relationship between the types of symmetry a system exhibits and the kinds of phase transitions it can undergo is a fundamental aspect of understanding universality classes in [[Critical Phenomena]]. Symmetry and symmetry breaking play a pivotal role in determining the nature of [[Phase Transitions]] and categorizing systems into [[Universality Classes]]. Let's delve into why symmetry is so crucial:

### Symmetry in Phase Transitions

- **Symmetry Before and After the Transition**: At a critical point, a system may undergo a phase transition, leading to a change in symmetry. For example, in a ferromagnetic phase transition, above the critical temperature ([[Curie point]]), the system is disordered and exhibits rotational symmetry because the orientation of spins is random. Below this temperature, the system orders magnetically, breaking this symmetry because the spins align in a specific direction.

- **[[Order Parameter]]**: The concept of an order parameter is often used to describe phase transitions. It measures the degree of order across the transition. The symmetry of the order parameter can dictate the type of phase transition. For instance, in the ferromagnetic transition, the magnetization acts as an order parameter that goes from zero (in the high-symmetry, disordered phase) to nonzero (in the low-symmetry, ordered phase).

### Symmetry and Universality Classes

- **[[Landau Theory]] of Phase Transitions**: [[Lev Landau]] developed a theory that categorizes phase transitions based on the symmetry properties of the order parameter and the system. According to Landau's theory, systems with similar [[symmetry breaking patterns]] and [[dimensions]] belong to the same universality class, meaning they have the same [[Critical Exponents]] and [[scaling laws]] near the transition.

- **[[Renormalization Group Theory]]**: This approach goes further by considering how fluctuations at different scales can affect phase transitions, particularly near [[Critical Points]]. It shows that the critical behavior of a system (and thus its universality class) depends on a few key features, including the system's [[Dimensionality]] and the symmetries of the order parameter. 

### Examples of Symmetry Influencing Universality Classes

- **[[Ising Model]] vs. [[XY Model]]**: The Ising model, which is a model of ferromagnetism, involves spins that can be either up or down ([[Z2 symmetry]]). The XY model involves spins in a plane, with continuous rotational symmetry ([[U(1) symmetry]]). Although these models describe different physical systems, the nature of their symmetry ([[discrete]] vs. [[Continuity|continuous]]) crucially affects the kinds of phase transitions they exhibit and which universality class they belong to.

- **Liquid-Gas Critical Point**: In a liquid-gas system, the symmetry involves the interchangeability of the liquid and gas phases at the critical point, where they become indistinguishable. This symmetry dictates the universality class of the liquid-gas critical point, which is characterized by specific critical exponents.

In summary, the type of symmetry a system exhibits not only dictates the kinds of phase transitions it can undergo but also categorizes the system into a universality class with other systems that share similar symmetry properties, even if their microscopic details differ. This powerful concept allows physicists to understand and predict the behavior of complex systems near critical points based on relatively simple principles.