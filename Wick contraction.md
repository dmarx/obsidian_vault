see also:
- [[Perturbation Methods]]

Wick contraction, named after Gian-Carlo Wick, is a concept in [[quantum field theory]] (QFT) that plays a crucial role in the [[perturbative expansion]] of quantum fields, particularly in the calculation of scattering amplitudes and correlation functions. It formalizes the process of evaluating time-ordered products of field operators by expressing them in terms of normal-ordered products plus additional terms arising from contractions between pairs of field operators. This process is essential for systematically handling interactions in QFT and computing observable quantities.

### Background

In QFT, the dynamics and interactions of quantum fields are described by the [[field operators]]. The perturbative approach, especially in the interaction picture, involves expanding the evolution operator in powers of the interaction [[Hamiltonian]]. This expansion leads to expressions involving time-ordered products of field operators. [[Wick's theorem]] provides a systematic way to deal with these products.

### Definition of Wick Contraction

A Wick [[contraction]] between two field operators is essentially the expectation value of their normal-ordered product in the vacuum state, which corresponds to the propagator between the points at which the operators are evaluated. Graphically, it's often represented as a line connecting the two contracted operators. 

### Wick's Theorem

Wick's theorem states that any time-ordered product of field operators can be rewritten as a sum of normal-ordered products of all possible contractions. Mathematically, for a set of operators \(A_1, A_2, \ldots, A_n\), the theorem expresses the time-ordered product \(T(A_1 A_2 \ldots A_n)\) in terms of normal-ordered products and contractions.

### Application in Feynman Diagrams

Wick contractions are intimately related to the Feynman diagrams that are ubiquitous in the perturbative analysis of QFT. Each contraction corresponds to a line in a Feynman diagram, representing the propagation of a particle between two points (or vertices). The process of performing all possible Wick contractions in a given term of the perturbative expansion corresponds to drawing all possible Feynman diagrams for that term, each associated with a specific contribution to the amplitude or correlation function being calculated.

### Importance

- **Perturbative Calculations:** Wick contractions simplify the calculation of perturbative contributions in QFT, making it feasible to compute scattering amplitudes, transition probabilities, and other physical quantities.
- **Feynman Diagrams:** They provide the mathematical foundation for Feynman diagrams, translating complicated algebraic expressions into intuitive graphical representations that encode the dynamics of particle interactions.
- **Quantum Statistics:** The concept of contraction also highlights the differences between bosons and fermions through the symmetry properties of their respective fields, affecting the sign of terms in the perturbative expansion.

### Challenges

While Wick contractions and Wick's theorem streamline calculations in QFT, the perturbative approach can become increasingly complex at higher orders, involving a rapidly growing number of terms and diagrams to consider. This complexity limits the practical computation of very high-order corrections and motivates the development of non-perturbative techniques and numerical methods for exploring quantum field dynamics beyond the reach of perturbation theory.

Wick's theorem and the associated contractions are foundational to the perturbative approach in QFT, elucidating the structure of quantum field interactions and facilitating the calculation of observable quantities within the framework of quantum theory.