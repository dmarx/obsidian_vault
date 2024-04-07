see also:
- [[Decomposition]]

In mathematics and its applications, particularly in [[Algebraic Topology]] and [[topological data analysis]] (TDA), filtrations are a methodical way to study the structure and features of [[topological spaces]], [[graphs]], and data sets by observing how these structures "grow" or change across a series of thresholds or parameters. This approach is especially powerful in understanding complex, high-dimensional, or noisy data.

### Basic Concept of Filtrations

A **filtration** is a nested sequence of spaces or substructures, each contained within the next, typically indexed by a parameter that often represents time or a scale factor. This sequence provides a multi-scale view of the structure being studied, allowing for the examination of its properties and features as they evolve.

Formally, a filtration of a topological space $X$ is a collection of subspaces $\{X_t\}_{t \in T}$, indexed by a totally ordered set $T$ (often the real numbers or a subset thereof), such that for any $s \leq t$ in $T$, we have $X_s \subseteq X_t$. Each $X_t$ is a "snapshot" of the space at the "time" or "scale" $t$, with the containment property ensuring that the snapshots form a coherent evolutionary sequence.

### Filtrations in Algebraic Topology

In algebraic topology, filtrations are used to study the topological properties of spaces in a graded or incremental manner. For example, a filtration of a simplicial complex might start with an empty set and gradually add simplices based on their dimensions or other criteria, revealing the emergence of topological features like connected components, holes, and voids at various scales.

### [[Persistent Homology]] and Filtrations

A significant application of filtrations is in **persistent homology**, a cornerstone technique in TDA. Persistent homology tracks the appearance and persistence of topological features (such as connected components, loops, and voids) across different scales in a filtration. The key output is a **[[persistence diagram]]** or **barcode**, which summarizes the lifespans of these features across the filtration. This information is robust to noise and can capture the "shape" of data in a multi-dimensional space, making it valuable for data analysis.

### Examples and Applications

- **[[Morse Theory]]**: Filtrations can be constructed based on the sublevel sets of a Morse function on a manifold. As the threshold value increases, new topological features of the manifold are exposed.

- **[[Rips Complexes]]**: In TDA, a common approach is to build a filtration of Rips complexes from a point cloud data set. Starting with an empty graph, edges are added between points that are within a certain distance of each other, and this threshold distance increases over time. This process can reveal the underlying topological structure of the data.

- **Software Analysis**: In [[computational topology]], filtrations are used to analyze the structure and behavior of software, identifying patterns and features that evolve over the development process.

Filtrations offer a powerful lens through which to view and analyze the topological and geometric structures inherent in complex data and spaces, providing insights that are not readily apparent at a single scale or dimension. This makes them invaluable tools in both pure mathematics and applied fields like data science, network analysis, and beyond.

>Filtrations can be constructed based on the sublevel sets of a Morse function on a manifold.

The concept of filtrations based on the [[sublevel sets]] of a [[Morse function]] on a manifold intertwines beautifully with Morse theory, offering deep insights into the topology of the manifold. This approach leverages the [[critical points]] of a Morse function to understand the changes in topology as one moves through the manifold. Let's delve into the details of Morse functions, sublevel sets, and their role in creating filtrations that reveal the manifold's topological structure.

### Morse Functions

A **Morse function** is a smooth function $f: M \rightarrow \mathbb{R}$ from a manifold $M$ to the real numbers, satisfying certain conditions at its critical points. Specifically, at each critical point (where the derivative of $f$ vanishes), the Hessian matrix (the matrix of second partial derivatives) of $f$ is non-degenerate (its determinant is non-zero). This ensures that the critical points are isolated and that we can classify them according to their index—the number of negative eigenvalues of the Hessian.

### Sublevel Sets

Given a Morse function $f$ on a manifold $M$, for any real number $a$, the **sublevel set** $f^{-1}((-\infty, a])$ consists of all points in $M$ where the value of $f$ is less than or equal to $a$. As $a$ increases, these sublevel sets form a filtration of the manifold:

$$\emptyset = f^{-1}((-\infty, a_0]) \subseteq f^{-1}((-\infty, a_1]) \subseteq \cdots \subseteq f^{-1}((-\infty, a_n]) = M$$

where $a_0 < a_1 < \cdots < a_n$ and each $a_i$ is chosen to be slightly greater than the $i$-th critical value of $f$. This sequence of sublevel sets provides a way to "scan" through the manifold, observing how its topology changes as we pass through critical values of the Morse function.

### Role in Topology

The key insight of Morse theory is that the topology of these sublevel sets changes only at the critical values of the Morse function, and the nature of this change is determined by the index of the critical point being passed. Specifically:

- **Index 0**: Introducing a new connected component
- **Index 1**: Creating a tunnel or handle
- **Index $n-1$** (in an $n$-dimensional manifold): Adding a void or cavity
- **Index $n$**: Closing off a void or cavity (in a compact manifold)

### Filtrations and Morse Theory

The filtration of sublevel sets based on a Morse function thus encodes significant information about the manifold's topology. By examining the changes in the topology of these sets as we pass through critical values, we can reconstruct the manifold's homotopy type and compute topological invariants like its Betti numbers, which count the number of independent cycles of various dimensions.

### Applications

This methodology has profound implications and applications across mathematics and physics, including:

- **[[Topological Data Analysis]] (TDA)**: Morse theory-inspired techniques are used to analyze high-dimensional data sets by studying the topology of point clouds or sampled spaces.
- **Quantum Field Theory**: The topology of the configuration spaces of physical systems can be studied using Morse theory, with implications for the behavior of the system.
- **Geometry and Topology**: Morse theory provides tools for proving theorems about the topology of manifolds, including the existence of certain types of surfaces or structures within manifolds.

In summary, filtrations constructed from the sublevel sets of a Morse function on a manifold offer a powerful approach to understanding the manifold's topology, illustrating the interplay between differential geometry, algebraic topology, and computational methods in modern mathematics.