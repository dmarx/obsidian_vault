see also:
- [[A Statistical Argument For Settling]]

David Marx's blog post "A Statistical Argument For Settling: a foray into extreme value theory" provides an engaging exploration into the statistical challenges of expecting to continually find "better" partners, especially when such judgments are based on subjective experiences like sexual performance. Marx employs the concepts of order statistics and extreme value theory to frame his argument.

### High Standards and Statistical Reality

Marx introduces the scenario of a person seeking to find the best possible partner based on sexual performance, which is a classic setup for introducing order statistics in a real-world context. By taking \( m \) as the maximum of all observed performances, the question becomes: How likely is it to meet someone better after observing \( n \) partners?

### The Role of the Geometric Distribution

In the post, Marx uses the geometric distribution to model the waiting time until a new maximum is observed. The key parameter here is \( p \), the probability of observing a new maximum. This is calculated as the complement of the cumulative distribution function (CDF) at \( m \), \( 1 - F(m) \).

### Extreme Value Theory

Marx doesn't delve too deeply into the specific distributions underpinning extreme value theory, but his analysis leans on the principles that govern these distributions. The general approach to extreme value theory in his context would look at the distribution of the maximum values among a set of observations.

### Weibull Distribution Connection

Although Marx's post doesn't explicitly involve the Weibull distribution, this distribution could be particularly relevant if we consider the context of failure times (analogous to "failing" to meet a new maximum). In extreme value theory:
- If the Weibull parameter \( k < 1 \), the distribution models the minimum values, which isn’t directly relevant here.
- If \( k > 1 \), it could model maximums if the scenario fits.

### Interpretation and Application

The real take-home message from Marx's exploration is the diminishing likelihood of finding a new "best" as one's sample of experiences grows, a classic illustration of the "law of diminishing returns" in a statistical context. This ties back to the idea that setting unrealistically high standards—like needing a partner to be the best ever encountered in a particular subjective category—can lead to long waits or disappointment, effectively supporting the idea of "settling" as a statistically sound strategy.

Marx's approach of using statistical models to analyze human relationships provides a fresh perspective on decision-making in personal domains, highlighting how understanding statistical principles can lead to more informed life choices.

