see also:
- [[Network Science]]
- [[Anomaly Detection]]
- [[Renormalization Group Theory]]
- [[Pooling]]
- [[levels of abstraction]]

Scan statistics on network graphs are a powerful tool for identifying regions of unusual activity or clustering within a network. Traditionally used in spatial statistics to detect clusters of events in geographic space, the concept of scan statistics has been adapted to the domain of network science to analyze patterns over graphs or networks. In the context of networks, scan statistics are employed to identify subgraphs (or clusters) where the observed number of events (such as communications, transactions, or social interactions) significantly deviates from what would be expected under a null model of random distribution.

### Core Concepts of Scan Statistics in Network Graphs

- **Subgraph Identification:** The primary goal is to scan the network graph for all possible subgraphs according to certain criteria (size, connectivity, etc.) and evaluate the concentration of events within these subgraphs.

- **Statistical Significance:** For each subgraph, the scan statistic measures the significance of the observed clustering of events. This involves comparing the observed number of events within the subgraph to the distribution of events expected under a null hypothesis of random occurrence throughout the network.

- **Null Model:** The null model is crucial as it provides a baseline against which observed data can be compared. In network graphs, the null model must account for the network's topology, including the distribution of node degrees and the overall density of connections.

### Application of Scan Statistics

Applications of scan statistics in network graphs span various domains, including:

- **Epidemiology:** Detecting outbreaks of disease by identifying clusters of cases in contact networks.
- **Cybersecurity:** Identifying unusual patterns of network traffic that may indicate cyber attacks or system failures.
- **Social Network Analysis:** Finding communities or clusters within social networks where there is an unusually high level of interaction.
- **Finance:** Detecting fraud by identifying clusters of transactions that deviate from typical patterns.

### Methodological Steps

1. **Network Representation:** The first step involves representing the system of interest as a network graph, where nodes represent entities (individuals, computers, etc.) and edges represent interactions or relationships.

2. **Event Mapping:** Events of interest are mapped onto the network, associating each event with a specific node or edge.

3. **Subgraph Enumeration:** Potentially interesting subgraphs are enumerated based on predefined criteria, which could include the number of nodes, geographical proximity (in physical networks), or connectivity patterns.

4. **Statistical Analysis:** For each subgraph, the number of observed events is compared to the expectation under the null model using the scan statistic. This usually involves calculating a likelihood ratio or other measures to assess the significance of the deviation.

5. **Correction for Multiple Testing:** Given the potentially large number of subgraphs analyzed, appropriate statistical corrections (such as Bonferroni correction or False Discovery Rate methods) are applied to account for multiple testing and reduce the risk of false positives.

### Challenges and Considerations

- **Computational Complexity:** Enumerating all possible subgraphs and calculating scan statistics for each can be computationally intensive, especially in large or densely connected networks.
  
- **Choice of Null Model:** The selection of an appropriate null model is critical and challenging, as it must accurately reflect the random processes underlying the network's formation and the distribution of events under normal conditions.

- **Interpretation:** Determining the practical significance of detected clusters requires domain-specific knowledge and careful interpretation, especially in understanding the mechanisms driving the observed clustering.

### Conclusion

Scan statistics offer a rigorous and statistically sound method for identifying clusters of events in network graphs, providing valuable insights into the structure and dynamics of complex systems across various fields. As computational methods and data availability continue to improve, the application of scan statistics in network analysis is likely to expand, offering deeper insights into the phenomena underlying connected systems.

---

>scan statistics and renormalization group theory

The integration of scan statistics with renormalization group (RG) theory presents an intriguing approach to analyzing and understanding complex systems, particularly in the context of identifying significant clusters or patterns within data that spans across different scales. While scan statistics provide a method for detecting localized clusters of events that are statistically significant against a background distribution, RG theory offers a powerful framework for understanding how the behavior of systems changes as one observes them at different scales. Combining these approaches can enhance our ability to detect and interpret patterns in complex datasets, from physical to social and biological systems.

### Scan Statistics

Scan statistics are used to identify clusters or "hotspots" of activity within data. The method involves scanning a dataset with a window of varying sizes and locations, looking for clusters of events that are unlikely to occur by chance. In network science, this translates to searching for subgraphs where interactions or events are densely concentrated, more so than what would be expected under a null model of random distribution.

### Renormalization Group Theory

RG theory originated in the field of statistical physics to deal with critical phenomena and phase transitions, providing a systematic way to study how the properties of a system change as one observes it at different scales. By progressively "coarse-graining" a system—essentially averaging out the details at smaller scales and focusing on larger-scale behavior—RG theory can determine which features of the system are scale-invariant and thus critical to its overall behavior. This approach has been instrumental in understanding phenomena such as the universality of critical exponents in phase transitions.

### Combining Scan Statistics and RG Theory

Integrating scan statistics with RG theory involves using the scan statistic methodology to detect clusters at various scales and employing RG concepts to understand how these clusters' significance and characteristics change across scales. This combination could be particularly powerful in several ways:

- **Multi-Scale Cluster Detection:** By applying scan statistics iteratively at different scales—akin to the coarse-graining step in RG theory—one can identify significant clusters of events that persist or change in importance across scales. This is crucial for distinguishing between noise and truly significant patterns that are robust across observational scales.

- **Scale-Invariant Properties:** RG theory can help identify properties of clusters detected by scan statistics that are scale-invariant, offering deeper insights into the underlying processes that generate these clusters. For example, in the analysis of social networks, this approach could reveal how community structures or information cascades manifest differently at the scale of tight-knit groups versus entire populations.

- **Critical Phenomena in Complex Systems:** The combination can be used to study critical phenomena in complex systems, such as the thresholds for epidemic spreading or information cascades, by examining how clusters of related events grow and connect as one adjusts the scale of observation. This could lead to a better understanding of the conditions under which a system transitions from one state to another (e.g., from disease-free to epidemic states).

### Challenges and Opportunities

- **Computational Complexity:** The integration of these methodologies is computationally challenging, requiring sophisticated algorithms to efficiently scan for clusters at multiple scales and to perform the RG analysis.
  
- **Interdisciplinary Application:** This approach spans disciplines, from physics to epidemiology, social science, and beyond. Tailoring the combination of scan statistics and RG theory to specific fields involves bridging gaps in terminology, methodology, and theoretical frameworks.

- **Theoretical Development:** Further theoretical work is needed to formalize the integration of scan statistics with RG theory, including developing appropriate null models for different scales and understanding the implications of scale invariance for cluster significance.

Integrating scan statistics with renormalization group theory opens new avenues for analyzing complex systems, offering the potential to uncover fundamental principles governing system behavior across scales. This interdisciplinary endeavor could lead to significant advances in our understanding of complex phenomena, from the microscale interactions within materials to the macroscale dynamics of social networks and ecosystems.