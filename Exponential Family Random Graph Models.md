
see also:
- [[Network Science]]
- [[probabilistic models]]

Exponential Family Random Graph Models (ERGMs) are a class of statistical models used for analyzing and predicting the structure of networks. ERGMs are part of the exponential family of distributions, which is a broad class of probability distributions that includes many of the most commonly used distributions in statistics. ERGMs are particularly useful for modeling social networks, where the patterns of connections between entities (such as individuals, organizations, or countries) are of interest. They provide a flexible framework for modeling network data, allowing researchers to incorporate various effects that drive network formation, such as tendencies toward reciprocity, transitivity (the friend of my friend is my friend), and homophily (the tendency of similar individuals to be connected).

### Core Principles of ERGMs

ERGMs model the probability of a given network structure by considering the network as a whole, rather than looking at individual edges independently. This approach allows for the inclusion of complex dependencies between edges, which are critical for capturing the structural patterns observed in real-world networks.

The probability of observing a given network \(G\) under an ERGM is defined as:

$$ P(G) = \frac{1}{Z} \exp\left(\sum_{k} \theta_k g_k(G)\right) $$

where:
- \(G\) represents the observed network,
- \(Z\) is a normalization constant ensuring that the probabilities of all possible networks sum to one,
- \(\theta_k\) are parameters to be estimated from data, reflecting the strength of different network tendencies (e.g., reciprocity, transitivity),
- \(g_k(G)\) are network statistics that capture specific structural features of \(G\) (e.g., the number of mutual dyads, triangles, or other substructures).

### Key Components and Their Interpretation

- **Network Statistics (\(g_k(G)\)):** These statistics quantify specific features of the network, such as the number of edges, the number of closed triangles, or the degree distribution. They are chosen based on hypotheses about the processes driving network formation.

- **Parameters (\(\theta_k\)):** The parameters reflect how much each network statistic contributes to the overall structure of the network. A positive parameter value indicates that networks with higher values of the corresponding statistic are more probable, while a negative value suggests the opposite.

- **Normalization Constant (\(Z\)):** This constant makes the model a proper probability distribution. However, it is usually intractable to compute directly for all but the simplest networks, necessitating the use of simulation-based methods for model estimation and inference.

### Estimation and Inference

Estimating the parameters of an ERGM usually involves a combination of maximum likelihood estimation and Markov Chain Monte Carlo (MCMC) sampling, due to the computational complexity of directly calculating \(Z\) and the likelihood. The goal is to find parameter values that make the observed network structure as probable as possible under the model.

### Applications

ERGMs have wide-ranging applications, especially in social network analysis, where they are used to study friendship networks, organizational structures, online social networks, and more. They help researchers understand the underlying processes that drive network formation and evolution, such as preferential attachment, social influence, and community structure.

### Challenges and Considerations

- **Model Degeneracy:** A well-known issue with ERGMs is model degeneracy, where the model places high probability on unrealistic networks (e.g., networks with all or no connections). This is often a sign of misspecification or overly complex models.

- **Computational Complexity:** The estimation and inference of ERGMs can be computationally intensive, particularly for large networks, due to the complexity of calculating the normalization constant and the need for MCMC simulations.

ERGMs offer a rich and nuanced framework for understanding the complex patterns of connectivity that characterize networks, bridging descriptive network analysis with inferential statistics to uncover the mechanisms underlying network formation.