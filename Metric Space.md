A [[Topological Space]] imbued with a metric, i.e. some notion of "distance"

See also:
- [[Measure]]

A metric space is a fundamental concept in mathematics, particularly in the fields of geometry, analysis, and topology. It provides a formal framework for quantifying the notion of distance between elements of a set.

### Definition

A **metric space** \((M, d)\) consists of a set \(M\) along with a metric \(d\), which is a function that defines a distance between any two elements in \(M\). The metric \(d: M \times M \rightarrow \mathbb{R}\) must satisfy the following properties for all \(x, y, z \in M\):

1. **Non-negativity:** \(d(x, y) \geq 0\) and \(d(x, y) = 0\) if and only if \(x = y\).
2. **Symmetry:** \(d(x, y) = d(y, x)\).
3. **Triangle Inequality:** \(d(x, z) \leq d(x, y) + d(y, z)\).

### Examples of Metric Spaces

- **Euclidean Space:** The set of all points in \(n\)-dimensional space (\(\mathbb{R}^n\)) with the distance function \(d(x, y) = \sqrt{\sum_{i=1}^{n}(x_i - y_i)^2}\) is a classic example of a metric space.
- **Discrete Metric:** On any set \(M\), the discrete metric \(d(x, y) = 1\) if \(x \neq y\) and \(0\) otherwise, turns \(M\) into a metric space.
- **Manhattan Distance:** In \(\mathbb{R}^2\), the function \(d(x, y) = |x_1 - y_1| + |x_2 - y_2|\) defines a metric space, where distance is measured along axes at right angles.

### Importance and Applications

Metric spaces are crucial in various branches of mathematics:

- **Topology:** The concept of a metric induces a topology on a set, allowing the study of continuity, compactness, and convergence within the space.
- **Analysis:** Metric spaces provide a setting for generalizing and extending many fundamental concepts in analysis, such as limits, continuity, and compactness.
- **Geometry:** Metric spaces generalize the idea of geometric space, including not just Euclidean spaces but also more complex structures like curved spaces.
- **Computer Science and Data Science:** Metrics are used in algorithms for searching, clustering, and classification where distances between data points are crucial.

### Generalizations

Several mathematical structures generalize metric spaces by relaxing some of the metric properties or by adding more structure:

- **Pseudometric Spaces:** Where \(d(x, y) = 0\) does not necessarily imply \(x = y\), allowing for different points to be "zero distance" apart.
- **[[Normed Vector Spaces]]:** Where the distance function is derived from a norm, adding algebraic structure to the space.
- **Riemannian Manifolds:** Which generalize metric spaces to smoothly varying metrics, allowing for the study of curved spaces in differential geometry.

In essence, metric spaces are a foundational concept in mathematics, providing the tools to rigorously define and work with distances, and serve as a cornerstone for many theoretical and applied disciplines.