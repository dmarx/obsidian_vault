see also:
- [[Evolution of Cooperation]]
- [[Evolutionary Psychology]]
- [[Cooperation]]
- [[Morality As Cooperation]]
- [[Game Theory]]
- [[Public Goods Game]]

Evolutionary game theory is a branch of [[game theory]] that draws from [[evolutionary biology]] to study the [[strategic interactions]] among [[rational agents]]. Unlike classical game theory, which focuses on the [[equilibrium]] outcomes of games among fully rational players, evolutionary game theory is more concerned with the dynamics of strategy change in populations over time. This approach is particularly useful for understanding the evolution of behaviors in biological and social systems.

### Key Concepts

1. **Strategies and Payoffs:** Individuals in a population adopt strategies during their interactions. Each strategy has an associated payoff, which depends on the strategy distribution within the population.

2. **[[Evolutionary Stable Strategy]] (ESS):** An ESS is a strategy that, if adopted by a population, cannot be invaded by any alternative strategy that is initially rare. Mathematically, a strategy $S$ is evolutionary stable if for any alternative strategy $T$, either
   $$
   \pi(S, S) > \pi(T, S)
   $$
   or, if $\pi(S, S) = \pi(T, S)$, then
   $$
   \pi(S, T) > \pi(T, T)
   $$
   where $\pi(X, Y)$ denotes the payoff to strategy $X$ when playing against strategy $Y$.

3. **[[Replicator Dynamics]]:** This is a set of differential equations that describe how the proportion of strategies in a population change over time, based on their payoffs. The growth rate of a strategy’s proportion in the population is proportional to the difference between the strategy’s payoff and the average payoff of the population. If $x_i$ represents the proportion of strategy $i$ in the population, and $\pi_i$ its payoff, the [[Replicator Equation]] for strategy $i$ is
   $$
   \frac{dx_i}{dt} = x_i (\pi_i - \bar{\pi})
   $$
   where $\bar{\pi}$ is the average payoff in the population.

4. **[[Population Games]]:** These are games that model the interactions within large populations where the payoff to an individual depends on the distribution of strategies within the entire population, rather than on pairwise interactions.

### Applications

Evolutionary game theory has a wide range of applications across disciplines:

- **Biology:** It helps explain the [[evolution of altruistic behavior]], the [[dynamics of animal conflicts]], and the [[evolution of communication]].
- **Economics:** It's used to model the dynamics of market strategies, where companies evolve through [[competition]] and [[adaptation]].
- **Social Sciences:** The theory provides insights into the evolution of social norms and behaviors.
- **Computer Science:** It's applied in algorithms and artificial intelligence, particularly in machine learning models that evolve strategies for optimization problems.

### Mathematical Foundations

The mathematical treatment of evolutionary game theory involves nonlinear dynamical systems, particularly when analyzing replicator dynamics. Stability analysis, phase portraits, and bifurcation theory are crucial for understanding the behavior of strategies over time.

For a deeper dive into evolutionary game theory, one might explore more sophisticated concepts like the [[Price equation]], which provides a general framework for understanding [[selection processes]], or [[coevolutionary games]], where the payoffs change as the population evolves.

By combining game theory, evolutionary biology, and [[dynamical systems]], evolutionary game theory offers a powerful framework for understanding the complexity of strategic interactions in natural and social systems.

---

[[Evolutionary Game Theory]] (EGT) is a framework that combines classical game theory with evolutionary biology to study the strategic interactions and decision-making processes of individuals in a population. Unlike classical game theory, which often assumes rational players with complete information, EGT focuses on populations of agents whose strategies evolve over time based on their interactions and relative success.

## Key Concepts in Evolutionary Game Theory

### Strategies

In EGT, strategies are the behaviors or actions that individuals in a population can adopt. Strategies can be pure (a specific action) or mixed (a probabilistic combination of actions).

### Payoff and Fitness

The payoff in EGT represents the success or utility that an individual gains from adopting a particular strategy in interactions with others. This payoff influences the individual's fitness, which determines the likelihood of the strategy being passed on to the next generation.

### Evolutionarily Stable Strategy (ESS)

