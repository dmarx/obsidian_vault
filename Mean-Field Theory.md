---
tags:
  - green
  - needs-outlinks
---
Mean-Field Theory (MFT) is a fundamental approach in statistical physics for modeling and understanding the behavior of [[many-body systems]] by averaging the effects of all interactions on a particular particle or spin to a single average or "mean field." This simplification reduces the complexity of dealing with interactions in a many-body system to a problem that involves only the interaction of individual particles with an effective field representing the average effect of their neighbors. MFT is widely used in various contexts, including magnetism, superconductivity, and phase transitions, providing insights into critical phenomena and the collective behavior of systems.

### Basic Principles

1. **[[Effective Interaction]]**: In MFT, the complex interactions between many particles are approximated by a single averaged effect, reducing the many-body problem to an effective one-body problem. For example, in a magnetic system, each spin interacts with an effective field produced by the average magnetization of all other spins.

2. **[[Self-Consistency Requirement]]**: The mean field is not known a priori and must be determined self-consistently. This is typically done by assuming a form for the order parameter (e.g., magnetization in a ferromagnetic material), calculating the mean field it produces, and then solving the equations to find the order parameter that is consistent with this mean field.

### Mathematical Formulation

Consider a simple model of a ferromagnet described by the Ising model, where spins \(s_i = \pm 1\) are placed on a lattice and interact with their nearest neighbors with an interaction strength \(J\). In the presence of an external magnetic field \(H\), the [[Hamiltonian]] can be written as:

$$ H = -J \sum_{\langle i, j \rangle} s_i s_j - H \sum_i s_i $$

where the first sum is over nearest-neighbor pairs. In MFT, the effect of all the neighboring spins on a given spin is approximated by an effective field \(H_{\text{eff}}\), leading to the mean-field Hamiltonian:

$$ H_{\text{MF}} = -H_{\text{eff}} \sum_i s_i $$

where \(H_{\text{eff}} = Jz\langle s \rangle + H\), \(J\) is the interaction strength, \(z\) is the coordination number (the number of nearest neighbors), and \(\langle s \rangle\) is the average spin, serving as the order parameter for magnetization.

### Applications and Predictions

- **[[Critical Temperature]]**: MFT predicts a critical temperature \(T_c\) above which the [[order parameter]] (e.g., magnetization) vanishes, indicating a [[phase transition]] from an ordered to a disordered phase. For the Ising model, \(T_c = Jz/k_B\), where \(k_B\) is the [[Boltzmann constant]].
  
- **[[Phase Diagrams]]**: MFT can be used to construct phase diagrams, indicating the conditions (temperature, external fields) under which different phases of the system are stable.
  
- **[[Critical Exponents]]**: MFT predicts specific values for the critical exponents that characterize the behavior of physical quantities near the phase transition. For example, it predicts \(\beta = 1/2\) for the order parameter, \(\gamma = 1\) for the susceptibility, and \(\alpha = 0\) for the specific heat (with a logarithmic divergence).

### Limitations

While MFT provides a useful first approximation for understanding phase transitions and collective phenomena, it neglects fluctuations, which become crucial near the critical point. As a result, MFT often overestimates the critical temperature and does not accurately capture the critical behavior of systems, especially in lower dimensions where fluctuations are more significant. The theory's predictions for critical exponents are accurate only above the [[upper critical dimension]] (\(d_c\)); for example, \(d_c = 4\) for the Ising model.

### Conclusion

Mean-Field Theory stands as a cornerstone of theoretical physics, offering significant insights into the collective behavior of many-body systems and the nature of phase transitions. Despite its simplifications, MFT has laid the groundwork for more sophisticated approaches, including the Renormalization Group theory, which better account for the role of [[Fluctuation Theory|fluctuations]] and provide a deeper understanding of critical phenomena.

> is there a relationship between mean-field theory and variational inference?

Yes, there is a conceptual relationship between Mean-Field Theory (MFT) in statistical physics and Variational Inference (VI) in the field of machine learning and statistics. Both approaches involve approximations that simplify complex systems by breaking them down into more manageable, non-interacting parts or by assuming independence among components of the system. While originating from different disciplines and serving different primary purposes, the underlying strategies of MFT and VI share a common goal of making intractable problems tractable through simplification and optimization.

### Mean-Field Theory (MFT)

MFT simplifies the analysis of many-body systems with interactions by replacing the complex interactions among all particles with an average or "mean field" that each particle experiences. This approach reduces the problem to one of analyzing a single particle (or a few particles) in an effective field, significantly simplifying the mathematics involved in describing the system's behavior, especially near phase transitions.

- **Application in Physics**: MFT is widely used to study phase transitions and critical phenomena, providing insights into the macroscopic behavior of systems based on their microscopic interactions.

### [[Variational Inference]] (VI)

VI is a technique in Bayesian inference used to approximate complex posterior distributions with simpler ones, making the problem of calculating or sampling from the posterior tractable. The approach involves selecting a family of distributions and finding the member of this family that is closest to the true posterior distribution, according to some divergence measure (often the Kullback-Leibler divergence).

- **Application in Statistics and Machine Learning**: VI is used to approximate posterior distributions in Bayesian models, enabling the practical application of these models to large datasets and complex problems.

### Relationship between MFT and VI

- **Approximation of Complex Interactions**: Both MFT and VI deal with complex systems by simplifying interactions within the system. MFT approximates interactions in many-body systems with an average field, while VI approximates complex posterior distributions with simpler, factorizable distributions.
- **Optimization**: Both approaches involve an optimization process—MFT through the minimization of the free energy subject to the mean field approximation, and VI through the minimization of the divergence between the approximate and true posterior distributions.
- **Factorization/Independence Assumptions**: A key aspect of VI is the assumption that the variables in the approximating distribution can be factorized (assumed independent), which is conceptually similar to treating particles as non-interacting in MFT.
- **[[Variational Principle]]**: Both MFT and VI can be viewed through the lens of the variational principle, where an optimal approximation is sought within a constrained set of possible solutions. In MFT, this often involves finding the configuration that minimizes the system's free energy, while in VI, it involves finding a distribution that minimizes the divergence from the posterior.

### Conclusion

While MFT and VI originate from and are primarily applied in different fields, the conceptual overlap in their approaches to simplifying complex systems underscores a broader theme in science: the utility of approximation and optimization methods in making intractable problems accessible. The relationship between these two methodologies highlights the interdisciplinary bridges that can enrich understanding and foster novel solutions across fields.