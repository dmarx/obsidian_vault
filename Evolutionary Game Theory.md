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