see also:
- [[Boltzmann Distribution]]
- [[Partition Function]]
- [[Ideal Gas Law]]

The Maxwell-Boltzmann distribution is a fundamental concept in [[statistical mechanics]], describing the distribution of speeds in particles of a gas in thermal equilibrium. This distribution is particularly applicable to classical gases, where the particles do not experience quantum effects and the energies involved are not relativistic.

### Mathematical Description

The Maxwell-Boltzmann distribution for the speed $v$ of particles in an ideal gas can be expressed as follows:

$$ f(v) = 4\pi \left(\frac{m}{2\pi k_B T}\right)^{3/2} v^2 \exp\left(-\frac{mv^2}{2k_B T}\right) $$

where:
- $f(v)$ is the probability density function for the speed $v$,
- $m$ is the mass of a gas particle,
- $k_B$ is the Boltzmann constant,
- $T$ is the absolute temperature of the gas,
- $v^2$ is the square of the speed of the particles.

This function gives the probability density that a particle chosen at random will have a speed near $v$. It is derived from considering the [[kinetic energy]] of particles in three dimensions and assumes that the directions of particle motion are [[isotropic]] (equally probable in all directions).

### Derivation

The derivation of the Maxwell-Boltzmann distribution can be approached by considering the kinetic theory of gases and the statistical properties of molecular speeds. Here’s a condensed outline:

1. **[[Kinetic Theory]] Basis:** Start with the assumption that gas particles are point-like and non-interacting, except during brief [[elastic collisions]].

2. **Energy Distribution:** Consider that the total energy is partitioned equally among all degrees of freedom ([[Equipartition Theorem]]). For a non-quantum mechanical, classical particle, the energy associated with each [[degree of freedom]] is $\frac{1}{2} k_B T$.

3. **[[Statistical Independence]]:** Each component of the particle velocity vector (i.e., $v_x$, $v_y$, and $v_z$) is assumed to be statistically independent and normally distributed due to the [[central limit theorem]], given the large number of random collisions.

4. **[[Probability Density Function]] for Speed:** The magnitude of the velocity vector (speed) is given by $v = \sqrt{v_x^2 + v_y^2 + v_z^2}$. The distribution of $v$ follows the Maxwell-Boltzmann speed distribution, derived from the squared sum of three normally distributed variables (a [[chi-squared distribution]] with three [[degrees of freedom]]).

### Applications

- **Gas Kinetics:** The Maxwell-Boltzmann distribution is fundamental in understanding properties like diffusion, effusion, and the rate of chemical reactions in gases.
- **Thermodynamic Properties:** It helps in calculating macroscopic properties of gases, such as pressure, temperature, and viscosity, from microscopic behavior.
- **Statistical Mechanics:** Serves as a cornerstone for more complex theories and models in statistical mechanics, like those needed for quantum gases or plasmas.

### Limitations

- **Non-ideal Conditions:** The Maxwell-Boltzmann distribution assumes ideal gas behavior and fails at high pressures and low temperatures where interactions between particles become significant.
- **Quantum Effects:** It does not apply to systems where quantum mechanical effects are non-negligible, such as in Bose-Einstein condensates or Fermi gases at low temperatures.

Understanding the Maxwell-Boltzmann distribution provides a crucial foundation for the study of statistical mechanics and thermodynamics, linking microscopic particle dynamics to macroscopic observable properties in classical gases. For further exploration, delving into modifications of this distribution for quantum systems, like the [[Fermi-Dirac distribution]] and [[Bose-Einstein distribution]], offers insight into the behavior of systems under quantum statistical regimes.