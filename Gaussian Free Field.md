see also:
- [[free field theory]]
- [[Gaussian Processes]]

### Introduction to Gaussian Free Fields

Gaussian Free Fields (GFF), also known as Gaussian random fields or free field theory in the context of quantum field theory, represent a fundamental class of random fields with Gaussian distributions. These fields are extensively used to model a variety of phenomena across physics, probability theory, and mathematical finance. The GFF can be seen as the Gaussian analogue of the Brownian motion, but extended to higher dimensions.

### Definition of Gaussian Free Fields

A Gaussian Free Field is a generalization of Gaussian processes to functions defined over a domain in a higher-dimensional space (usually \( \mathbb{R}^d \) or a subset thereof). The field is characterized by its mean and covariance structure, and every finite collection of its values forms a multivariate Gaussian distribution.

#### Mathematical Formulation

Consider a domain \( D \subseteq \mathbb{R}^d \). A GFF on this domain is a random function \( \phi : D \rightarrow \mathbb{R} \) such that for any finite set of points \( x_1, x_2, ..., x_n \in D \), the values \( \phi(x_1), \phi(x_2), ..., \phi(x_n) \) are jointly Gaussian with:
- Mean zero: \( \mathbb{E}[\phi(x)] = 0 \) for all \( x \in D \),
- Covariance given by the Green's function \( G \) of the Laplacian \( \Delta \) on \( D \) with appropriate boundary conditions, such that:
  $$
  \mathbb{E}[\phi(x) \phi(y)] = G(x, y).
  $$

The Green's function \( G(x, y) \) represents the fundamental solution to the Laplace equation and describes how influence propagates from point \( y \) to point \( x \) within the field.

### Properties and Interpretations

- **Markov Property**: Like the Brownian motion, the Gaussian Free Field exhibits a form of the Markov property in spatial domains. This implies that the field inside a subdomain \( D' \subset D \), conditioned on the values on the boundary of \( D' \), is independent of the field outside \( D' \).
- **Conformal Invariance**: In two dimensions, the GFF exhibits conformal invariance, making it a key object in conformal field theory and the study of critical phenomena in statistical physics.
- **Log-Correlated Fields**: In certain cases, particularly in two dimensions, the covariance structure of the GFF leads to logarithmic correlations, indicating that \( G(x, y) \) behaves like \( -\log |x - y| \) as \( y \) approaches \( x \).

### Applications of Gaussian Free Fields

- **Quantum Field Theory**: GFFs serve as a simplified model for studying quantum fields, particularly in understanding the properties of fields without interactions.
- **Statistical Mechanics**: GFFs are used to model height functions in dimer models and other systems exhibiting Gaussian fluctuations.
- **Mathematical Finance**: Variants of Gaussian Free Fields are employed to model spatial correlations in financial variables or risks.

### Computation and Simulation

Simulating and computing properties of Gaussian Free Fields often involves numerical solutions to partial differential equations (PDEs) to approximate the Green's function, especially in complex domains. Monte Carlo methods and finite element methods are commonly used for these purposes.

### Conclusion

The Gaussian Free Field is a versatile and powerful tool in theoretical and applied mathematics, capable of describing spatial random processes with Gaussian properties. Its foundational role in fields such as quantum field theory and statistical mechanics underscores its importance in bridging mathematical theory with physical phenomena, providing insights into both the behavior of fundamental particles and the emergent properties of complex systems.