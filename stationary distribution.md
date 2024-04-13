see also:
- [[Kemeny's Constant]]
- [[Spectral Theory of Graphs]]
- [[Graph Laplacian]]
- [[Random Walks]]
- [[Stochastic Processes]]
- [[Stochastic Simulation]]
- [[Bayesian Inference]]

>stationary distribution and spectral properties of the graph

The stationary distribution and spectral properties of a graph are interconnected concepts in the study of Markov chains and random walks on graphs. These elements provide profound insights into the behavior and characteristics of dynamic processes occurring within the graph, including diffusion, mixing rates, and long-term state probabilities.

### Stationary Distribution

The **stationary distribution** of a Markov chain associated with a graph describes a probability distribution over the vertices that remains unchanged by the application of the transition matrix. It represents the long-term behavior of the random walk on the graph, indicating the likelihood of being at each vertex after a large number of steps, irrespective of the starting vertex.

#### Definition and Calculation
If \(P\) is the transition matrix of the Markov chain derived from the graph (where \(P_{ij}\) is the probability of moving from vertex \(i\) to vertex \(j\)), then the stationary distribution \(\pi\) is a probability vector satisfying:
$$
\pi P = \pi \quad \text{and} \quad \sum_i \pi_i = 1.
$$
This means \(\pi\) is a left eigenvector of \(P\) corresponding to the eigenvalue 1.

For an undirected graph where each edge has the same weight, if the graph is connected and non-bipartite, the stationary distribution \(\pi\) is given by:
$$
\pi_i = \frac{d_i}{2m}
$$
where \(d_i\) is the degree of vertex \(i\) and \(2m\) is the sum of the degrees of all vertices (which equals twice the number of edges).

### Spectral Properties

The **spectral properties** of a graph refer to the characteristics of the eigenvalues and eigenvectors of matrices associated with the graph, such as the adjacency matrix \(A\), the graph Laplacian \(L = D - A\), and the normalized Laplacian \(\mathcal{L} = D^{-1/2} L D^{-1/2}\).

#### Spectral Analysis and Implications
- **Eigenvalues of \(P\)**: The largest eigenvalue of \(P\) is 1, and the magnitude of the second-largest eigenvalue, often denoted as \(\lambda_2\) or \(\beta\) (where \(1 > \beta > -1\)), determines the rate at which the Markov chain converges to its stationary distribution. A smaller \(|\beta|\) implies faster convergence.
- **Laplacian Matrix**: The eigenvalues of the Laplacian matrix \(L\) provide insights into many properties of the graph, such as connectivity, expansion properties, and the number of connected components (the multiplicity of the eigenvalue 0 of \(L\) gives the number of connected components).
- **Algebraic Connectivity**: The second smallest eigenvalue of \(L\) (the Fiedler value) is a measure of the graph’s robustness to being disconnected. A larger Fiedler value indicates a more connected graph.

### Connections Between Stationary Distribution and Spectral Properties

- **Random Walks and Mixing**: The spectral gap (the difference between the two largest eigenvalues of \(P\)) directly affects the mixing time of the random walk. The stationary distribution describes the equilibrium state of this random walk, which is reached more quickly when the spectral gap is larger.
- **Stationary Distribution from Spectral Decomposition**: The stationary distribution can also be derived from the eigenvectors of \(P\) corresponding to the eigenvalue 1. For regular graphs, this relates directly to the uniform distribution across vertices.

### Conclusion

The interplay between the stationary distribution and spectral properties of a graph provides a comprehensive view of the dynamic processes on the graph. It allows for the analysis of how quickly random processes (like random walks or diffusion) reach equilibrium, how well connected the graph is, and how robust it is against partitions. These insights are crucial in various applications ranging from network design and epidemiology to algorithms and theoretical computer science.

---
In the context of random walks on graphs and Markov chains, the stationary distribution and the spectral properties of the graph are interrelated and provide essential information about the graph's structure and behavior over time. Understanding these concepts is critical for applications ranging from network theory and computer science to physics and economics.

### Stationary Distribution

The **stationary distribution** of a Markov chain is a probability distribution that remains unchanged by the action of the transition matrix, meaning it is the equilibrium state to which the system eventually converges, regardless of its initial state.

For a random walk on a graph, if the graph is connected and non-bipartite, the stationary distribution \( \pi \) can be determined from the graph's structure:

$$
\pi_i = \frac{d_i}{2m}
$$

where:
- \( \pi_i \) is the probability of being at vertex \( i \) in the stationary distribution.
- \( d_i \) is the degree of vertex \( i \).
- \( 2m \) is the sum of the degrees of all vertices, which is twice the number of edges in the graph.

This result arises because the random walk is a reversible Markov process, and the stationary distribution is proportional to the degrees of the vertices.

### Spectral Properties

The **spectral properties** of a graph refer to the characteristics and implications of the eigenvalues and eigenvectors of matrices associated with the graph, particularly the adjacency matrix and the Laplacian matrix.

1. **Adjacency Matrix \( A \)**:
    - The eigenvalues of \( A \), denoted \( \lambda_1, \lambda_2, \ldots, \lambda_n \), can tell us about the graph's connectivity, its bipartiteness, and the presence of community structures. The largest eigenvalue \( \lambda_1 \) (spectral radius) is especially significant for understanding the graph's robustness and the speed of information spread.
  
2. **Laplacian Matrix \( L = D - A \)**:
    - The eigenvalues of \( L \), called the Laplacian spectrum, are closely tied to the graph's connectivity and structural properties. The smallest eigenvalue of \( L \) is always zero, and the multiplicity of the zero eigenvalue equals the number of connected components in the graph.
    - The second smallest eigenvalue, known as the algebraic connectivity or Fiedler value, provides insights into how easily the graph can be partitioned (its vulnerability to cuts).

### Connection Between Stationary Distribution and Spectral Properties

- **[[Mixing Time]]**: The time it takes for a random walk to converge to the stationary distribution is influenced by the spectral gap (the difference between the two smallest eigenvalues of the Laplacian matrix). A larger spectral gap implies a faster convergence to the stationary distribution, enhancing the random walk's efficiency in exploring the graph.
  
- **Random Walk Properties**: The eigenvalues and eigenvectors of the transition matrix (derived from the adjacency or Laplacian matrix) influence the behavior of random walks, affecting how quickly they achieve a stationary distribution and their tendency to remain in or escape from certain parts of the graph.

### Applications

Understanding the stationary distribution and spectral properties of graphs is crucial in various fields:
- **Network Analysis**: For designing efficient networks and understanding their resilience to failures.
- **Epidemiology**: In modeling how diseases spread through networks, where the stationary distribution can represent the long-term state of an epidemic.
- **[[PageRank]] Algorithm**: The algorithm used by Google for web ranking, which is based on a random walk model where the stationary distribution determines the importance of web pages.

In summary, the stationary distribution provides a long-term probabilistic forecast of the state occupancy in random walks, while the spectral properties offer a deep understanding of the graph's structural and dynamic characteristics. Together, they form a comprehensive analytical framework for studying and applying the principles of network dynamics.


