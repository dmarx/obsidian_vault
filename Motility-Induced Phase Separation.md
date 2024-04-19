see also:
- [[Active Matter Systems]]

**Introduction**

Motility-induced phase separation (MIPS) is a phenomenon observed in systems of self-propelled particles, which, under certain conditions, can spontaneously separate into dense (solid or liquid-like) and dilute (gas-like) phases, even in the absence of attractive interactions between the particles. This counterintuitive behavior arises from purely non-equilibrium effects, driven by the particles' motility, and has been a subject of extensive study in the fields of [[active matter physics|active matter]] and [[statistical physics]].

**Mechanism of MIPS**

The underlying mechanism of MIPS can be understood by considering how the motility of particles and their interactions lead to a feedback loop between density and mobility. In systems exhibiting MIPS, the following steps typically occur:

1. **Local Density Increase**: When self-propelled particles move randomly, they occasionally encounter one another and temporarily slow down due to steric hindrance or alignment interactions.
   
2. **Reduced Mobility**: As more particles accumulate in a region, their ability to move freely is further hindered, reducing the overall mobility in that region.
   
3. **Feedback Loop**: This reduction in mobility causes particles to spend more time in the crowded area, further increasing the local density. This positive feedback between reduced mobility and increased density can lead to the growth of a dense phase.

4. **[[Phase Separation]]**: Once a critical density is reached, the system can spontaneously separate into regions of high density (where particles are largely immobile) and low density (where particles are free to move), much like the phase separation observed in equilibrium systems of particles with attractive interactions.

**Mathematical Formalism**

To model MIPS, we can consider a simplified system of active [[Brownian Motion|Brownian particles]]. The dynamics of each particle $i$ can be described by its position $\mathbf{r}_i(t)$ and orientation $\theta_i(t)$. The equations of motion in two dimensions are:

$$\dot{\mathbf{r}}_i = v_0 \mathbf{e}(\theta_i) + \mu \sum_{j \neq i} \mathbf{F}_{ij}$$
$$\dot{\theta}_i = \eta_i(t)$$

where $v_0$ is the self-propulsion speed, $\mathbf{e}(\theta) = (\cos \theta, \sin \theta)$ is the orientation vector, $\mu$ is the mobility, $\mathbf{F}_{ij}$ represents interaction forces between particles, and $\eta_i(t)$ is a noise term representing rotational diffusion.

**Phase Diagram and Stability Analysis**

The phase behavior of an active particle system can be explored by analyzing the stability of the uniform (mixed) state against small perturbations. A [[linear stability analysis]], starting from the [[Boltzmann approach]], can be utilized to determine the conditions under which the uniform state becomes unstable, leading to phase separation. This involves examining the interplay between self-propulsion, particle interactions, and [[rotational diffusion]].

**Applications and Implications**

MIPS has implications in understanding biological systems, such as [[bacterial colonies]], where similar segregation phenomena occur due to active motion. It also provides insights into designing [[synthetic active materials]] where control over phase behavior can be used to engineer novel properties and functionalities.

**Advanced Topics**

Further studies in MIPS involve exploring the effects of different types of interactions (e.g., [[alignment interactions]]), particle shapes, and dimensions on the phase behavior. Computational simulations and analytical models are extensively used to predict and analyze the complex behaviors in these [[non-equilibrium systems]].

### Conclusion

Understanding MIPS enriches our knowledge of [[non-equilibrium statistical mechanics]] and active matter, offering a window into the collective behaviors of systems [[far from equilibrium]]. For a comprehensive analysis, readers might explore the foundational models of active Brownian particles and delve into the mathematical theories of non-equilibrium phase transitions, which are crucial for describing such phenomena.