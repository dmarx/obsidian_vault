see also:
- [[Maxwell-Boltzmann Distribution]]
- [[Boltzmann Distribution]]
- [[Partition Function]]
- [[Statistical Mechanics]]

The equipartition theorem is a fundamental principle in classical [[statistical mechanics]] that states that energy is equally distributed among all available [[degrees of freedom]] in a system at [[thermal equilibrium]]. According to this theorem, each degree of freedom contributes an average energy of $\frac{1}{2} k_B T$ to the system's total energy, where $k_B$ is the [Boltzmann constant] and $T$ is the temperature in Kelvin.

### Definition of a Degree of Freedom

A degree of freedom in this context refers to an independent way in which a system can store energy. In classical mechanics, these are typically associated with the motion of particles:
- **Translational [[degrees of freedom]]** relate to the motion along the x, y, and z axes.
- **Rotational degrees of freedom** relate to rotation about these axes (for non-point-like particles or molecules).
- **Vibrational degrees of freedom** involve the potential and kinetic energy stored in the structure of molecules as they oscillate about equilibrium positions (more relevant for molecules than for monatomic gases).

### Application to Gases

For a monatomic ideal gas, where particles are approximated as point masses, the particles possess only translational degrees of freedom. Since the particles can move in three dimensions, each particle has three translational degrees of freedom. According to the equipartition theorem:

- Each translational degree of freedom contributes $\frac{1}{2} k_B T$ to the total kinetic energy.
- Therefore, the total average kinetic energy per particle in a monatomic gas is $\frac{3}{2} k_B T$.

### Mathematical Formulation

The kinetic energy for a particle of mass $m$ moving with velocity $v$ is given by:
$$ E = \frac{1}{2} m v^2 $$

If we consider an ensemble of such particles in a gas, the average kinetic energy per particle, according to the equipartition theorem, is:
$$ \langle E \rangle = \frac{3}{2} k_B T $$

This aligns with the Maxwell-Boltzmann distribution, where the average kinetic energy derived from the distribution of particle speeds must also equal $\frac{3}{2} k_B T$.

### Derivation of Maxwell-Boltzmann Distribution

In deriving the Maxwell-Boltzmann distribution using the equipartition theorem:
1. **Velocity Components as Normal Distributions:** The components of velocity ($v_x$, $v_y$, $v_z$) are each associated with a kinetic energy of $\frac{1}{2} m v_x^2$, $\frac{1}{2} m v_y^2$, and $\frac{1}{2} m v_z^2$. Each component contributes $\frac{1}{2} k_B T$ to the average kinetic energy, and their distributions are normal (Gaussian) due to the central limit theorem.

2. **Total Speed Distribution:** To find the distribution of the speed (magnitude of velocity vector), one combines these normal distributions of the velocity components. The result is the Maxwell-Boltzmann speed distribution, which accounts for the kinetic energy being distributed equally among the three translational degrees of freedom.

### Significance and Limitations

The equipartition theorem provides a powerful tool for predicting the energy distribution in classical systems. However, it has limitations when applied to systems where quantum effects are significant (such as at very low temperatures) or where interactions between particles significantly affect the system's behavior (such as in non-ideal gases). In such cases, modifications to classical statistical mechanics are necessary, and different statistical distributions (like Fermi-Dirac or Bose-Einstein) are used to describe the system's properties more accurately.