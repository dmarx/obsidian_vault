---
tags:
  - needs-outlinks
---
see also:
- [[statistics]]
- [[Random Variables]]

Statistical moments are quantitative measures that capture various aspects of the shape and characteristics of a probability distribution. They are fundamental in the fields of statistics and probability, providing insights into the distribution's location, scale, skewness, and kurtosis, among other features. Each moment corresponds to a particular derivative of a generating function, such as the moment-generating function or the cumulant-generating function.

Here's a detailed breakdown of the first few moments and their significance:

### 1. First Moment: Mean
The first moment about the origin provides the mean ($\mu$) of the distribution, which is a measure of central tendency. It is defined as:
$$\mu = E[X] = \int_{-\infty}^\infty x f(x) \, dx$$
for a continuous variable $X$ with density $f(x)$, or
$$\mu = E[X] = \sum_{i} x_i p_i$$
for a discrete variable, where $x_i$ are the values and $p_i$ their respective probabilities.

### 2. Second Moment: [[Variance]]
The second moment about the mean provides the variance ($\sigma^2$), which measures the dispersion of the distribution around its mean. It is computed as:
$$\sigma^2 = E[(X - \mu)^2] = \int_{-\infty}^\infty (x - \mu)^2 f(x) \, dx$$
for continuous variables, or
$$\sigma^2 = E[(X - \mu)^2] = \sum_{i} (x_i - \mu)^2 p_i$$
for discrete variables.

### 3. Third Moment: Skewness
The third central moment is used to calculate the skewness of the distribution, which measures the asymmetry of the distribution around its mean. Skewness is normalized by the standard deviation to the third power, thus:
$$\text{Skewness} = \frac{E[(X - \mu)^3]}{\sigma^3}$$
A positive skew indicates a distribution with an extended tail to the right, while a negative skew indicates a tail to the left.

### 4. Fourth Moment: Kurtosis
The fourth central moment is used to define the kurtosis, which measures the "tailedness" of the distribution. Kurtosis is often normalized by the square of the variance (standard deviation squared), giving:
$$\text{Kurtosis} = \frac{E[(X - \mu)^4]}{\sigma^4}$$
A higher kurtosis than that of a normal distribution (which has a kurtosis of 3) indicates a distribution with heavier tails and a sharper peak, termed leptokurtic.

### Higher Moments
Higher moments ($n^{th}$ moments) about the mean can be similarly defined and are used to describe additional aspects of the distribution's shape:
$$E[(X - \mu)^n]$$
They become progressively more complex and harder to interpret but can be crucial in certain statistical models, particularly in finance and signal processing.

Statistical moments are not only foundational in descriptive statistics but also serve as the building blocks for various forms of [[statistical inference]], helping to characterize distributions for hypothesis testing, model fitting, and more. For deeper statistical analysis, exploring the relationships between moments and other distribution characteristics or leveraging them in the form of [[Cumulants]] and [[moment generating functions]] can provide further insights.