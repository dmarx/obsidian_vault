see also:
- [[Invariants]]
- [[Bifurcations]]
- [[Bifurcation Theory]]

Whitney stratifications are a fundamental concept in [[differential topology]] and [[singularity theory]], introduced by [[Hassler Whitney]] in the 1960s. They provide a systematic way to decompose a space, often a [[singular space]], into [[manifolds]] of varying dimensions, called [[strata]], that fit together in a regular way. This [[decomposition]] allows mathematicians to extend the tools and intuitions of [[smooth manifold theory]] to more general spaces, including those with [[singularities]].

### Definition and Key Properties

A **Whitney stratification** of a [[topological space]] $X$ is a partition of $X$ into a locally finite collection of disjoint, connected, smooth manifolds (called **strata**) that satisfy certain regularity conditions (Whitney's conditions A and B) to ensure a controlled behavior of strata near each other.

- **[[Strata]]**: Each piece in the decomposition, or stratum, is a smooth manifold that can vary in dimension. The strata are subject to certain conditions that prevent "bad" interactions between different strata.

- **Whitney's Condition A**: If a sequence of points $x_i$ in a stratum $S$ converges to a point in a lower-dimensional stratum $S'$, and if the [[tangent space|tangent planes]] to $S$ at $x_i$ converge, then the limiting tangent plane contains the tangent plane to $S'$ at the limit point.

- **Whitney's Condition B**: Given two sequences of points $x_i$ in $S$ and $y_i$ in $S'$ converging to the same point in $S'$, if the secant lines (lines connecting $x_i$ to $y_i$) converge to a limiting line and the tangent planes to $S$ at $x_i$ also converge, then the limiting line lies in the limiting tangent plane.

### Importance of Whitney Stratifications

Whitney stratifications allow mathematicians and scientists to:

- **Understand [[Singular Spaces]]**: They provide a framework for analyzing spaces with [[singularities]], such as [[Algebraic Varieties]], by decomposing them into simpler, well-understood pieces.

- **Extend Differential Topology Tools**: Tools from [[differential topology]] and [[differential geometry|geometry]] can be applied to each stratum of a Whitney stratified space, enabling the study of spaces that are not smooth manifolds in their entirety.

- **Analyze [[Dynamical Systems]]**: In dynamical systems, Whitney stratifications can be used to study the behavior near singularities and [[invariant sets]], such as [[attractors]] or [[repellers]].

### Applications

Whitney stratifications have found applications across several areas of mathematics and related fields:

- **[[Algebraic Geometry]]**: In the study of algebraic varieties, stratifications help in understanding the local and global structure of varieties, including their singular and nonsingular parts.

- **[[Singularity Theory]]**: Stratifications are crucial in the analysis of singular points of mappings, offering a way to classify and study different types of singularities.

- **Dynamical Systems and Physics**: They are used to analyze the [[phase space]] of dynamical systems, especially in understanding the structure of [[chaotic attractors]] and the bifurcation of invariant sets.

- **[[Optimization]] and Data Analysis**: Stratifications have been applied to optimization problems and data analysis, where the geometry of the problem or the data set may naturally lead to a stratified structure.

### Mathematical Challenges and Developments

The theory of Whitney stratifications involves deep mathematical concepts from differential geometry, algebraic geometry, and topology. One of the challenges is to construct a Whitney stratification for a given singular space, a task that can be highly nontrivial depending on the complexity of the space. Recent developments continue to explore the connections between Whitney stratifications and other areas, such as [[Tropical Geometry]] and [[symplectic topology]], broadening the applicability and understanding of these stratifications in mathematics.