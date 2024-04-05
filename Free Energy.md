see also:
- [[Landau Free Energy]]

The concept of free energy in [[thermodynamics]] and [[statistical mechanics]] is a pivotal one, encompassing various forms depending on the context, such as [[Helmholtz Free Energy]], [[Gibbs Free Energy]], and others. It is a measure of the [[work]] obtainable from a system when the temperature and volume (in the case of Helmholtz free energy) or the temperature and pressure (in the case of Gibbs free energy) are maintained constant. Free energy is particularly important in the context of chemical reactions and phase transitions, where it helps to determine the direction and extent of chemical processes.

### Helmholtz Free Energy

Helmholtz free energy ($F$) is defined as the energy available to perform work at constant temperature and volume, and it's mathematically given by:

$$F = U - TS$$

where:
- $U$ is the internal energy of the system,
- $T$ is the absolute temperature,
- $S$ is the entropy of the system.

The decrease in Helmholtz free energy ($\Delta F$) corresponds to the maximum work that can be extracted from a closed system at constant volume and temperature, excluding the pV-work (expansion work).

### Gibbs Free Energy

Gibbs free energy ($G$), on the other hand, is used to describe the maximum reversible work that a thermodynamic system can perform at constant temperature and pressure. It is defined as:

$$G = H - TS$$

or alternatively,

$$G = U + PV - TS$$

where:
- $H = U + PV$ is the enthalpy of the system,
- $P$ is the pressure,
- $V$ is the volume of the system.

A negative change in Gibbs free energy ($\Delta G < 0$) during a process at constant temperature and pressure indicates that the process can occur spontaneously.

### Statistical Mechanics Perspective

From the perspective of statistical mechanics, free energy relates to the partition function of a system. The [[partition function]] ($Z$) is a sum over all possible states of a system, weighted by their Boltzmann factor, $e^{-\beta E}$, where $\beta = \frac{1}{k_B T}$, $k_B$ is the Boltzmann constant, and $E$ is the [[energy]] of a state.

- For the Helmholtz free energy, $F$ can be expressed in terms of the partition function as:

$$F = -k_B T \ln(Z)$$

- Similarly, for the Gibbs free energy in the [[grand canonical ensemble]], where the particle number is variable:

$$G = -k_B T \ln(\Xi)$$

where $\Xi$ is the grand partition function, a sum over states of varying particle numbers, each state weighted by its chemical potential, volume, and temperature.

### Applications and Importance

Free energy concepts are crucial in various scientific and engineering disciplines. They allow for the determination of the [[stability]] of phases, the direction of chemical reactions, the efficiency of engines, and the behavior of systems in equilibrium and non-equilibrium thermodynamics. For example, in biochemistry, the Gibbs free energy change of biochemical reactions is fundamental to understanding cellular processes such as metabolism and energy transfer.

In [[statistical mechanics]], these concepts are also used to derive relations among macroscopic quantities by considering the microscopic details of the systems, offering a bridge between the microstates and the macroscopic observables of thermodynamic systems.