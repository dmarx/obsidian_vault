Particle filters, also known as [[Sequential Monte Carlo]] methods, are a set of advanced algorithms used for estimating the state of a dynamic system where the state is partially observed and can evolve over time. Unlike the Kalman filter, which is optimal for linear systems with Gaussian noise, particle filters are designed to handle non-linear systems with non-Gaussian noise, making them highly versatile and applicable to a wide range of complex systems.

### How Particle Filters Work

The core idea behind particle filters is to represent the required posterior distribution of the state variables by a set of random samples (particles) with associated weights. These particles are propagated over time, and their distribution approximates the probability distribution of the system's state.

1. **Initialization**: The filter starts by generating a set of particles, each representing a possible state of the system, usually drawn from the prior distribution or based on an initial guess.

2. **Prediction**: For each time step, the particles are propagated according to the system's model dynamics, incorporating any process noise. This step predicts the next state of each particle.

3. **Update**: When a new measurement is obtained, the weights of the particles are updated based on the likelihood of the observed measurement given the particle's predicted state. This step incorporates the measurement information, adjusting the belief about the system's state.

4. **[[Resampling]]**: Over time, some particles may acquire very low weights and contribute little to the representation of the posterior distribution. The resampling step involves generating a new set of particles by drawing with replacement from the current set, where the probability of drawing each particle is proportional to its weight. This process focuses the particle set on regions of higher likelihood, combating degeneracy and ensuring diversity among the particles.

5. **Estimation**: The estimate of the system's state is obtained by aggregating the particles, typically as a weighted average based on their weights, which can provide a point estimate, or by using the particles to approximate the entire posterior distribution of the state.

### Applications

Particle filters are widely used in various domains, including:

- **Robotics**: For localization and mapping, enabling robots to navigate and understand their environment.
- **Computer Vision**: In tracking objects across image sequences, even under occlusion or when the objects' motion is non-linear.
- **[[Signal Processing]]**: For [[denoising]] signals and extracting useful information from noisy measurements.
- **Economics and Finance**: For estimating the states of non-linear models of economies or financial markets.
- **Biomedical Engineering**: In tracking the state of biological systems, such as the spread of diseases.

### Advantages and Limitations

**Advantages**:
- Flexibility to model non-linear and non-Gaussian problems.
- The ability to represent multimodal distributions, capturing multiple hypotheses about the system's state.
- Incremental update mechanism, suitable for real-time applications.

**Limitations**:
- Computationally intensive, especially with a large number of particles.
- The choice of proposal distribution and resampling strategy can significantly affect performance.
- Suffers from the curse of dimensionality, with the required number of particles growing exponentially with the dimension of the state space.

Despite these limitations, particle filters remain a powerful tool for state estimation in [[Complex Systems Theory|complex systems]], providing a flexible framework to incorporate [[nonlinear dynamics]] and non-Gaussian noise.