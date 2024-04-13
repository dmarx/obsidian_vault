see also:
- [[Wick contraction]]
- [[Perturbation Methods]]

Wick's Theorem is a powerful tool in [[quantum field theory]] (QFT) that simplifies the calculation of time-ordered products of operators, which are ubiquitous in perturbative expansions of quantum fields. Named after Gian-Carlo Wick, this theorem provides a systematic way to express time-ordered products, which describe the evolution of quantum systems, in terms of normal-ordered products and contractions, greatly facilitating the computation of scattering amplitudes and other physical observables.

### Overview

In QFT, interactions are often treated perturbatively, leading to expressions involving time-ordered products of field operators. Wick's Theorem enables these expressions to be rewritten in a more manageable form. 

### Statement of Wick's Theorem

Consider a set of operators \(A_1, A_2, \ldots, A_n\). Wick's Theorem states that the time-ordered product of these operators can be expressed as a sum of normal-ordered products with all possible contractions:

$$
T(A_1 A_2 \ldots A_n) = :A_1 A_2 \ldots A_n: + \text{all possible contractions}
$$

Here, \(T(\cdot)\) denotes the time-ordered product, and \( :\cdot: \) denotes the normal-ordered product. A contraction of two operators is essentially the expectation value of their time-ordered product in the vacuum state, minus any normal-ordered product terms. In practical terms, a contraction between two field operators represents the propagator that corresponds to the exchange of a virtual particle between the points (or events) associated with these operators.

### Implications and Applications

- **Simplification of Calculations:** Wick's Theorem is crucial for simplifying calculations in QFT, especially in the context of perturbative expansions where interactions are treated as small corrections to free (non-interacting) theories.

- **Foundation for Feynman Diagrams:** The theorem underpins the use of Feynman diagrams, where each contraction corresponds to a line (or propagator) in a diagram representing the interaction between particles. The full expansion of a time-ordered product into normal-ordered terms and contractions can be visually represented by drawing all possible Feynman diagrams.

- **Versatility:** While initially formulated for quantum electrodynamics (QED), Wick's Theorem is applicable to a wide range of quantum field theories, including those with scalar, fermionic, and vector fields.

### Mathematical Framework

The mathematical framework of Wick's Theorem involves detailed rules for how contractions are performed, especially distinguishing between bosonic (commuting) and fermionic (anticommuting) fields. For fermions, the antisymmetry of operators leads to additional minus signs when permuting operators, affecting the computation of contractions and the structure of the corresponding Feynman diagrams.

### Challenges

Although Wick's Theorem significantly streamlines the calculation of time-ordered products, the complexity of these calculations can still grow rapidly with the order of perturbation theory being considered. Each additional interaction vertex in a Feynman diagram corresponds to higher-order terms in the perturbative expansion, leading to a combinatorial increase in the number of diagrams and contractions that must be calculated.

### Conclusion

Wick's Theorem is a cornerstone of perturbative quantum field theory, enabling the systematic and efficient computation of quantum processes. By translating complex algebraic operations into graphical representations via Feynman diagrams, it not only simplifies calculations but also provides deep insights into the fundamental interactions governing the quantum world.