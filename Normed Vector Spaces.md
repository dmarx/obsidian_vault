---
tags:
  - sod/green
  - needs-outlinks
---
see also:
- [[L-p Spaces]]

A normed vector space is a central concept in functional analysis, linear algebra, and related fields, blending geometric intuition with algebraic operations. It extends the idea of vector spaces by introducing a way to measure vector lengths and distances between vectors, thereby adding a topological structure to the vector space.

### Definition

A **normed vector space** is a pair $(V, \|\cdot\|)$ where $V$ is a vector space over a field $\mathbb{F}$ (usually $\mathbb{R}$ or $\mathbb{C})$, and $\|\cdot\|$ is a norm on $V$. The norm is a function $\|\cdot\|: V \rightarrow \mathbb{R}$ that assigns a non-negative length or size to each vector in $V$, satisfying the following properties for all vectors $x, y \in V$ and all scalars $a \in \mathbb{F}$:

1. **Non-negativity:** $\|x\| \geq 0$ with $\|x\| = 0$ if and only if $x = 0$.
2. **Scalar Multiplication:** $\|ax\| = |a|\|x\|$ for any scalar $a$.
3. **Triangle Inequality:** $\|x + y\| \leq \|x\| + \|y\|$.

### Examples

- **Euclidean Space ($\mathbb{R}^n$ or $\mathbb{C}^n$)**: The norm defined by $\|x\| = \sqrt{x_1^2 + x_2^2 + \ldots + x_n^2}$ for a vector $x = (x_1, x_2, \ldots, x_n)$ is known as the Euclidean norm, making \(\mathbb{R}^n\) or \(\mathbb{C}^n\) a normed vector space.

- **\(p\)-norms**: Given $1 \leq p < \infty$, the \(p\)-norm (or $L^p$ norm) on $\mathbb{R}^n$ is defined as $\|x\|_p = (|x_1|^p + |x_2|^p + \ldots + |x_n|^p)^{1/p}$. For \(p = \infty\), the norm is defined as $\|x\|_\infty = \max\{|x_1|, |x_2|, \ldots, |x_n|\}$, which is the maximum norm.

- **[[Function Spaces]]**: Spaces of continuous, differentiable, or integrable functions can be equipped with norms that measure the size of functions in various ways, such as the maximum absolute value of a function over a domain or the integral of the absolute value of a function.

### Distance in Normed Vector Spaces

In a normed vector space, the distance \(d(x, y)\) between two vectors \(x\) and \(y\) is naturally defined by the norm of their difference: \(d(x, y) = \|x - y\|\). This makes every normed vector space into a metric space, allowing the application of metric space concepts like convergence, continuity, and compactness within the context of vector spaces.

### Importance

Normed vector spaces are crucial in many areas of mathematics and applied sciences. They provide a framework for analyzing and understanding the behavior of vectors and functions, particularly in infinite-dimensional spaces. These spaces form the basis for more complex structures in functional analysis, such as [[Banach Space]] (complete normed vector spaces) and [[Hilbert Space]] (complete normed vector spaces with an inner product inducing the norm), which are essential in the study of [[differential equations]], quantum mechanics, and many areas of pure and applied mathematics.

---

> norm

In mathematics, a **norm** is a function that assigns a strictly positive length or size to all vectors in a vector space—except for the zero vector, which is assigned a length of zero. Norms are essential in various areas of mathematics, including linear algebra, analysis, and applied mathematics, because they provide a way to quantify the size or distance in a vector space. 

### Definition

Formally, a norm on a vector space $V$ over a field $\mathbb{F}$ (commonly $\mathbb{R}$ or $\mathbb{C}$) is a function $\|\cdot\|: V \rightarrow \mathbb{R}$ satisfying the following properties for all vectors $u, v \in V$ and all scalars $\alpha \in \mathbb{F}$:

1. **Non-negativity**: $\|v\| \geq 0$ with equality if and only if $v = 0$.
2. **Scalar Multiplication**: $\|\alpha v\| = |\alpha| \|v\|$, where $|\alpha|$ is the absolute value of $\alpha$.
3. **Triangle Inequality**: $\|u + v\| \leq \|u\| + \|v\|$. This states that the norm of the sum of two vectors is less than or equal to the sum of their norms.
4. **Definiteness**: $\|v\| = 0$ if and only if $v = 0$.

### Common Examples of Norms

- **Euclidean Norm (or 2-norm)**: On $\mathbb{R}^n$, the Euclidean norm is defined as $\|x\|_2 = \sqrt{x_1^2 + x_2^2 + \cdots + x_n^2}$, where $x = (x_1, x_2, ..., x_n)$. This norm corresponds to the usual geometric length of a vector in $n$-dimensional space.

