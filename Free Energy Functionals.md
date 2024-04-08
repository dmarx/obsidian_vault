---
tags:
  - sod/gold
  - sod/green
  - empty-hub
---

see also:
- [[Functional Analysis]]

[[Free energy]] [[Functionals]] are fundamental concepts in the theoretical description of complex systems in physics, chemistry, and materials science. They play a pivotal role in understanding phase behavior, dynamics, and equilibrium properties of systems at the microscopic and macroscopic levels. A free energy functional is essentially a mathematical representation that expresses the free energy of a [[Systems|system]] as a function of one or more [[Order Parameter|order parameters]] that describe the state of the system. These functionals are crucial in the study of [[phase transitions]], [[Interface Phenomena]], and the [[thermodynamic stability]] of various phases.

### Types of Free Energy

There are primarily two types of free energy relevant to the discussion of free energy functionals:

1. **[[Helmholtz Free Energy]] ($F$)**: Relevant in contexts where the system is at constant volume and temperature. It is defined as $F = U - TS$, where $U$ is the internal energy, $T$ is the temperature, and $S$ is the entropy.

2. **[[Gibbs Free Energy]] ($G$)**: Used when the system is at constant pressure and temperature, defined as $G = H - TS$, with $H = U + PV$ being the enthalpy, $P$ the pressure, and $V$ the volume.

### Formalism of Free Energy Functionals

The formalism of free energy functionals involves expressing the free energy, $F$ or $G$, as a functional of the order parameter(s) $\psi$. The order parameter can represent various physical quantities depending on the context, such as magnetization in a ferromagnet, density in a fluid, or composition in a binary mixture. The general form of a free energy functional can be written as:

$$F[\psi(\mathbf{r})] = \int d\mathbf{r} \, f(\psi(\mathbf{r}), \nabla\psi(\mathbf{r}), \mathbf{r})$$

where $f$ is a local free energy density that depends on the order parameter $\psi(\mathbf{r})$, its gradient $\nabla\psi(\mathbf{r})$, and possibly the position $\mathbf{r}$. This expression captures both the local contributions to the free energy and the contributions from spatial inhomogeneities or interfaces.

### Applications and Examples

- **[[Phase Field Models]]**: These models use free energy functionals to describe the evolution of microstructures in materials, such as the growth of grains in a polycrystal or the dynamics of [[phase separation]]. The free energy functional typically includes terms that account for bulk [[phase stability]] and [[interfacial energy]].

- **Landau Theory of Phase Transitions**: In the [[Landau theory]], the free energy is expanded in powers of the order parameter near a phase transition point. This approach can describe second-order phase transitions by analyzing the stability and changes in the minima of the free energy functional.

- **[[Ginzburg-Landau Theory]] for Superconductors**: This theory extends the Landau theory to include spatial variations of the order parameter, describing the behavior of superconductors near the superconducting transition. The Ginzburg-Landau free energy functional is instrumental in predicting properties like the penetration depth and coherence length of superconductors.

- **[[Density Functional Theory]] (DFT)**: In the context of quantum mechanics and materials science, DFT expresses the total energy of a quantum system as a functional of the electron density. Although not a free energy functional in the thermodynamic sense, it shares the conceptual framework of using functionals to determine system properties.

### Importance and Challenges

The use of free energy functionals is crucial for predicting the equilibrium properties of systems without resorting to the detailed simulation of every particle or quantum state. They provide a bridge between microscopic interactions and macroscopic observables. However, constructing accurate free energy functionals for complex systems remains a significant challenge, often requiring sophisticated approximations and empirical input. Despite these challenges, free energy functionals continue to be a powerful tool in theoretical and computational physics, enabling the study of a wide range of phenomena from phase transitions to the behavior of complex fluids and beyond.