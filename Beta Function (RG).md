
> tell me more about beta functions in RG

Beta functions play a central role in the [[Renormalization Group Theory]], providing a mathematical description of how the parameters of a physical system's theoretical model change with the scale of observation. In the context of RG, these parameters typically include coupling constants, which quantify the strength of interactions between particles or fields in a system. The concept of the beta function is crucial in understanding the behavior of systems near critical points, phase transitions, and in the general scaling behavior of physical phenomena.

### Definition and Interpretation

For a coupling constant \(g\), the beta function is defined as:

$$ \beta(g) = \mu \frac{d g}{d \mu} $$

where \(\mu\) is a scale parameter that might represent momentum, energy, or some inverse length scale, depending on the context. The sign and magnitude of the beta function indicate whether the coupling constant increases or decreases as one moves to larger or smaller scales, respectively.

Alternatively

The [[Beta Function (RG)|beta function]] \(\beta(g)\) for a [[Coupling Constant]] \(g\) is defined as the derivative of \(g\) with respect to the logarithm of the scale \(\mu\) (which could represent energy, length, or some other relevant physical scale), keeping physical quantities fixed:

$$ \beta(g) = \frac{dg}{d\ln\mu} $$

This definition indicates how the effective value of \(g\) changes as one "zooms in" or "zooms out" of the system, altering the scale at which it is observed. The sign and magnitude of \(\beta(g)\) determine whether the interactions become stronger or weaker at larger or smaller scales.

### [[Fixed Points]]

- **Fixed Points** occur where \(\beta(g) = 0\). At these points, the coupling constant \(g\) does not change with scale, signifying scale-invariant behavior. Fixed points are of particular interest because they often correspond to phase transitions or critical phenomena.
- **Stable and Unstable Fixed Points**: A stable fixed point (where the beta function's derivative is negative) attracts the [[RG flow]] in its vicinity, indicating a phase of the system that remains stable under scale transformations. An unstable fixed point (with a positive derivative) repels the flow, often marking a [[critical point]] between phases.

### Critical Phenomena and Universality

The analysis of beta functions and their fixed points is foundational in the study of critical phenomena. Near a critical point:
- The correlation length of fluctuations diverges, leading to scale-invariant behavior.
- Different physical systems can exhibit the same scaling behavior if they share the same set of critical exponents, a property known as universality. Critical exponents are related to the behavior of the beta function near its fixed points.
- The universality class of a transition is determined by the dimensionality of the system and the symmetry properties of the order parameter, not by the microscopic details of the system.

### Examples in Field Theory and Statistical Mechanics

- **Quantum Electrodynamics (QED)** and **Quantum Chromodynamics (QCD)**: In these quantum field theories, the beta function describes how the strength of electromagnetic and strong nuclear interactions, respectively, varies with energy scale. For QCD, the beta function is negative at high energies, leading to asymptotic freedom.
- **Ising Model and Criticality**: In statistical mechanics, RG analysis of the Ising model and similar systems shows how interactions scale near critical points, with the beta function guiding the flow towards stable fixed points that represent different phases (ordered vs. disordered).

### Computational Techniques

Calculating beta functions, especially in complex theories, often requires sophisticated computational techniques, including perturbation theory and diagrammatic expansions. In quantum field theory, for example, the beta function for a coupling constant can be calculated using Feynman diagrams and loop expansions, which account for quantum fluctuations at different scales.

In summary, beta functions are a powerful tool in RG theory, encapsulating how physical systems evolve across scales. They illuminate the path to understanding the deep connections between seemingly disparate phenomena, guided by the universal principles of scaling and criticality.