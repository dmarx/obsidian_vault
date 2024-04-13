see also:
- [[Curvature]]
- [[Network Science]]
- [[Riemannian Geometry]]
- [[Topology]]

>network graph analog of "local curvature" measures

In network science, the concept of "local curvature" draws inspiration from differential geometry, where curvature quantifies how much a curve deviates from being a straight line (in 2D) or a plane (in 3D). While networks (graphs) do not inhabit continuous spaces and thus do not have curvature in the traditional geometric sense, several analogs have been developed to capture similar notions of curvature within the discrete structure of graphs. These measures aim to describe the local and global shape of the network, offering insights into its topology, robustness, and dynamics. Among the most notable analogs of curvature in network graphs are the Ollivier-Ricci curvature and the Forman-Ricci curvature.

### Ollivier-Ricci Curvature

The [[Ollivier-Ricci curvature]], inspired by Ricci curvature from Riemannian geometry, has been adapted for discrete networks. It measures how the distribution of mass (or probability) around a node diverges from that of another node, with the divergence conceptualized in terms of optimal transport cost between the distributions surrounding these nodes.

- **Intuition:** In a graph, a positive Ollivier-Ricci curvature between two nodes suggests that the nodes are part of a tightly-knit community (similar to being part of a sphere in geometric space), whereas a negative curvature indicates that the nodes are in a more dispersed or tree-like structure (analogous to a saddle shape in geometry).
- **Calculation:** For nodes \(x\) and \(y\) in a graph, the Ollivier-Ricci curvature is calculated based on the Wasserstein distance (a type of optimal transport distance) between probability distributions defined on the neighborhoods of \(x\) and \(y\).

### Forman-Ricci Curvature

[[Forman-Ricci curvature]], proposed by Robin Forman as an adaptation of [[Ricci curvature]] for cell complexes, including networks, provides a more combinatorial and computationally tractable approach to curvature in graphs. It is defined directly in terms of the graph’s structure (edges and nodes) without resorting to optimal transport.

- **Intuition:** The Forman-Ricci curvature for an edge in a network captures the connectivity and clustering properties around that edge, with higher curvature values indicating stronger clustering or tighter community structure.
- **Calculation:** The Forman-Ricci curvature of an edge depends on the degrees of the nodes it connects and the number of triangles (3-cycles) that the edge participates in. The specific formula adjusts these components to estimate how much an edge contributes to the network's overall "curvedness."

### Applications and Implications

- **Network Analysis:** Curvature measures can help identify critical edges and nodes that play significant roles in the network’s structure and function, such as bridges between communities (which may correspond to edges of particularly low curvature) or highly central nodes within communities (associated with high curvature).
- **Robustness and Resilience:** Networks with predominantly positive curvature may exhibit greater robustness to failures and attacks, as positive curvature indicates strong inter-node connectivity, facilitating alternative paths for network flow.
- **Navigation and Routing:** Curvature can inform strategies for efficient navigation and routing within networks, with curvature patterns highlighting optimal paths that balance short distances and high connectivity.

### Challenges

- **Interpretation:** While curvature analogs provide valuable insights into network structure, interpreting these measures in the context of specific applications requires careful consideration of the network's topology and the dynamics of processes running on the network.
- **Computation:** Especially for large networks, calculating curvature measures like the Ollivier-Ricci curvature can be computationally intensive, though recent advances have aimed at developing more efficient algorithms and approximations.

The adaptation of curvature measures to network graphs represents a fascinating intersection of geometry and network science, offering novel tools for understanding the complex structures and behaviors of networks across diverse domains.