An [[Evolutionarily Stable Strategy]] (ESS) is a strategy that, if adopted by a population, cannot be invaded by any alternative strategy. Formally, a strategy \( S \) is an ESS if, for any alternative strategy \( S' \), the following conditions hold:

1. \( \pi(S, S) > \pi(S', S) \)
2. If \( \pi(S, S) = \pi(S', S) \), then \( \pi(S, S') > \pi(S', S') \)

Here, \( \pi(X, Y) \) denotes the payoff to strategy \( X \) when played against strategy \( Y \).

### [[Replicator Dynamics]]

Replicator dynamics is a mathematical model that describes how the frequency of strategies in a population changes over time based on their relative payoffs. The change in frequency \( x_i \) of strategy \( i \) is given by:

$$
\frac{dx_i}{dt} = x_i (\pi_i - \bar{\pi})
$$

where \( \pi_i \) is the payoff of strategy \( i \) and \( \bar{\pi} \) is the average payoff in the population. This equation indicates that strategies with higher-than-average payoffs will increase in frequency, while those with lower-than-average payoffs will decrease.

### Payoff Matrices and Games

EGT often uses payoff matrices to represent the outcomes of interactions between different strategies. A common example is the [[Hawk-Dove Game]], which models the conflict between aggressive (hawk) and peaceful (dove) strategies. The payoff matrix for the Hawk-Dove game is:

$$
\begin{matrix}
 & \text{Hawk} & \text{Dove} \\
\text{Hawk} & \left(\frac{V-C}{2}, \frac{V-C}{2}\right) & (V, 0) \\
\text{Dove} & (0, V) & \left(\frac{V}{2}, \frac{V}{2}\right)
\end{matrix}
$$

Here, \( V \) represents the value of the resource being contested, and \( C \) represents the cost of fighting. The entries in the matrix represent the payoffs for the strategies in different interactions.

## Applications of Evolutionary Game Theory

### Biological Evolution

EGT was originally developed to study the evolution of behaviors in biological populations. It helps explain the emergence of cooperative behaviors, mating strategies, and social hierarchies. For example, the [[Prisoner's Dilemma]] game is used to study the evolution of cooperation among individuals.

### Social and Cultural Evolution

EGT is applied to understand the evolution of social norms, cultural practices, and institutional rules. By modeling interactions within a population, researchers can study how certain behaviors become dominant or stable over time.

### Economics and Behavioral Sciences

In economics, EGT is used to analyze markets, competition, and the evolution of preferences and strategies among consumers and firms. It helps explain phenomena such as the emergence of conventions, market equilibria, and the stability of economic behaviors.

### Political Science

EGT is utilized to study voting behavior, coalition formation, and conflict resolution. It provides insights into how political strategies evolve and stabilize within populations.

### Ecology and Environmental Science

EGT models interactions between species, such as predator-prey dynamics, competition, and cooperation. It helps understand the evolution of ecological strategies and the stability of ecosystems.

## Mathematical Modeling in EGT

### Example: [[Hawk-Dove Game]]

To illustrate the application of replicator dynamics, consider the Hawk-Dove game. Let \( x \) be the proportion of hawks in the population, and \( 1-x \) be the proportion of doves. The average payoffs for hawks (\( \pi_H \)) and doves (\( \pi_D \)) are:

$$
\pi_H = x \left(\frac{V - C}{2}\right) + (1 - x)V
$$

$$
\pi_D = x(0) + (1 - x)\left(\frac{V}{2}\right)
$$

The average payoff in the population (\( \bar{\pi} \)) is:

$$
\bar{\pi} = x \pi_H + (1 - x) \pi_D
$$

Using replicator dynamics, the change in the frequency of hawks (\( x \)) over time is:

$$
\frac{dx}{dt} = x (\pi_H - \bar{\pi})
$$

This model allows us to analyze the stability of the hawk and dove strategies and predict the equilibrium proportions of each strategy in the population.

## Evolutionary Stability and Mixed Strategies

### Mixed Strategies

In some games, individuals adopt mixed strategies, where they probabilistically choose between different pure strategies. For example, in the Hawk-Dove game, a mixed strategy might involve playing hawk with probability \( p \) and dove with probability \( 1 - p \).

### Calculating ESS for Mixed Strategies

To determine if a mixed strategy is an ESS, we calculate the expected payoffs for the mixed strategy against itself and against pure strategies. The mixed strategy is an ESS if it satisfies the conditions for evolutionary stability.

## Summary

Evolutionary Game Theory provides a powerful framework for studying the evolution of strategies and behaviors in populations. By incorporating concepts from game theory and evolutionary biology, EGT explains how certain strategies become dominant or stable over time. It has broad applications across biology, social sciences, economics, political science, and ecology, offering insights into the dynamics of competition, cooperation, and strategic interactions.