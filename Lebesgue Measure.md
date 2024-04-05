The [[Lebesgue Measure|Lebesgue measure]] plays a foundational role in modern [[analysis]], particularly in the theory of [[Integral|integration]] and [[probability]]. It generalizes the concept of length, area, and volume in a way that accommodates a broader class of [[sets]] than those typically manageable by the traditional [[Riemann integral]]. This [[measure]] was introduced by Henri Lebesgue in the early 20th century to facilitate the integration of functions that are difficult or impossible to integrate in the Riemann sense.

### Definition

The Lebesgue measure, denoted as $\lambda$, is a way of assigning a volume to subsets of $n$-dimensional [[Euclidean space]] $\mathbb{R}^n$. For $n=1$, it represents the length of intervals or unions of intervals; for $n=2$, it represents the area, and for $n=3$, the volume. This measure is defined for a more comprehensive set of objects than those typically measurable by simpler notions of volume.

The formal construction of the Lebesgue measure involves several steps, starting with the concept of outer measure and then restricting this measure to a class of sets called Lebesgue measurable sets.

#### Outer Measure

The Lebesgue outer measure of a set $A \subseteq \mathbb{R}^n$ is defined as the infimum of the sums of the volumes of countable collections of $n$-dimensional rectangles that cover $A$. Mathematically, this can be expressed as:

$$
\lambda^*(A) = \inf\left\{\sum_{k=1}^\infty \text{vol}(R_k) : A \subseteq \bigcup_{k=1}^\infty R_k, \, R_k \text{ are } n\text{-dimensional rectangles}\right\}
$$

where $\text{vol}(R_k)$ denotes the volume of the $k$-th rectangle.

#### [[Lebesgue Measurable]] Sets

A set $A \subseteq \mathbb{R}^n$ is Lebesgue measurable if, for every subset $E \subseteq \mathbb{R}^n$, the following holds:

$$
\lambda^*(E) = \lambda^*(E \cap A) + \lambda^*(E \setminus A)
$$

This condition essentially states that the outer measure of any set can be decomposed into the sum of the outer measures of its intersection with $A$ and the set difference with $A$. The collection of Lebesgue measurable sets is denoted by $\mathcal{M}$.

#### Properties of the Lebesgue Measure

The Lebesgue measure has several key properties that make it suitable for analysis:

- **Translation Invariance**: For any Lebesgue measurable set $A$ and any vector $v \in \mathbb{R}^n$, the set $A+v = \{a+v : a \in A\}$ is measurable, and $\lambda(A+v) = \lambda(A)$.
- **Countable Additivity**: If $\{A_i\}_{i=1}^\infty$ is a countable collection of disjoint Lebesgue measurable sets, then $\lambda(\bigcup_{i=1}^\infty A_i) = \sum_{i=1}^\infty \lambda(A_i)$.
- **Completeness**: Every subset of a set of Lebesgue measure zero is also Lebesgue measurable, and its measure is zero.

### Significance

The Lebesgue measure's ability to measure a wider class of sets than simple geometric shapes allows for the integration of functions that are discontinuous or not nicely behaved over intervals. This flexibility makes the [[Lebesgue Integral|Lebesgue integral]] a more powerful and general tool for analysis, laying the groundwork for modern [[probability theory]], [[functional analysis]], and other areas of mathematics.

---
The concept of [[Lebesgue Measure|Lebesgue measure]] is central to real analysis and serves as a foundation for modern measure theory, providing a way to rigorously define the measure of subsets of $n$-dimensional Euclidean space $\mathbb{R}^n$. Developed by Henri Lebesgue in the early 20th century, it generalizes the notion of the lengths of intervals, areas of surfaces, and volumes of solids in a way that is particularly useful for the integration of functions with respect to this measure, leading to the [[Lebesgue Integral|Lebesgue integral]].

### Definition

The Lebesgue measure, denoted as $\lambda$, is a measure on the $\sigma$-algebra of Lebesgue measurable sets in $\mathbb{R}^n$ that satisfies the following properties:

1. **Non-negativity**: For every Lebesgue measurable set $E \subset \mathbb{R}^n$, $\lambda(E) \geq 0$.
2. **Null empty set**: $\lambda(\emptyset) = 0$.
3. **Countable additivity (or $\sigma$-additivity)**: If $\{E_i\}_{i=1}^{\infty}$ is a countable collection of pairwise disjoint Lebesgue measurable sets, then $\lambda\left(\bigcup_{i=1}^{\infty} E_i\right) = \sum_{i=1}^{\infty} \lambda(E_i)$.
4. **Translation invariance**: For any Lebesgue measurable set $E$ and any vector $v \in \mathbb{R}^n$, $\lambda(E + v) = \lambda(E)$, where $E + v = \{x + v : x \in E\}$.

### Construction

The construction of the Lebesgue measure can be briefly described in several steps:

1. **Defining measure for intervals**: Start by defining the measure of any box (or rectangle) in $\mathbb{R}^n$ as the product of its side lengths. For a box $B = [a_1, b_1] \times [a_2, b_2] \times \cdots \times [a_n, b_n]$, its Lebesgue measure is $\lambda(B) = \prod_{i=1}^{n} (b_i - a_i)$.

2. **[[Outer measure]]**: For any subset $A \subset \mathbb{R}^n$, define its outer measure, $\lambda^*(A)$, as the infimum of the sums of the measures of collections of boxes that cover $A$.

3. **Measurable sets**: A set $E \subset \mathbb{R}^n$ is Lebesgue measurable if for every subset $A \subset \mathbb{R}^n$, $\lambda^*(A) = \lambda^*(A \cap E) + \lambda^*(A \cap E^c)$, where $E^c$ denotes the complement of $E$ in $\mathbb{R}^n$.

4. **Measure of measurable sets**: The Lebesgue measure of a Lebesgue measurable set $E$ is simply $\lambda(E) = \lambda^*(E)$.

### Significance and Applications

The significance of the Lebesgue measure lies in its ability to measure a broader class of sets and integrate a wider class of functions than possible with the classical [[Riemann Integral|Riemann integral]]. This generality makes it invaluable in various fields of mathematics and applied sciences, including probability theory, functional analysis, and mathematical physics.

One of the key applications of the Lebesgue measure is in defining the [[Lebesgue Integral|Lebesgue integral]], which allows for the integration of functions that are not Riemann integrable and provides powerful convergence theorems like the [[Dominated Convergence Theorem]] and the [[Monotone Convergence Theorem]].

### Mathematical Formalisms

The mathematical elegance of Lebesgue's approach lies in its use of outer measures and measurable sets. For a function $f: \mathbb{R}^n \to \mathbb{R}$, the Lebesgue integral $\int f \, d\lambda$ is defined by approximating $f$ from below and above with simple functions (functions that take a finite number of values) whose integrals can be easily computed using the measure of the sets on which these values are taken.

### Conclusion

The [[Lebesgue Measure|Lebesgue measure]] is a cornerstone of modern analysis, offering a robust framework for measuring sets and integrating functions over these sets. Its development not only solved longstanding problems in mathematics but also opened up new avenues for research and application in analysis and beyond.