- **$p$-norm**: More generally, for $1 \leq p < \infty$, the $p$-norm (or Lp norm) is given by $\|x\|_p = (|x_1|^p + |x_2|^p + \cdots + |x_n|^p)^{\frac{1}{p}}$. The Euclidean norm is a special case where $p=2$. The case $p=1$ yields the **Manhattan Norm**, and as $p$ approaches infinity, the $p$-norm converges to the **Infinity Norm** ($\|x\|_\infty$), which is equal to $\max\{|x_1|, |x_2|, ..., |x_n|\}$.

- **Infinity Norm (or max norm)**: This norm measures the size of a vector as the maximum absolute value of its components: $\|x\|_\infty = \max_{i} |x_i|$.

### Properties and Applications

- **Metric**: A norm induces a metric (distance function) $d(u, v) = \|u - v\|$ on the vector space, which measures the distance between any two vectors $u$ and $v$.

- **Unit Sphere**: The set of all vectors with norm equal to one forms the unit sphere in the normed vector space. The shape of this sphere can vary significantly depending on the chosen norm.

- **Topological Structure**: Norms give a vector space a topological structure, allowing for the definition and analysis of concepts like convergence, continuity, and compactness within the space.

- **Applications**: Norms are widely used in numerical analysis to estimate errors, in functional analysis to study function spaces, and in optimization problems where one seeks to minimize or maximize some norm-related quantity.

In summary, norms are central to the structure of vector spaces and the study of linear algebra, providing a powerful way to quantify and compare elements within these spaces. Their versatility and utility extend across pure and applied mathematics, making them indispensable tools in both theoretical and practical contexts.

>Norms give a vector space a topological structure

Indeed, norms endow a vector space with a topological structure, which enables the study of continuous functions, convergence of sequences, and compactness, among other concepts, within the space. This [[Topology On A Set|topological structure]] is derived from the [[Metric Space|metric]] induced by the norm, which defines a notion of distance between vectors.

### How Norms Induce a Topology

Given a normed vector space $(V, \|\cdot\|)$ over a field $\mathbb{F}$ (typically $\mathbb{R}$ or $\mathbb{C}$), the norm $\|\cdot\|$ induces a metric (distance function) $d: V \times V \rightarrow \mathbb{R}$ defined by $d(u, v) = \|u - v\|$ for all $u, v \in V$. This metric satisfies the properties of a distance function:

1. **Non-negativity**: $d(u, v) \geq 0$ for all $u, v \in V$, with $d(u, v) = 0$ if and only if $u = v$.
2. **Symmetry**: $d(u, v) = d(v, u)$ for all $u, v \in V$.
3. **Triangle Inequality**: $d(u, w) \leq d(u, v) + d(v, w)$ for all $u, v, w \in V$.

The metric $d$ allows for the definition of open balls, which are the basic building blocks of the topology on $V$. An open ball centered at a vector $v \in V$ with radius $r > 0$ is the set $B(v, r) = \{u \in V : \|u - v\| < r\}$. These open balls generate a topology on $V$, where a set $U \subseteq V$ is defined to be open if for every $v \in U$, there exists some $r > 0$ such that $B(v, r) \subseteq U$. This collection of open sets satisfies the axioms of a topology:

- The empty set and the whole space $V$ are open.
- The intersection of any finite collection of open sets is open.
- The union of any collection of open sets is open.

### Implications of the Topological Structure

1. **Convergence**: A sequence $(v_n)$ in $V$ converges to a limit $v \in V$ if, for every $\epsilon > 0$, there exists an $N \in \mathbb{N}$ such that $\|v_n - v\| < \epsilon$ for all $n \geq N$. This is equivalent to saying that the sequence gets arbitrarily close to the limit in terms of the norm-induced distance.

2. **Continuity**: A function $f: V \rightarrow W$ between two normed vector spaces is continuous if the preimage of every open set in $W$ is open in $V$. In terms of the norm, $f$ is continuous at $v \in V$ if, for every $\epsilon > 0$, there exists a $\delta > 0$ such that $\|u - v\| < \delta$ implies $\|f(u) - f(v)\| < \epsilon$ for all $u \in V$.

3. **Compactness**: A set $S \subseteq V$ is compact if every open cover of $S$ has a finite subcover. In infinite-dimensional normed vector spaces, compact sets have properties significantly different from those in finite-dimensional spaces, reflecting the complexity of the topology induced by the norm.

By equipping vector spaces with a norm, one not only quantifies the "size" or "length" of vectors but also introduces a rich topological structure that allows for the exploration of continuous transformations, limits, and other fundamental concepts in analysis.