see also:
- [[Dual of a Graph]]

Graph theory is a fundamental area of mathematics focused on the study of graphs, which are mathematical structures used to model pairwise relations between objects. A graph in this context is made up of vertices (or nodes) and edges (or links) that connect pairs of vertices. This field has rich applications in computer science, biology, social science, transport networks, and many other areas.

### Basic Definitions

- **Graph**: A set of vertices and a set of edges that connect pairs of vertices. Formally, a graph $G$ is an ordered pair $G = (V, E)$ where $V$ is the set of vertices and $E$ is the set of edges, each edge being a set of two vertices.

- **Vertex (Node)**: The fundamental unit by which graphs are defined, typically representing an entity in the graph.

- **Edge (Link)**: A connection between two vertices representing their relationship. Edges can be either directed (indicating a one-way relationship) or undirected (indicating a mutual relationship).

- **Adjacency**: Two vertices are adjacent if there is an edge connecting them. The adjacency relation can be represented in matrix form, known as the adjacency matrix. If $A$ is the adjacency matrix, then $A_{ij} = 1$ if there is an edge from vertex $i$ to vertex $j$, and $A_{ij} = 0$ otherwise.

### Key Concepts

- **Degree**: The degree of a vertex is the number of edges connected to it. For directed graphs, this is further divided into the in-degree (number of incoming edges) and the out-degree (number of outgoing edges).

- **Path**: A sequence of edges which connect a sequence of vertices. A path's length is the number of edges in the path.

- **Cycle**: A path that starts and ends at the same vertex, with all vertices (and edges) being distinct, except the initial and final vertices.

- **Connected Graph**: An undirected graph is connected if there is a path between every pair of vertices. A directed graph is strongly connected if there is a directed path from any vertex to every other vertex.

- **[[Graph Isomorphism]]**: Two graphs $G$ and $H$ are isomorphic if there is a bijection $f: V(G) \to V(H)$ such that any two vertices $u$ and $v$ of $G$ are adjacent in $G$ if and only if $f(u)$ and $f(v)$ are adjacent in $H$.

- **Subgraph**: A graph $H$ is a subgraph of a graph $G$ if $V(H) \subseteq V(G)$ and $E(H) \subseteq E(G)$.

### Advanced Topics

1. **[[Planar Graphs]]**: Graphs that can be drawn on a plane without any edges crossing. The famous [[Four Color Theorem]] states that any planar graph's vertices can be colored with at most four colors such that no two adjacent vertices share the same color.

2. **[[Graph Coloring]]**: Assignment of labels or colors to vertices of a graph subject to certain constraints, the most typical being that no two adjacent vertices can share the same color.

3. **[[Network Flow]]**: Maximizing the flow from a source to a sink in a network. The [[Max-Flow Min-Cut Theorem]] establishes that the maximum amount of flow possible is equal to the capacity of the smallest cut set separating the source and sink.

4. **Graph Algorithms**: Many algorithms exist for solving problems on graphs, such as:
   - [[Dijkstra's Algorithm]] for finding the shortest path in a graph.
   - The [[Ford-Fulkerson Algorithm]] for computing the maximum network flow.
   - [[Breadth-First Search (BFS)]] and [[Depth-First Search (DFS)]] for graph traversal.

Graph theory combines beautifully the abstraction of mathematical structures with the applicability to real-world problems, making it a vibrant and continuously evolving field of study.