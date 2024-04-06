see also:
- [[Probability Theory]]
- [[Bayesian Interpretation of Probability]]
- [[Frequentist Interpretation of Probability]]
- [[Philosophy of Probability]]
- [[Causal Inference]]
- [[Causal Models]]
- [[probabilistic models]]
- [[Generative Models]]
- [[Statistical Learning Theory]]
- [[Stochastic Processes]]
- [[Probability Measure]]
- [[Event Space]]
- [[Sample Space]]

**Random variables** are foundational concepts in [[probability theory]] and statistics, providing a bridge between outcomes of random phenomena and numerical values. They enable the mathematical treatment of randomness and uncertainty, allowing for the quantification, analysis, and modeling of random processes.

### Definition

A random variable is a function that assigns a [[Real Numbers|real number]] to each outcome in the sample space of a [[random experiment]]. Formally, if $(\Omega, \mathcal{F}, P)$ is a [[probability space]], where $\Omega$ is the [[sample space]], $\mathcal{F}$ is a $\sigma$-algebra of events, and $P$ is a probability measure, then a random variable $X$ is a function:

$$
X: \Omega \rightarrow \mathbb{R}
$$

such that for every [[Borel Sets|Borel set]] $B$ in $\mathbb{R}$, the preimage $X^{-1}(B) = \{\omega \in \Omega: X(\omega) \in B\}$ is an event in $\mathcal{F}$. This condition ensures that probabilities can be assigned to the values taken by the random variable.

### Types of Random Variables

- **Discrete Random Variables**: These have a countable number of possible values. Examples include the number of heads in a series of coin flips or the number of cars passing through an intersection in an hour. The probability distribution of a discrete random variable is given by a probability mass function (PMF).

- **Continuous Random Variables**: These can take on any value within an interval on the real number line. Examples include the height of a randomly selected person or the time required for a chemical reaction to complete. The [[probability distribution]] of a continuous random variable is described by a [[probability density function]] (PDF).

### Important Concepts

- **[[Expectation]] (Expected Value)**: The expectation of a random variable is a measure of its [[central tendency]], essentially a weighted average of all possible values. For a discrete random variable $X$, it is defined as $E[X] = \sum_{x} xP(X=x)$, and for a continuous random variable, as $E[X] = \int_{-\infty}^{\infty} xf(x)dx$, where $f(x)$ is the PDF of $X$.

- **[[Variance]]**: The variance of a random variable measures the [[spread]] of its values around the mean, defined as $Var(X) = E[(X - E[X])^2]$. It quantifies the variability or dispersion of the distribution.

- **Probability Distributions**: The probability distribution of a random variable specifies how probabilities are assigned to each of its possible values. Key distributions include the [[Binomial distribution]] for discrete variables and the Normal ([[Gaussian Kernel|Gaussian]]) distribution for continuous variables.

- **[[Independence]]**: Two random variables $X$ and $Y$ are independent if knowing the value of one provides no information about the value of the other. Mathematically, $X$ and $Y$ are independent if for all $x$ and $y$, $P(X=x \text{ and } Y=y) = P(X=x)P(Y=y)$.

### Applications

Random variables are used across various fields to model uncertainty and variability in processes and experiments, including:

- **Statistics**: For data analysis, hypothesis testing, and inferential statistics to make predictions or inferences from sample data.
- **Finance**: To model risks, returns on investments, and to price derivatives.
- **Engineering**: In reliability engineering and signal processing to model failure times and noise, respectively.
- **Natural Sciences**: To describe the randomness inherent in physical and biological processes.

Understanding random variables and their distributions is crucial for interpreting data, making predictions, and making decisions under uncertainty.

>>A random variable is a function that assigns a real number to each outcome in the sample space of a random experiment
>that sounds like a frequentist interpretation of a "random variable". how do bayesians understand the notion of "random variables"

The Bayesian interpretation of probability, and by extension, random variables, differs significantly from the frequentist perspective. While the frequentist approach views random variables as arising from processes with inherent randomness, the Bayesian interpretation treats random variables as expressions of uncertainty about a quantity's true value.

### Bayesian Perspective on Random Variables

In the Bayesian framework, a random variable represents a quantity whose exact value is uncertain but about which we have some knowledge expressed in the form of a probability distribution. This distribution reflects our beliefs or information about the possible values the variable can take, prior to observing any data. After observing data, Bayesians update their beliefs using Bayes' theorem, resulting in a posterior distribution that reflects updated knowledge about the variable's possible values.

### Key Differences

- **Interpretation of Probability**: Bayesian probability is subjective and represents a degree of belief or confidence in a particular outcome or hypothesis. This contrasts with the frequentist interpretation, which views probability as the long-run frequency of outcomes in repeated experiments.

- **Random Variables**: For Bayesians, random variables do not necessarily originate from random processes; instead, they are quantities with uncertain values. The "randomness" reflects the observer's knowledge or ignorance about the true value rather than inherent randomness in the phenomenon.

- **Prior and Posterior Distributions**: Bayesian analysis starts with a prior distribution representing initial beliefs about a random variable's value. After observing data, Bayes' theorem is used to update this belief, resulting in a posterior distribution. This process highlights how Bayesians incorporate both prior knowledge and new evidence into their understanding of random variables.

### Example: Estimating a Parameter

Consider the task of estimating a parameter $\theta$ (such as the probability of heads in coin flips). 

- **Frequentist Approach**: $\theta$ is considered a fixed but unknown value. A random variable, such as the sample mean from coin flips, is used to make inferences about $\theta$. The variability in the sample mean across different samples reflects the random process of flipping the coin.

- **Bayesian Approach**: $\theta$ itself is treated as a random variable with a prior distribution reflecting what is known or believed about $\theta$ before any data is collected. After data collection, Bayes' theorem is applied to update the prior to a posterior distribution, which represents the updated beliefs about $\theta$'s possible values.

### Conclusion

The Bayesian interpretation of random variables as expressions of uncertainty allows for a more flexible framework that can incorporate prior knowledge and update beliefs in light of new evidence. This contrasts with the frequentist view, which focuses on the inherent randomness of processes generating data. Both perspectives offer valuable insights and tools for statistical analysis, with their applicability depending on the context and the specific questions being addressed.