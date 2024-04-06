---
tags:
  - green
  - root
  - needs-outlinks
---
see also:
- [[Competition]]
- [[Competition models]]
- [[Coordination Games]]
- [[cooperative behavior]]
- [[Cooperative and Competitive Dynamics]]
- [[Economics]]
- [[Decision Process]]
- [[Markov Decision Process]]
- [[Optimization]]
- [[Control Theory]]
- [[Evolutionary Dynamics]]
- [[Evolutionary Game Theory]]
- [[Population Games]]
- [[coevolutionary games]]

Game theory is a mathematical framework designed for analyzing situations in which players make strategic decisions, aiming to maximize their own benefits while considering the choices of others. It is applicable across various disciplines, including economics, political science, psychology, and biology. At its core, game theory studies games of strategy, not of chance, and focuses on games that involve multiple actors (referred to as "players") who make decisions that impact their own outcome and possibly the outcomes of others.

### Key Concepts

1. **Players**: The decision-makers in the game. In game theory, a player can be an individual, a group of individuals, a firm, or any entity making strategic decisions.

2. **Strategies**: A strategy is a complete plan of action a player will follow in given circumstances within a game. It defines the choices a player will make in every possible situation they could face.

3. **Payoffs**: The outcome or reward a player receives from a set of strategies chosen by all players. Payoffs can be any measure of value players aim to maximize or minimize, such as profit, utility, satisfaction, etc.

4. **Games**: Structured strategic interactions among players. Games can be classified in several ways:
   - **Cooperative vs. Non-cooperative**: Cooperative games allow for binding agreements among players, whereas non-cooperative games do not.
   - **Zero-sum vs. Non-zero-sum**: In zero-sum games, one player's gain is another's loss. Non-zero-sum games can have outcomes where all players benefit.
   - **Simultaneous vs. Sequential**: In simultaneous games, players make decisions without knowledge of the others' choices. In sequential games, players make decisions one after another, with knowledge of previous actions.
   - **Static vs. Dynamic**: Static games occur in one stage, while dynamic games have multiple stages, possibly with evolving strategies and states.

5. **[[Equilibrium]] Concepts**:
   - **[[Nash Equilibrium]]**: A set of strategies where no player can benefit by unilaterally changing their strategy, given the strategies of the other players. It is a key concept in non-cooperative game theory.
   - **[[Pareto Optimality]]**: A state of allocation of resources in which it is impossible to make any one individual better off without making at least one individual worse off.

### Mathematical Formalism

Game theory often employs mathematical structures like matrices to represent simple games and more complex formulations for extensive games. A classic representation of a game in strategic form is a payoff matrix, especially for 2-player games. 

Consider a two-player game where each player has two strategies. The payoff matrix might look like this:

$$
\begin{pmatrix}
(a, b) & (c, d) \\
(e, f) & (g, h)
\end{pmatrix}
$$

Here, each cell of the matrix represents the payoffs to the players for each combination of strategies: the first element of each tuple is the payoff to Player 1, and the second is the payoff to Player 2. For example, if Player 1 chooses the first strategy and Player 2 chooses the second, the payoffs would be $c$ to Player 1 and $d$ to Player 2.

### Nash Equilibrium in Mathematical Terms

A Nash Equilibrium occurs when each player's strategy is optimal given the strategies of all other players. Mathematically, let $s_i$ be the strategy chosen by player $i$, and let $S_i$ be the set of possible strategies for player $i$. A strategy profile $(s_1^*, s_2^*, \dots, s_n^*)$ is a Nash Equilibrium if for every player $i$, we have:

$$
u_i(s_i^*, s_{-i}^*) \geq u_i(s_i, s_{-i}^*) \quad \forall s_i \in S_i
$$

where $u_i(s_i, s_{-i})$ is the payoff function for player $i$, $s_i^*$ is player $i$'s strategy in the equilibrium, and $s_{-i}^*$ represents the strategy profiles of all other players except $i$.

### Applications and Limitations

Game theory's applications are widespread, influencing strategies in economics ([[market competition]], [[auctions]]), political science ([[voting systems]], [[conflict resolution]]), biology ([[evolutionary strategies]]), and beyond. However, its real-world applicability can be limited by [[assumptions of rationality]], [[information completeness]], and the challenges in accurately modeling complex strategic interactions.

Understanding game theory requires a solid grasp of mathematical concepts and logical reasoning, making it a fascinating intersection of mathematics, logic, and human behavior. It serves as a foundational tool in [[Economics|economic analysis]], [[Political Science|political strategy]], and [[strategic decision-making]] in various fields.