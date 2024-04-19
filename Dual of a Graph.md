see also:
- [[Duality]]

The concept of the **dual of a graph** is a fundamental idea in graph theory, particularly in the context of planar graphs. The dual of a graph depends heavily on its embedding in a plane, suggesting that the relationship between a graph and its dual is rooted in their geometric representations.

### Definition of Dual Graph

For a given planar graph $G$, the dual graph $G^*$ is constructed by placing a vertex in each face of $G$ (including the outer face), and drawing an edge between two vertices in $G^*$ for every edge in $G$ that is shared by the two corresponding faces in $G$. Thus, each edge in the original graph corresponds to exactly one edge in the dual graph, crossing it at a right angle if drawn geometrically.

### Formal Construction

Given a planar graph $G = (V, E)$ embedded in the plane, the dual graph $G^* = (V^*, E^*)$ is constructed as follows:

1. **Vertices of $G^*$**: Each vertex in $G^*$ corresponds to a face in $G$. Therefore, if $G$ has $f$ faces, then $V^*$ will have $f$ vertices.

2. **Edges of $G^*$**: For every edge in $G$ that is an edge of two faces $f_1$ and $f_2$, there is an edge in $G^*$ connecting the vertices corresponding to $f_1$ and $f_2$. If an edge in $G$ is on the boundary of the same face (as can happen with a loop), the corresponding edge in $G^*$ will loop back on the vertex corresponding to that face.

3. **Incidence Relations**: If an edge $e$ in $G$ separates two different faces, $f_1$ and $f_2$, then the corresponding edge $e^*$ in $G^*$ will connect the vertices $v^*_1$ and $v^*_2$ representing $f_1$ and $f_2$, respectively.

### Properties of Dual Graphs

- **Planarity**: If $G$ is planar, then $G^*$ is also planar.
- **Biconnectivity**: If $G$ is connected, then $G^*$ will be connected. Moreover, if $G$ is biconnected (i.e., removing any one vertex does not disconnect the graph), the dual graph $G^*$ will also be biconnected.
- **Face-Vertex Correspondence**: There is a face-vertex correspondence between $G$ and $G^*$ in the sense that the roles of vertices and faces are interchanged.
- **Repeated Dualization**: Dualizing a graph twice, i.e., taking the dual of the dual $(G^*)^*$, generally gives a graph isomorphic to the original graph $G$, especially if we consider graphs embedded in the sphere.

### Examples and Applications

In the realm of [[Topology]] and [[Geometric Graph Theory]], dual graphs play a significant role. For instance, in problems like network design, the concept of dual graphs is used to find complementary properties, such as flows and cuts, via the [[Max-Flow Min-Cut Theorem]], where the cut-set of a network and its flows can be studied through its dual.

Moreover, in polygonal mesh used in computer graphics and finite element methods, the dual of a graph helps in defining relationships between elements (like polygons) that share common edges, which is crucial for mesh refinement and optimization techniques.

In summary, the dual graph is a powerful concept in planar graph theory, providing deep insights not only in mathematics but also in various practical applications where geometrical and topological properties of graphs are essential.

>Duality in nonplanar graphs

Duality in nonplanar graphs, unlike in planar graphs, is not as straightforward because nonplanar graphs do not have a natural embedding in the plane that allows for the easy construction of a dual graph without edge crossings. In planar graphs, the dual is defined with respect to the faces formed by the graph's embedding, but nonplanar graphs lack a direct analog to these "faces" when embedded in a plane, leading to intersections or crossings. 

### Generalizing Duality

To discuss duality for nonplanar graphs, one might need to consider more abstract forms of duality or apply different concepts:

1. **[[Topological Duality]]**: By considering the graph as embedded not in the plane but on other surfaces with higher genus (a measure of a surface's complexity, with the plane having genus 0), one can extend the idea of duality. For example, a graph embedded on a torus (a doughnut-shaped surface) can have a dual graph constructed in a similar manner to the planar case. Here, faces are defined by cycles that cannot be contracted to a point without cutting the surface.

2. **[[Algebraic Duality]]**: Another approach to defining a kind of duality for graphs involves algebraic structures associated with the graph. For example, one can consider the graph's adjacency matrix or its Laplacian matrix and explore dual properties through these algebraic representations. Duality in this sense might involve transformations or operations that correspond to conceptual "duals" of the original graph's properties, such as inverting certain matrix operations or exploring eigenvalue-eigenvector relationships.

3. **[[Matroid Duality]]**: A more abstract generalization of graph duality comes from [[matroid theory]], where a graph can be seen as a special kind of [[matroid]] (a [[Graph Matroid]]). The dual of a graph matroid, known as a co-graph matroid, can be defined for any graph and retains certain dual properties reminiscent of planar graph duality, such as relationships between independent sets and spanning sets.

### Challenges and Concepts

- **Embedding Issues**: Nonplanar graphs can often be embedded on surfaces of higher genus without crossings, but finding such embeddings and corresponding duals can be mathematically intensive and not always intuitive.

- **Graph Minors and Duality**: One could also explore duality through graph minors, a concept deeply studied in graph theory, particularly in the work related to the Graph Minor Theorem by Robertson and Seymour. In this framework, duality might relate to how a graph can or cannot be reduced to simpler forms while preserving certain connectivity or property relationships.

### Computational and Theoretical Implications

In computational graph theory, duality in nonplanar graphs isn't often directly computed due to the complexities and abstract nature of what "duality" might mean outside of the planar context. Instead, focus is generally placed on practical algorithms that deal with specific properties of graphs (like connectivity, flow, coloring) without explicitly constructing a dual graph.

In conclusion, while duality for nonplanar graphs lacks a straightforward geometric interpretation similar to planar graphs, it can be explored through more abstract mathematical frameworks and theories. Each approach to nonplanar graph duality offers different insights and tools, applicable in various areas of mathematics and computer science.