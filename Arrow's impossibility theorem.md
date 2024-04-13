see also:
- [[Game Theory]]
- [[Economics]]

[[Arrow's Impossibility Theorem]], formulated by economist Kenneth Arrow in his doctoral thesis and later published in his book "Social Choice and Individual Values" (1951), is a landmark result in social choice theory and economics. The theorem demonstrates a fundamental paradox in voting and [[Collective Decision Making]] systems: it is impossible to design a voting system that simultaneously fulfills a set of seemingly reasonable and desirable criteria for fair and rational collective decision-making. 

### Criteria for a [[Fair Voting System]]

Arrow's theorem considers a [[Voting Systems|voting system]] that tries to aggregate the preferences of individuals over a set of three or more options (or candidates) into a complete, transitive preference ordering for the society as a whole. Arrow defined the following axioms that any fair voting system should satisfy:

1. **Non-Dictatorship:** No single individual's preferences should dictate the group's preference ordering, regardless of the preferences of the other members of the group.

2. **[[Pareto Efficiency]] (Unanimity):** If every individual in a group prefers one option over another, then the group preference should also reflect a preference for that option over the other.

3. **Independence of Irrelevant Alternatives (IIA):** The group's preference between any two options should not be affected by changes in the ranking of other options. In other words, the ranking between any two options depends only on the individual rankings of these two options, not on whether a third option is available.

4. **Universal Domain (Unrestricted Domain):** The voting system should be able to process any set of individual preferences to produce a group preference. That is, the system should work for any possible configuration of individual rankings of the options.

### Statement of the Theorem

Arrow's impossibility theorem states that no voting system can satisfy all four of these criteria simultaneously if there are three or more options to choose from. This implies that all voting systems must, in some situations, violate at least one of the principles of fairness or rationality as defined by Arrow.

### Mathematical Formalization

To formalize Arrow's theorem, consider a set $A$ of alternatives with $|A| \geq 3$. Let $N$ be a set of individuals. A social welfare function $F$ takes as input a profile of individual preferences (complete, transitive orders over $A$) and produces a complete, transitive social preference order over $A$. Arrow's conditions can be formalized as follows:

1. **Non-Dictatorship:** $\nexists i \in N$ such that for all preference profiles, the social preference order is always the preference order of individual $i$.

2. **Pareto Efficiency:** For any two alternatives $x, y \in A$, if every individual prefers $x$ to $y$, then the social preference should also prefer $x$ to $y$.

3. **Independence of Irrelevant Alternatives:** For any two alternatives $x, y \in A$, the social preference between $x$ and $y$ depends only on the individuals' preferences between $x$ and $y$, unaffected by individuals' preferences regarding other alternatives.

4. **Universal Domain:** The social welfare function $F$ must produce a social preference order for any possible set of individual preference orders over $A$.

Arrow's theorem is then: Given the set of alternatives $A$ where $|A| \geq 3$, there is no social welfare function $F$ that satisfies Non-Dictatorship, Pareto Efficiency, Independence of Irrelevant Alternatives, and Universal Domain simultaneously.

### Implications and Interpretations

The implications of Arrow's theorem are profound, suggesting inherent limitations in the design of collective decision-making processes. It highlights trade-offs that must be considered in the design of electoral systems, decision-making in organizations, and other contexts where group preferences need to be aggregated. The theorem has spurred a vast amount of research in economics, political science, and philosophy, exploring ways to navigate these limitations, alternative axioms, and decision-making frameworks that might circumvent Arrow's constraints.