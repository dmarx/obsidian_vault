A normed vector space is a central concept in functional analysis, linear algebra, and related fields, blending geometric intuition with algebraic operations. It extends the idea of vector spaces by introducing a way to measure vector lengths and distances between vectors, thereby adding a topological structure to the vector space.

### Definition

A **normed vector space** is a pair $(V, \|\cdot\|)$ where $V$ is a vector space over a field $\mathbb{F}$ (usually $\mathbb{R}$ or $\mathbb{C})$, and $\|\cdot\|$ is a norm on $V$. The norm is a function $\|\cdot\|: V \rightarrow \mathbb{R}$ that assigns a non-negative length or size to each vector in $V$, satisfying the following properties for all vectors $x, y \in V$ and all scalars $a \in \mathbb{F}$:

1. **Non-negativity:** $\|x\| \geq 0$ with $\|x\| = 0$ if and only if $x = 0$.
2. **Scalar Multiplication:** $\|ax\| = |a|\|x\|$ for any scalar $a$.
3. **Triangle Inequality:** $\|x + y\| \leq \|x\| + \|y\|$.

### Examples

- **Euclidean Space ($\mathbb{R}^n$ or $\mathbb{C}^n$)**: The norm defined by $\|x\| = \sqrt{x_1^2 + x_2^2 + \ldots + x_n^2}$ for a vector $x = (x_1, x_2, \ldots, x_n)$ is known as the Euclidean norm, making \(\mathbb{R}^n\) or \(\mathbb{C}^n\) a normed vector space.

- **\(p\)-norms**: Given $1 \leq p < \infty$, the \(p\)-norm (or $L^p$ norm) on $\mathbb{R}^n$ is defined as $\|x\|_p = (|x_1|^p + |x_2|^p + \ldots + |x_n|^p)^{1/p}$. For \(p = \infty\), the norm is defined as $\|x\|_\infty = \max\{|x_1|, |x_2|, \ldots, |x_n|\}$, which is the maximum norm.

- **Function Spaces**: Spaces of continuous, differentiable, or integrable functions can be equipped with norms that measure the size of functions in various ways, such as the maximum absolute value of a function over a domain or the integral of the absolute value of a function.

### Distance in Normed Vector Spaces

In a normed vector space, the distance \(d(x, y)\) between two vectors \(x\) and \(y\) is naturally defined by the norm of their difference: \(d(x, y) = \|x - y\|\). This makes every normed vector space into a metric space, allowing the application of metric space concepts like convergence, continuity, and compactness within the context of vector spaces.

### Importance

Normed vector spaces are crucial in many areas of mathematics and applied sciences. They provide a framework for analyzing and understanding the behavior of vectors and functions, particularly in infinite-dimensional spaces. These spaces form the basis for more complex structures in functional analysis, such as [[Banach Spaces]] (complete normed vector spaces) and [[Hilbert spaces]] (complete normed vector spaces with an inner product inducing the norm), which are essential in the study of differential equations, quantum mechanics, and many areas of pure and applied mathematics.