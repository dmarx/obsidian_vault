A **simplicial complex** is a fundamental concept in [[Algebraic Topology]] and [[combinatorial topology]], serving as a crucial tool for studying the structure and properties of [[topological spaces]]. Simplicial complexes are made up of simplices, which are generalizations of geometric shapes such as points (0-simplices), line segments (1-simplices), triangles (2-simplices), and tetrahedra (3-simplices) to higher dimensions.

### Definition of a Simplex

A **[[Simplex]]** is the convex hull of a finite set of points in a Euclidean space that do not all lie in the same hyperplane. Formally, an $n$-dimensional simplex (or $n$-simplex) can be defined as the convex hull of $n + 1$ affinely independent points. These points are called the vertices of the simplex.

### Construction of Simplicial Complexes

A **simplicial complex** $K$ is a set of simplices that satisfies the following conditions:

1. **Faces of Simplices**: Every face of a simplex in $K$ is also in $K$. A face of a simplex is any simplex formed by a subset of the vertices of the original simplex. For example, the faces of a 2-simplex (triangle) include its edges (1-simplices) and vertices (0-simplices).

2. **Intersection Property**: The intersection of any two simplices in $K$ is either empty or a face of both simplices. This condition ensures that simplices are glued together along common faces in a well-defined manner.

### Examples

- A single point is a 0-dimensional simplicial complex.
- A graph (in the sense of discrete mathematics) can be viewed as a 1-dimensional simplicial complex, where the vertices are 0-simplices and the edges are 1-simplices.
- A solid tetrahedron, including its interior, is not a simplicial complex by itself because it includes a "filling" that cannot be expressed as a union of simplices. However, its boundary, consisting of four triangular faces, six edges, and four vertices, does form a simplicial complex.

### Applications

**Simplicial complexes** are used in various mathematical and computational fields:

- **Topology and Algebraic Topology**: Simplicial complexes provide a combinatorial way to study topological spaces, facilitating the computation of topological invariants such as homology and cohomology groups.

- **[[Computational Geometry]] and Topology**: They are essential in algorithms for mesh generation, [[manifold learning]], and the analysis of high-dimensional data sets.

- **[[Persistent Homology]]**: In topological data analysis, simplicial complexes are used to construct [[Filtrations]] that capture the shape of data at multiple scales, allowing for the computation of persistent homology.

### Homotopy Type Theory and Simplicial Complexes

Within the framework of [[Homotopy Type Theory]] (HoTT), simplicial complexes can provide intuition and models for understanding types and homotopies. While HoTT deals with spaces and paths in a more abstract, type-theoretic manner, the concrete geometric realization of spaces as simplicial complexes can illuminate concepts like homotopy equivalence and higher-dimensional types, including [[Higher Inductive Types]] (HITs), which extend the idea of simplicial complexes into the realm of type theory by allowing for the construction of types with higher-dimensional paths.