The Lebesgue integral, developed by [[Henri Lebesgue]] in the early 20th century, extends the concept of integration beyond the limitations of the [[Riemann Integral]]. It plays a crucial role in modern analysis, particularly in measure theory, functional analysis, and probability theory. The Lebesgue integral is more general and flexible than the Riemann integral, allowing for the integration of a broader class of functions, including those with an infinite number of discontinuities.

### Preliminaries: [[Measure Theory]]

The foundation of the Lebesgue integral is measure theory. A measure on a set is a systematic way to assign a number to each suitable subset of that set, intuitively interpreted as its size. In the context of the Lebesgue integral, the most commonly used measure is the Lebesgue measure on the real line, which generalizes the concept of length of intervals to more complex sets.

### Definition of the Lebesgue Integral

1. **Measurable Functions:** A function $f: \mathbb{R} \rightarrow \mathbb{R}$ is said to be measurable if, for every real number $\alpha$, the set $\{x \in \mathbb{R} : f(x) > \alpha\}$ is measurable (i.e., its size or measure can be determined).

2. **Simple Functions:** A simple function is a finite linear combination of characteristic functions of measurable sets. The Lebesgue integral of a simple function that takes on a finite number of values $\{a_1, a_2, \ldots, a_n\}$ on measurable sets $\{E_1, E_2, \ldots, E_n\}$ is defined as $$\int \sum_{i=1}^n a_i \chi_{E_i} = \sum_{i=1}^n a_i m(E_i)$$ where $m(E_i)$ is the measure of the set $E_i$, and $\chi_{E_i}$ is the characteristic function of $E_i$.

3. **General Lebesgue Integral:** For a non-negative measurable function $f$, the Lebesgue integral of $f$ over a measurable set $E$ is defined as the supremum of the integrals of all simple functions that are less than or equal to $f$ on $E$. For functions that take on both positive and negative values, the integral is defined as the difference of the integrals of its positive and negative parts, provided at least one of those integrals is finite.

### Key Properties and Theorems

- **[[Monotonicity|Monotone]] Convergence Theorem:** If $\{f_n\}$ is a sequence of measurable functions that increase monotonically pointwise to a measurable function $f$, then the integral of $f_n$ converges to the integral of $f$.

- **[[Dominated Convergence Theorem]]:** If $\{f_n\}$ is a sequence of measurable functions that converges almost everywhere to a function $f$, and there exists an integrable function $g$ such that $|f_n| \leq g$ for all $n$, then $f$ is integrable, and the integral of $f_n$ converges to the integral of $f$.

- **[[Fatou's Lemma]]:** For any sequence of non-negative measurable functions $\{f_n\}$, the integral of the pointwise limit infimum of $f_n$ is less than or equal to the limit infimum of the integrals of $f_n$.

### Advantages Over Riemann Integral

The Lebesgue integral's major advantage is its ability to integrate a wider range of functions, especially those that are problematic for the Riemann integral due to discontinuities or other irregularities. Its framework also facilitates the development of advanced mathematical concepts and techniques, particularly in the analysis of functions and their properties.

Furthermore, the Lebesgue integral's properties, especially the [[Dominated Convergence Theorem]], provide powerful tools for exchanging limits and integrals, which is essential in many areas of analysis and applied mathematics. This makes the Lebesgue integral a fundamental concept in modern mathematics, underpinning many theoretical and applied areas of research.