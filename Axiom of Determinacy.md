see also:
- [[Principle of Determinacy]] (dupe?)

The Axiom of Determinacy (AD) is a fundamental principle in the area of mathematical logic, particularly within set theory and the study of infinite games. It stands as an alternative to the more traditional Axiom of Choice (AC) in certain contexts, offering a different perspective on the nature of sets, particularly those related to infinite processes and decision-making.

### Definition and Statement

The Axiom of Determinacy asserts that for every game of infinite length, where two players alternately pick natural numbers, there exists a winning strategy for at least one of the players. These games are defined over the set of all infinite sequences of natural numbers. The set of sequences for which the first player has a winning strategy is denoted by $A$, and the complement, where the second player has a winning strategy, by $A^c$.

Mathematically, a game $G$ is associated with a subset $A$ of $\mathbb{N}^\mathbb{N}$ (the space of all infinite sequences of natural numbers). Players I and II alternately choose natural numbers to form an infinite sequence. Player I wins if the sequence is in $A$; otherwise, Player II wins. The Axiom of Determinacy posits that for every such subset $A$, either Player I or Player II has a strategy that ensures victory, regardless of the opponent's moves.

### Implications

- **Rejection of the Axiom of Choice**: In the context of Zermelo-Fraenkel set theory (ZF), AD is incompatible with the Axiom of Choice (AC). This is because AC allows for the construction of sets (such as certain well-orderings of the reals) that lead to non-determined games. The choice between AD and AC significantly influences the landscape of mathematical objects and their properties.

- **Descriptive Set Theory**: Under AD, sets of reals that are definable in certain ways (for example, Borel sets, analytic sets, and projective sets) have regular properties that they might not necessarily have under AC. For instance, every set of reals would be Lebesgue measurable, have the property of Baire, and be determinate.

- **Large Cardinals and Inner Models**: The strength of AD in terms of consistency strength is substantial; it implies the existence of large cardinals, which are certain types of infinite numbers that cannot exist in the standard Zermelo-Fraenkel set theory with the Axiom of Choice. The study of models of set theory where AD holds, often involves "inner models" with large cardinals, providing deep insights into the structure of mathematical universes.

### Mathematical Formalism

One formal approach to understanding AD involves the concept of a strategy function. A strategy for a player is a function that prescribes a move (a natural number) based on the history of the game (the sequence of moves made up to that point). Formally, a strategy for Player I could be a function $f: (\mathbb{N}^{\lt\omega}) \rightarrow \mathbb{N}$, where $\mathbb{N}^{\lt\omega}$ represents the set of all finite sequences of natural numbers. Similarly, a strategy for Player II is defined but takes into account the additional move by Player I.

### Real-world Analogies and Philosophical Aspects

The Axiom of Determinacy also invites philosophical interpretation, particularly in discussions about free will, determinism, and the nature of mathematical existence. It suggests a universe where, at least within the confines of the defined games, outcomes are predetermined by the existence of winning strategies, a stark contrast to the inherent indeterminism implied by the Axiom of Choice with its non-constructive selections.

### Conclusion

The Axiom of Determinacy plays a crucial role in modern set theory, offering a rich framework for exploring the foundations of mathematics. By prioritizing the determinacy of infinite games, AD provides a pathway to understanding the structure of sets and the behavior of sequences, enriching the mathematical landscape with its unique implications and philosophical depth.