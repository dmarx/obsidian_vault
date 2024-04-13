see also:
- [[Sinkhorn Distances]]
>tell me more about Optimal Transport and the Wasserstein Distance

[[Optimal Transport]] (OT) and the Wasserstein Distance are fundamental concepts in mathematics and computer science, providing a rigorous framework for comparing probability distributions. These concepts have gained significant attention across various fields, including economics, machine learning, and computational geometry, due to their ability to capture the intuitive notion of moving mass in the most efficient way possible. Here’s a deeper dive into both:

### Optimal Transport

The theory of Optimal Transport dates back to the French mathematician Gaspard Monge in the 18th century, although the modern formulation and significant developments were made in the 20th century by Leonid Kantorovich. OT seeks the most cost-effective strategy for transporting resources (mass) from one configuration to another. The problem can be visualized as finding the best way to move piles of sand from several origins to several destinations, minimizing the total cost associated with moving each grain of sand.

### Mathematical Formulation

Mathematically, given two probability distributions \( \mu \) and \( \nu \) over spaces \( X \) and \( Y \), and a cost function \( c(x, y) \) that describes the cost of moving a unit of mass from \( x \) to \( y \), the OT problem seeks a transport plan \( \gamma \) that minimizes the total cost:

\[ \text{Minimize} \int_{X \times Y} c(x,y) d\gamma(x,y) \]

subject to \( \gamma \) being a joint distribution whose marginals are \( \mu \) and \( \nu \). In simpler terms, it looks for the cheapest way to rearrange \( \mu \) into \( \nu \) according to the cost function \( c \).

### Wasserstein Distance

The Wasserstein Distance, also known as the Earth Mover's Distance, emerges from the OT problem as a particular case where the cost function \( c(x, y) \) measures the distance between points in a metric space. Specifically, the \(p\)-Wasserstein distance between two distributions is defined using the optimal transport cost with \( c(x, y) = \text{distance}(x, y)^p \), for some \( p \geq 1 \). The \( 1 \)-Wasserstein distance is often used due to its intuitive interpretation as the "least amount of work" required to transform one distribution into the other, with "work" being quantified as mass times distance.

### Applications

- **Machine Learning and Data Science**: In these fields, the Wasserstein distance has been used to compare probability distributions in various tasks, such as generative adversarial networks (GANs) where it helps in measuring the distance between the generated data distribution and the real data distribution.
- **Image Retrieval and Processing**: The Wasserstein distance can quantify the similarity between images in a more nuanced way than traditional methods, taking into account the spatial distribution of pixel intensities.
- **Economics and Resource Allocation**: OT models can simulate and solve problems related to resource allocation, logistics, and transport in a way that minimizes costs or maximizes efficiency.

### Computational Aspects

While the OT problem and the Wasserstein distance offer powerful theoretical tools, their direct computation, especially for high-dimensional data, can be challenging due to computational complexity. However, recent advancements, including the use of entropic regularization (leading to Sinkhorn distances) and neural network approximations, have made these tools more accessible and practical for large-scale applications.

In essence, Optimal Transport and the Wasserstein Distance provide a robust framework for analyzing and solving diverse problems involving the movement and transformation of distributions. Their ability to incorporate the geometry of the underlying space makes them particularly appealing for applications that require a nuanced understanding of how distributions differ from one another.

---

see also:
- [[Ollivier-Ricci curvature]]

The Wasserstein distance, also known as the Earth Mover's distance (EMD), is a measure of the distance between two probability distributions over a given space. It originates from the field of optimal transport, a branch of mathematics concerned with finding the most efficient way to move mass from one distribution to another. The Wasserstein distance is particularly useful because it takes into account the underlying geometry of the space, making it a powerful tool for comparing distributions that are not only different in mass but also located differently within the space.

### Definition

Given two probability distributions \(P\) and \(Q\) over a metric space \(M\), with a distance metric \(d\) defined on \(M\), the Wasserstein distance of order \(p\) between \(P\) and \(Q\) is defined as:

$$
W_p(P, Q) = \left( \inf_{\gamma \in \Gamma(P, Q)} \int_{M \times M} d(x, y)^p d\gamma(x, y) \right)^{1/p}
$$

where:
- \(\Gamma(P, Q)\) is the set of all joint distributions \(\gamma\) on \(M \times M\) with marginals \(P\) and \(Q\).
- \(d(x, y)\) is the distance between points \(x\) and \(y\) in \(M\).
- The infimum (inf) is taken over all possible transport plans \(\gamma\) that describe how mass is moved from \(P\) to \(Q\).

The most commonly used Wasserstein distances are \(W_1\) (the first-order Wasserstein distance) and \(W_2\) (the second-order Wasserstein distance), with \(W_1\) often being used for practical applications due to its computational properties and interpretability as the minimum work required to transform \(P\) into \(Q\).

### Interpretation

The Wasserstein distance can be interpreted as the minimum cost required to transform one probability distribution into another, with the cost computed based on the distances each unit of mass has to be moved. This makes it especially suited for applications where the spatial arrangement of the distributions is important.

### Applications

- **Image Processing and Computer Vision:** Wasserstein distance is used in comparing images represented as distributions of features or pixel intensities.
  
- **Machine Learning:** It is employed in generative adversarial networks (GANs) to measure the distance between the distribution of generated data and real data, improving the training process and the quality of generated samples.
  
- **Data Science:** Wasserstein distance finds applications in clustering, anomaly detection, and domain adaptation, where measuring how similar or different two distributions are is crucial.
  
- **Geosciences and Environmental Science:** Used in analyzing spatial distributions of phenomena such as rainfall or pollution levels.

### Challenges

- **Computational Complexity:** Computing the Wasserstein distance, especially in high-dimensional spaces, can be computationally intensive, although recent advances have led to more efficient algorithms and approximations.

- **Choice of Metric:** The choice of the distance metric \(d\) in the underlying space \(M\) can significantly impact the Wasserstein distance, requiring careful consideration based on the application.

The Wasserstein distance offers a nuanced way to compare distributions, capturing both the amount of mass that needs to be moved and the distance it needs to be moved over, making it a valuable tool in various analytical and machine learning applications.