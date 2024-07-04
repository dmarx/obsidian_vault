Replicator dynamics is a mathematical framework used in [[Evolutionary Game Theory]] (EGT) to model how the frequency of strategies or traits in a population evolves over time based on their relative success. It provides a dynamic description of how advantageous strategies spread and disadvantageous strategies decline within a population.

## Basic Concepts

### Strategy Frequencies

Let \( x_i \) represent the frequency of strategy \( i \) in the population. The sum of the frequencies of all strategies in the population is 1:

$$
\sum_{i} x_i = 1
$$

### Payoff Matrix

The success of a strategy depends on its payoff when interacting with other strategies. The payoff matrix \( A \) defines the payoffs for each strategy pair. If \( a_{ij} \) is the payoff to strategy \( i \) when played against strategy \( j \), the average payoff \( \pi_i \) to strategy \( i \) is:

$$
\pi_i = \sum_{j} a_{ij} x_j
$$

### Average Population Payoff

The average payoff \( \bar{\pi} \) of the population is the weighted sum of the payoffs of all strategies:

$$
\bar{\pi} = \sum_{i} x_i \pi_i = \sum_{i} x_i \sum_{j} a_{ij} x_j
$$

### Replicator Equation

The change in frequency \( x_i \) of strategy \( i \) over time is given by the replicator equation:

$$
\frac{dx_i}{dt} = x_i (\pi_i - \bar{\pi})
$$

This equation indicates that the frequency of strategy \( i \) increases if its payoff \( \pi_i \) is greater than the average population payoff \( \bar{\pi} \), and decreases if its payoff is less.

## Interpretation

The replicator dynamics equation shows that strategies with above-average payoffs increase in frequency, while those with below-average payoffs decrease. Over time, the population composition evolves towards strategies that yield higher payoffs.

## Example: Hawk-Dove Game

The [[Hawk-Dove Game]] models conflict between two strategies: Hawk (aggressive) and Dove (peaceful). The payoff matrix \( A \) is:

$$
A = \begin{pmatrix}
\frac{V-C}{2} & V \\
0 & \frac{V}{2}
\end{pmatrix}
$$

where \( V \) is the value of the resource, and \( C \) is the cost of fighting.

Let \( x \) be the frequency of Hawks in the population, and \( 1-x \) be the frequency of Doves. The average payoffs for Hawks (\( \pi_H \)) and Doves (\( \pi_D \)) are:

$$
\pi_H = x \left(\frac{V - C}{2}\right) + (1 - x)V
$$

$$
\pi_D = x(0) + (1 - x)\left(\frac{V}{2}\right)
$$

The average population payoff \( \bar{\pi} \) is:

$$
\bar{\pi} = x \pi_H + (1 - x) \pi_D
$$

The replicator equation for Hawks is:

$$
\frac{dx}{dt} = x (\pi_H - \bar{\pi})
$$

### Stability Analysis

To find the equilibrium points, set \( \frac{dx}{dt} = 0 \):

$$
x (\pi_H - \bar{\pi}) = 0
$$

This occurs when \( x = 0 \), \( x = 1 \), or \( \pi_H = \bar{\pi} \). Solving \( \pi_H = \bar{\pi} \) gives the internal equilibrium frequency of Hawks:

$$
x^* = \frac{V}{C}
$$

### Interpretation

- When \( x = 0 \), the population consists entirely of Doves.
- When \( x = 1 \), the population consists entirely of Hawks.
- When \( x = \frac{V}{C} \), there is a mixed equilibrium where both strategies coexist.

The stability of these equilibria can be analyzed by examining the sign of \( \frac{dx}{dt} \) near the equilibrium points. If \( \frac{dx}{dt} \) changes sign appropriately, the equilibrium is stable.

## Extensions of Replicator Dynamics

### Multi-Strategy Models

For more than two strategies, the replicator dynamics extend to higher dimensions. Let \( \mathbf{x} \) be the vector of strategy frequencies, and \( A \) be the payoff matrix. The replicator equation in matrix form is:

$$
\frac{d\mathbf{x}}{dt} = \mathbf{x} \circ (A \mathbf{x} - \bar{\pi})
$$

where \( \circ \) denotes the element-wise product, and \( \bar{\pi} = \mathbf{x}^T A \mathbf{x} \).

### Stochastic Replicator Dynamics

In stochastic environments, the replicator dynamics can be modified to include random fluctuations. This is modeled by adding noise terms to the replicator equations, capturing the effect of random events on strategy frequencies.

### [[Adaptive Dynamics]]

Adaptive dynamics extends replicator dynamics by considering the continuous evolution of strategies. Instead of fixed strategies, individuals can adopt new strategies through small mutations, leading to a continuous adaptation process.

## Applications of Replicator Dynamics

### Biological Evolution

Replicator dynamics is used to model the evolution of traits in biological populations, explaining the stability and diversity of behaviors such as cooperation, competition, and mating strategies.

### Economics

In economics, replicator dynamics helps analyze the evolution of market strategies, consumer behavior, and the stability of equilibria in competitive environments.

### Social Dynamics

Replicator dynamics models the spread of social norms, cultural traits, and technological innovations within populations, providing insights into how certain behaviors become dominant.

### Ecology

In ecology, replicator dynamics is used to study the interactions between species, such as predator-prey dynamics, competition, and mutualism, and to understand the stability of ecological communities.

In summary, replicator dynamics provides a powerful mathematical framework for studying the evolution of strategies in populations. By modeling how the frequency of strategies changes over time based on their relative success, it offers insights into the stability and dynamics of various evolutionary and social processes.