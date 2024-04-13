
see also:
- [[Graph Laplacian]]
- [[Spectral Theory of Graphs]]

>This partitioning tends to minimize the number of edges between the two clusters why

The [[Graph Partitioning|partitioning]] obtained from the Fiedler vector, corresponding to the second smallest eigenvalue of the Laplacian matrix, tends to minimize the number of edges between the two clusters due to the inherent properties of the [[Laplacian matrix]] and its relation to the [[graph cut]]. This result stems from the specific characteristics of the Laplacian matrix and the properties of its eigenvectors and eigenvalues. Here’s a more detailed breakdown:

### The Laplacian Matrix and the Fiedler Vector

The Laplacian matrix \(L = D - A\) captures the difference between the degree matrix \(D\) and the adjacency matrix \(A\). In the context of [[graph theory]]:
- \(L_{ii} = \) degree of vertex \(i\).
- \(L_{ij} = -1\) if vertex \(i\) and vertex \(j\) are adjacent.
- \(L_{ij} = 0\) if vertex \(i\) and vertex \(j\) are not adjacent.

The key property of the Laplacian matrix is that for any vector \(x\),
$$
x^T L x = \sum_{i < j} A_{ij} (x_i - x_j)^2 = \frac{1}{2} \sum_{i, j} A_{ij} (x_i - x_j)^2,
$$
where \(x_i\) and \(x_j\) are the components of \(x\). This expression quantifies the total "discrepancy" across edges weighted by the entries of \(x\).

### The Fiedler Vector and Graph Partitioning

The Fiedler vector, which corresponds to the second smallest eigenvalue (or the first non-zero eigenvalue) of \(L\), inherently carries information about the minimal discrepancy or "cut" across the graph:
- **Cut Minimization**: When partitioning a graph into two clusters based on the sign of the elements of the Fiedler vector, elements \(x_i\) and \(x_j\) corresponding to vertices in different clusters will have opposite signs, maximizing the term \((x_i - x_j)^2\) for inter-cluster edges. Conversely, for intra-cluster edges, where \(x_i\) and \(x_j\) have the same sign, \((x_i - x_j)^2\) is minimized.

### Rayleigh Quotient and Graph Partitioning

The eigenvectors of the Laplacian matrix minimize the Rayleigh quotient, which for the Fiedler vector is:
$$
\frac{x^T L x}{x^T x}
$$
Given the formulation of \(x^T L x\) in terms of edge discrepancies, minimizing this quotient effectively minimizes the weighted sum of squared differences across edges for the given partitioning, constrained by the orthogonality to the trivial eigenvector and normalized by \(x^T x\).

### Practical Implications

The Fiedler vector thus leads to a partition where the number of edges between the two clusters (the "cut size") is minimized relative to the number of edges within each cluster. This is particularly useful for identifying community structures or bottlenecks in a network, where the natural divisions in the network are those that minimize connections (or potential disruptions) between different parts of the network.

This [[spectral clustering]] approach, grounded in the spectral properties of the Laplacian matrix, offers a fundamentally robust way to discern structural separations in graphs that are optimal in the sense of connectivity and cut minimization.

---

 **Algebraic Connectivity:** The second smallest eigenvalue of the Laplacian matrix, known as the algebraic connectivity or [[Fiedler Vector|Fiedler value]], indicates how difficult it is to "cut" the graph into disconnected components. A smaller value suggests that the graph can be easily disconnected.