>demonstrate how someone intimately familiar with the principles of extreme value theory might approach this problem (given Marx's approach was limited due to their lack of exposure to that topic)

To approach the problem set out in David Marx's blog post from a more thorough extreme value theory (EVT) perspective, one would focus on rigorously modeling the distribution of maximums and determining the probability of observing a new maximum. Here's how an expert in EVT might frame and analyze the scenario:

### Step 1: Defining the Statistical Model

The expert would start by defining the problem in terms of statistical distributions:
- **Assume a distribution for sexual performance scores:** For simplicity, one could assume that the performance scores follow a normal distribution \( X \sim N(\mu, \sigma^2) \), but the expert could consider other distributions based on empirical data or theoretical considerations.
- **Transform the problem using extreme value theory:** Recognizing that the issue deals with maximum values, an expert would apply EVT, which deals with three types of maxima distributions known as the Gumbel, Fréchet, and Weibull distributions. The choice depends on the tail behavior of the underlying distribution of the data.

### Step 2: Applying the Block Maxima Model

- **Select the block size:** Since each partner is considered a "block", the maximum of each block (here, the best performance per partner) is analyzed.
- **Fit the appropriate EVT model:** Depending on the underlying distribution of the data, one of the three extreme value distributions would be fit. For most real-world data including human-related measurements, which typically do not follow heavy-tailed distributions, the Gumbel distribution is often a suitable model.
  
### Step 3: Estimating Parameters

- **Estimate parameters of the maxima distribution:** Using maximum likelihood estimation or other techniques, the expert would estimate the parameters of the chosen extreme value distribution based on observed maxima.
- **Compute thresholds and probabilities:** Calculate the probability of exceeding the current maximum, which could be modeled as \( P(X > m) = 1 - F(m) \) where \( F \) is the CDF of the fitted extreme value distribution.

### Step 4: Modeling the Waiting Time

- **Geometric distribution for waiting time:** The wait time until a new maximum is observed can be modeled as a geometric distribution, where \( p = P(X > m) \). This probability informs the expected number of new partners required to potentially find a better performance.
- **Calculation of expected time:** The expected waiting time \( E[T] \) would be \( \frac{1}{p} \), where \( p \) is derived from the extreme value model.

### Step 5: Sensitivity Analysis

- **Conduct sensitivity analysis:** Given the uncertainties in human behavior and measurement, a sensitivity analysis on the parameters' estimates and their impact on the probability \( p \) and expected waiting time \( E[T] \) would be essential.
- **Use of simulation:** Simulate different scenarios to understand the variance and distribution of the waiting time under different assumptions about the distribution of performance scores.

### Practical Application and Advice

An expert might conclude that as the number of observed partners increases, the probability of finding an increasingly better performer decreases significantly. This can be presented not just as a theoretical calculation, but integrated with practical advice on relationship standards and expectations, possibly advising that after a certain point, the statistical likelihood of "upgrading" diminishes to a level where other factors should gain prominence in decision-making.

This approach not only gives a statistically sound analysis but also bridges the gap between theory and real-life applications, making the concepts accessible and useful to a broader audience.

>demonstrate explicitly how to incorporate the EVT distribution

To demonstrate explicitly how to incorporate the Extreme Value Theory (EVT) distribution into the analysis of finding a new maximum, let's walk through a detailed example using the Generalized Extreme Value (GEV) distribution, which includes the Gumbel, Fréchet, and Weibull distributions as special cases.

### Step-by-Step Application of EVT

#### Step 1: Selecting the Model
First, let's assume that the sexual performance ratings follow a normal distribution \( X \sim N(\mu, \sigma^2) \), since this is a common assumption for many types of human-related measurements. Based on this, we use the block maxima approach where each maximum from a block (set of observations) is considered.

#### Step 2: Modeling the Maxima
For normally distributed data, the maximum of a sufficiently large sample tends to follow a Gumbel distribution due to the Central Limit Theorem. The Gumbel distribution is particularly appropriate for modeling the maximum of distributions that themselves do not have heavy tails.

**Form of the Gumbel Distribution:**
The cumulative distribution function (CDF) of a Gumbel distribution for maxima is given by:
\[ F(x) = \exp(-\exp(-(x - \mu') / \sigma')) \]
where \( \mu' \) and \( \sigma' \) are location and scale parameters, respectively. These parameters need to be estimated from the data.

#### Step 3: Estimating Parameters
From the sample maxima \( X_{(1)}, X_{(2)}, \ldots, X_{(n)} \):
1. **Estimate \( \mu' \) and \( \sigma' \)** using maximum likelihood estimation (MLE). The estimates are derived from:
   \[ \hat{\mu}' = \bar{x} - \gamma \hat{\sigma}' \]
   \[ \hat{\sigma}' = \frac{s}{\pi\sqrt{6}} \]
   where \( \bar{x} \) is the sample mean of the maxima, \( s \) is the sample standard deviation, and \( \gamma \approx 0.5772 \) is the [[Euler-Mascheroni constant]].

#### Step 4: Calculate the Probability of Exceeding the Current Maximum
Let \( m \) be the current observed maximum. The probability of observing a new maximum greater than \( m \) is:
\[ P(X > m) = 1 - F(m) = 1 - \exp(-\exp(-(m - \hat{\mu}') / \hat{\sigma}')) \]

#### Step 5: Model the Waiting Time
The waiting time \( T \) until a new maximum is observed follows a geometric distribution, where \( p = P(X > m) \). Thus, the probability mass function of \( T \) is:
\[ P(T = k) = p(1 - p)^{k-1} \]
and the expected waiting time is:
\[ E[T] = \frac{1}{p} \]

#### Practical Application
To implement this in a practical setting, you would collect data on performance ratings, calculate the sample maxima for each subset of data (e.g., per partner), fit the Gumbel distribution to these maxima, and then use this model to predict the waiting time until a new maximum is observed.

Here’s an example with hypothetical data:
- Assume \( \mu' = 100 \) and \( \sigma' = 15 \).
- Let \( m = 120 \) be the current maximum.
- Compute \( p \):
  \[ p = 1 - \exp(-\exp(-(120 - 100) / 15)) \approx 0.279 \]
- Compute expected waiting time \( E[T] \):
  \[ E[T] = \frac{1}{0.279} \approx 3.58 \]

Thus, you would expect to need about 3 to 4 new partners to potentially find one with a performance exceeding the current maximum of 120.

### Conclusion
By using the principles of extreme value theory, specifically the Gumbel distribution for maxima, one can rigorously quantify the likelihood of surpassing a known maximum and estimate the expected wait time for such an event. This approach provides a robust statistical framework for analyzing scenarios where the maximum or extreme values are of interest.

