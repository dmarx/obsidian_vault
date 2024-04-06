see also:
- [[Statistical Learning Theory]]
- [[Borel Sets]]
- [[Borel Measures]]
- [[Philosophy of Probability]]
- [[Countability]]

A **probability measure** is a fundamental concept in [[probability theory]], formalizing the intuitive idea of assigning "chances" or "likelihoods" to the occurrence of events within a mathematical framework. It extends the notion of [[measure]] from [[measure theory]] to the specific context of probability, allowing for a rigorous analysis of random events, their properties, and relationships.

### Definition

Let $(\Omega, \mathcal{F}, P)$ be a probability space, where:

- $\Omega$ is the [[sample space]], representing the set of all possible outcomes of a random experiment.
- $\mathcal{F}$ is a $\sigma$-algebra on $\Omega$, representing the collection of events (subsets of $\Omega$) to which probabilities can be assigned. The elements of $\mathcal{F}$ are called measurable sets.
- $P: \mathcal{F} \rightarrow [0, 1]$ is the probability measure, a function that assigns to each event $A \in \mathcal{F}$ a number $P(A)$, interpreted as the probability of $A$.

The probability measure $P$ satisfies the following axioms:

1. **Non-negativity**: For any event $A \in \mathcal{F}$, $P(A) \geq 0$.
2. **Normalization**: The probability of the entire sample space is 1, $P(\Omega) = 1$.
3. **Countable Additivity (or σ-additivity)**: For any countable sequence of pairwise disjoint events $A_1, A_2, \ldots \in \mathcal{F}$, the probability of their union is equal to the sum of their individual probabilities:

$$
P\left(\bigcup_{i=1}^{\infty} A_i\right) = \sum_{i=1}^{\infty} P(A_i).
$$

### Properties and Consequences

- **Probability of the Empty Set**: $P(\emptyset) = 0$, since the empty set represents an impossible event.
- **Finite Additivity**: If $A$ and $B$ are disjoint events, then $P(A \cup B) = P(A) + P(B)$.
- **Complement Rule**: The probability of the complement of an event $A$ is $P(A^c) = 1 - P(A)$.
- **Subadditivity**: For any sequence of events $A_1, A_2, \ldots$, not necessarily disjoint, $P\left(\bigcup_{i=1}^{\infty} A_i\right) \leq \sum_{i=1}^{\infty} P(A_i)$.
- **Continuity from Below**: If $A_1 \subseteq A_2 \subseteq \ldots$ is an increasing sequence of events, then $P\left(\bigcup_{i=1}^{\infty} A_i\right) = \lim_{i \to \infty} P(A_i)$.
- **Continuity from Above**: If $A_1 \supseteq A_2 \supseteq \ldots$ is a decreasing sequence of events and at least one $A_i$ has finite probability, then $P\left(\bigcap_{i=1}^{\infty} A_i\right) = \lim_{i \to \infty} P(A_i)$.

### Applications

Probability measures are essential in all branches of probability and statistics, including:

- **[[Descriptive Statistics]]**: For summarizing and understanding data distributions.
- **[[Inferential Statistics]]**: For making predictions or inferences about a population based on sample data.
- **[[Stochastic Processes]]**: For modeling processes that evolve over time in a random manner, such as stock prices, weather patterns, and many others.

Probability measures provide the mathematical underpinning for quantifying uncertainty and randomness, enabling the systematic study and application of probabilistic concepts across a wide range of disciplines.