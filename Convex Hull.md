The **convex hull** of a set of points in a [[Euclidean space]] $\mathbb{R}^d$ is a fundamental concept in computational geometry, [[optimization]], and many areas of mathematics. It is the smallest convex set that contains all the points in the given set.

### Definition
Given a set of points $X \subseteq \mathbb{R}^d$, the convex hull of $X$, denoted as $\text{conv}(X)$, is defined as the set of all convex combinations of points from $X$. Mathematically, it can be expressed as:
$$
\text{conv}(X) = \left\{ \sum_{i=1}^k \lambda_i x_i \mid x_i \in X, \lambda_i \geq 0, \sum_{i=1}^k \lambda_i = 1, k \in \mathbb{N} \right\}
$$
Here, each $\lambda_i$ represents a weight assigned to the point $x_i$, where all weights are non-negative and sum to 1.

### Properties
1. **[[Convexity]]**: By definition, the convex hull is a convex set.
2. **[[Compactness]]**: If $X$ is a compact set, then $\text{conv}(X)$ is also compact.
3. **Inclusion**: For any set $X \subseteq \mathbb{R}^d$, $\text{conv}(X)$ is the smallest convex set that contains $X$.

### Computation
The computation of the convex hull is a central problem in computational geometry. Several algorithms exist for this purpose, with their efficiency depending on the dimension $d$ and the number of points $n$. Common algorithms include:

- **Graham's scan** and **Andrew's monotone chain algorithm**: These are used for computing the convex hull in $\mathbb{R}^2$ and are based on sorting the points and then constructing the hull.
- **Quickhull**: A method similar in concept to QuickSort and used in various dimensions, known for its average-case efficiency.
- **Incremental algorithms**: These build the hull by adding one point at a time and are useful in higher dimensions.

### Visual Example
In $\mathbb{R}^2$, if you consider a set of points, the convex hull can be visualized as the shape of a rubber band stretched around the outermost points. This shape includes all the given points and is convex.

### Applications
The convex hull has applications in numerous fields:
- **Pattern Recognition**: Defining the boundaries of object clusters.
- **Computer Graphics**: Collision detection and shape analysis.
- **Robotics**: Workspace determination and obstacle avoidance.
- **Geographic Information Systems (GIS)**: Defining boundaries around geographical features.

### Further Exploration
The study of convex hulls is connected to several other mathematical topics and algorithms, such as [[Caratheodory's Theorem|Carathéodory's theorem]] and [[Delaunay Triangulation]]. Understanding convex hulls can provide insights into the structure and behavior of complex systems and forms a foundation for advanced studies in discrete and computational geometry.