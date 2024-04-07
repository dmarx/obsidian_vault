In the context of [[uniform spaces]], an **entourage** is a fundamental concept used to abstractly define the idea of "closeness" without relying on a specific metric. The framework of entourages allows for the generalization of uniform properties such as uniform continuity and uniform convergence, extending these concepts to spaces where a traditional metric structure might not be present or explicitly defined.

### Definition

A uniform space is a set $X$ equipped with a uniform structure, which is defined by a family of subsets of $X \times X$ called entourages, satisfying specific axioms that capture the intuitive idea of elements being close to each other.

An entourage is a subset $U$ of the Cartesian product $X \times X$ such that if $(x, y) \in U$, the elements $x$ and $y$ of $X$ are considered to be "close" according to the criterion established by $U$. The collection of entourages must satisfy the following properties to constitute a uniform structure:

1. **Every entourage contains the diagonal**: For every entourage $U$, the diagonal $\Delta = \{(x, x) | x \in X\}$ is a subset of $U$. This ensures reflexivity, meaning every point is considered close to itself.

2. **Symmetry**: If $(x, y) \in U$, then $(y, x) \in U$ for any entourage $U$. This symmetry property means that closeness is a reciprocal relationship.

3. **Transitivity (via entourage composition)**: For any entourage $U$, there exists another entourage $V$ such that if $(x, y) \in V$ and $(y, z) \in V$, then $(x, z) \in U$. This can be thought of in terms of entourage composition, ensuring that closeness is a transitive property.

### Visualizing Entourages

Imagine $X$ as a set of points, and consider $X \times X$ as a plane with points $(x, y)$ representing pairs of points from $X$. An entourage $U$ can be visualized as a region around the diagonal $\Delta$ of this plane. If a point $(x, y)$ lies within the region defined by $U$, then $x$ and $y$ are considered "close" according to the entourage $U$.

### Applications and Examples

- **Metric Spaces as Uniform Spaces**: In a metric space $(X, d)$, an entourage can be constructed from the metric by defining $U_\epsilon = \{(x, y) | d(x, y) < \epsilon\}$ for any $\epsilon > 0$. The collection of such $U_\epsilon$ for all $\epsilon > 0$ forms a basis for a uniform structure on $X$, aligning with the intuitive metric idea of closeness.

- **Uniform Continuity**: A function $f: X \to Y$ between two uniform spaces is uniformly continuous if for every entourage $V$ in $Y$, there exists an entourage $U$ in $X$ such that $(x, y) \in U$ implies $(f(x), f(y)) \in V$. This abstracts the notion of uniform continuity, which in metric spaces ensures that $f$ preserves the closeness of points uniformly across the domain.

Entourages thus provide a powerful tool for generalizing concepts of analysis to a wide range of spaces, supporting the study of functions and structures in settings that transcend the limitations of metric-based definitions.