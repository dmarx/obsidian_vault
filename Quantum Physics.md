>i have a graduate degree in math and statistics: explain to me how probabilities are modeled and composed in quantum mechanics

Given your background in mathematics and statistics, I'll aim for a detailed and technical explanation of how probabilities are modeled and composed in quantum mechanics.

Quantum mechanics fundamentally diverges from classical mechanics by introducing a probabilistic interpretation of physical phenomena. The key mathematical framework used to describe these probabilities is the theory of Hilbert spaces and operators.

### [[Hilbert Spaces]]

In quantum mechanics, the state of a physical system is described by a vector (state vector) in a complex Hilbert space. A Hilbert space is a complete vector space equipped with an inner product that allows measuring angles and lengths. The state vector \(|\psi\rangle\) (often called a "quantum state") encapsulates all the information about the system. The probabilities of various physical outcomes are derived from the properties of these vectors.

### Quantum States and Probability Amplitudes

The probability amplitude is a fundamental concept in quantum mechanics. For a given quantum state \(|\psi\rangle\), the probability amplitude associated with a particular outcome (e.g., the position of a particle) is a complex number whose absolute square gives the probability of observing that outcome when a measurement is made.

If $|\psi\rangle$ is a state vector and $|x\rangle$ represents a state corresponding to observing the system in a particular configuration (e.g., a particle at position \(x\)), then the probability amplitude for this outcome is the inner product \( \langle x|\psi\rangle\). The probability of finding the particle at position \(x\) is given by \(|\langle x|\psi\rangle|^2\).

### [[Operators]] and Observables

In quantum mechanics, physical quantities (observables) such as position, momentum, and energy are represented by operators acting on the Hilbert space. These operators are typically [[Hermitian]] (or self-adjoint), ensuring that their eigenvalues are real numbers, which correspond to the possible outcomes of measurements.

The action of an operator \( \hat{O} \) on a state \( |\psi\rangle \) can project \( |\psi\rangle \) onto an eigenstate \( |o\rangle \) of \( \hat{O} \), with the eigenvalue \( o \) being the observed outcome. The probability of observing \( o \) is given by \( |\langle o|\psi\rangle|^2 \), assuming \( |o\rangle \) and \( |\psi\rangle \) are normalized.

### Superposition and Entanglement

Quantum mechanics allows for the superposition of states, where a quantum system can be in a combination (linear superposition) of multiple states simultaneously. The probabilities of outcomes are influenced by the superposition principle, leading to interference effects.

Entanglement is another quantum phenomenon where the states of two or more particles become correlated in such a way that the state of each particle cannot be described independently of the state of the others, even when the particles are separated by large distances. This leads to correlations in their observed properties that are stronger than what is possible classically.

### Composition of Probabilities

In quantum mechanics, the composition of probabilities often involves the addition of probability amplitudes (rather than probabilities) followed by squaring the absolute value of the total amplitude to find the probability of a combined outcome. This can lead to interference effects, where the probabilities are not additive in the classical sense.

For example, in a double-slit experiment, the probability amplitude of a particle passing through one slit and reaching a screen is added to the amplitude of passing through the other slit before the absolute square is taken to compute the probability of arriving at a particular point on the screen. This results in an interference pattern that is characteristic of quantum systems.

### Mathematical Tools

The formalism of quantum mechanics utilizes various mathematical tools, including linear algebra (for handling vectors and operators in Hilbert space), functional analysis (to deal with infinite-dimensional spaces), and group theory (for understanding symmetries and conservation laws).

Your knowledge of math and statistics provides a solid foundation for delving deeper into these topics, exploring the intricate behaviors of quantum systems, and understanding the underlying probabilistic nature of quantum mechanics.