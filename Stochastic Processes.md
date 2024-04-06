see also:
- [[Probability Theory]]
- [[Measure Theory]]
- [[Partial Differential Equations]]
- [[Stochastic Simulation]]
- [[Stochastic Optimization]]
- [[Stochastic Differential Equations]]

**Stochastic processes** are mathematical objects used to model systems or phenomena that evolve over time in a way that involves randomness or uncertainty. They are fundamental in various fields, including finance, physics, biology, and engineering, providing a framework for analyzing temporal changes in random systems.

### Definition

A stochastic process is a collection of [[Random Variables]] $\{X(t): t \in T\}$ defined on a common [[probability space]] $(\Omega, \mathcal{F}, P)$, where:

- $\Omega$ is the sample space, representing all possible outcomes.
- $\mathcal{F}$ is a $\sigma$-algebra on $\Omega$, representing the events to which probabilities are assigned.
- $P$ is a [[probability measure]] that assigns probabilities to the events in $\mathcal{F}$.
- $X(t)$ is a random variable corresponding to each point $t$ in the index set $T$. The index set $T$ often represents time, which can be discrete ($T = \{0, 1, 2, \ldots\}$) or continuous ($T = [0, \infty)$).
- Each random variable $X(t)$ maps outcomes in $\Omega$ to states in a state space $S$, which could be the set of real numbers $\mathbb{R}$, a set of integers, or more complex structures.

### Types of Stochastic Processes

- **Discrete-Time Processes**: Where the index set $T$ is countable. An example is a random walk, where an entity's position changes at discrete time intervals according to some random rule.

- **Continuous-Time Processes**: Where $T$ is uncountable, typically an interval or the entire set of non-negative real numbers. The Wiener process (or Brownian motion) is a classic example, modeling phenomena like the erratic motion of pollen particles in fluid.

### Key Concepts and Examples

- **Markov Processes**: These processes have the property that the future state depends only on the current state, not on the sequence of events that preceded it. The Markov property simplifies analysis and modeling of stochastic processes.

- **Poisson Processes**: Used to model the occurrence of events that happen independently of each other at a constant average rate, such as calls arriving at a call center or radioactive decay.

- **Wiener Process (Brownian Motion)**: A continuous-time process with continuous paths that models random movement, foundational in mathematical finance for modeling stock prices and in physics for diffusion processes.

- **Martingales**: A type of stochastic process that models a fair game, where the conditional expectation of the next value, given all prior values, is equal to the present value. Martingales are central in probability theory and financial mathematics.

### Applications

- **Financial Mathematics**: Stochastic processes are used to model stock prices, interest rates, and the evolution of financial markets. The Black-Scholes model for option pricing, which involves a Wiener process, is a seminal example.

- **[[Queueing Theory]]**: The analysis of queues (e.g., people waiting in line, data packets in networks) uses stochastic processes to model the arrival and service processes, helping optimize service systems.

- **Epidemiology**: Modeling the spread of diseases through populations, where the number of infected individuals over time can be modeled by stochastic processes.

- **Physics and Chemistry**: Modeling random phenomena such as particle motion (Brownian motion), radioactive decay, and noise in electronic circuits.

Stochastic processes provide powerful tools for modeling and analyzing systems where uncertainty and randomness play a crucial role, enabling predictions, simulations, and insights into the behavior of complex dynamical systems across diverse disciplines.