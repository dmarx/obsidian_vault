see also:
- [[Self-Organization]]
- [[Criticality]]
- [[Complexity Theory]]

[[Self-organized criticality]] (SOC) is a concept in the field of complex systems and statistical physics that describes how certain dissipative systems naturally evolve into a critical state, where a minor event can lead to significant, widespread consequences. This concept was first introduced by Per Bak, Chao Tang, and Kurt Wiesenfeld in a 1987 paper as a way to explain the widespread occurrence of [[power-law distributions]] (e.g., [[Pink Noise|1/f noise]], [[fractal structures]]) in nature. SOC systems display features like [[scale invariance]] and a lack of [[characteristic length]] scales, which are typical of [[critical points]] found in second-order [[phase transitions]], but without the need to fine-tune external parameters to reach such a state.

### Mathematical Framework and Models

A classical example of SOC is the [[sandpile model]]. Imagine starting with a flat sandpile onto which sand is slowly dropped one grain at a time. Over time, the pile grows until it reaches a critical slope. At this point, adding a single grain of sand can cause an avalanche. The size of these avalanches can vary greatly, from a single grain falling to a few others, to massive slides involving a large fraction of the pile. Remarkably, the distribution of avalanche sizes follows a power law, a signature of SOC.

The dynamics of SOC systems are often modeled using cellular automata or agent-based models. The sandpile model, for instance, can be represented on a lattice where each site has a state corresponding to the slope or the height of the sandpile at that point. Rules for the sandpile evolution involve redistributing sand among neighboring sites when a critical slope is exceeded, mimicking the avalanche process.

Mathematically, the state of the system $S$ at time $t+1$ can be expressed as a function of its state at time $t$, considering the local interaction rules $R$ and the addition of external perturbations $\xi(t)$:

$$S(t+1) = R(S(t), \xi(t))$$

In the sandpile model, $\xi(t)$ would represent the dropping of sand at time $t$, and $R$ embodies the rules for how sand is redistributed in the event of an avalanche.

### Key Properties

1. **[[Scale Invariance]]:** SOC systems do not have a characteristic scale; phenomena within them follow power-law distributions, meaning there is self-similarity across scales. Mathematically, if $P(s)$ is the probability of an avalanche of size $s$, it follows that $P(s) \sim s^{-\tau}$, where $\tau$ is a critical exponent.
   
2. **[[Criticality]]:** The system self-tunes to a critical state where it is poised on the "[[edge of chaos]]." In this state, the system exhibits a delicate balance between [[stability]] and dynamism, enabling it to respond to external perturbations with a wide range of outcomes.

3. **[[Punctuated Equilibrium]]:** SOC systems are characterized by long periods of stability interrupted by sudden changes, analogous to the evolutionary theory of punctuated equilibrium. This behavior contrasts with systems in equilibrium, where changes occur gradually and predictably.

### Applications and Implications

SOC has been invoked to explain phenomena in various domains, including:
- **Geophysics:** The frequency and magnitude of earthquakes follow a power-law distribution, similar to avalanches in the sandpile model.
- **Biology:** Patterns of neural activity and evolution dynamics have been analyzed through the lens of SOC, suggesting that living systems may operate near criticality to maximize responsiveness and [[adaptability]].
- **Financial Markets:** Fluctuations in stock market prices and trade volumes exhibit signs of SOC, with large events (market crashes) being statistically similar to smaller fluctuations on a logarithmic scale.

SOC represents a powerful framework for understanding the dynamics of complex systems, highlighting how simple local interactions can lead to emergent global behaviors that are both unpredictable and self-sustaining. The study of SOC challenges traditional notions of equilibrium and stability in systems, offering insights into the mechanisms that drive complexity in nature.