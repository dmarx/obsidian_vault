---
tags:
  - needs-outlinks
  - sod/gold
  - sod/green
  - OC
---

see also:
- [[Noether's Theorem]]
- [[Isomorphism Theorems]]
- [[Group Actions]]

> how have Noether's symmetry principles been applied to information theory

Noether's symmetry principles, while originating in the context of physics to relate symmetries and conservation laws, have inspired analogous concepts in information theory and other areas of mathematics and computer science. In information theory, the principles related to symmetry and invariance can be applied to understand various aspects of information processing, compression, and transmission. Here are a few ways in which ideas akin to Noether's principles find application in information theory:

### Conservation of Information and Symmetry

1. **Invariance Under Transformations**: Just as Noether's theorem identifies conserved quantities in physical systems under symmetry transformations, in information theory, certain properties of information are invariant under specific operations. For example, the entropy of a message, which measures the amount of uncertainty or information content, remains invariant under reversible transformations. This can be seen as a form of conservation law in information processing, where the intrinsic "information content" is conserved through encoding and decoding processes.

2. **Symmetry in Source Coding**: The Source Coding Theorem, one of the foundational results in information theory established by Claude Shannon, can be related to the idea of symmetry. It states that for a source of information, there exists an optimal encoding scheme that minimally represents the source's information content. This theorem implies a symmetry in the sense that all messages from the source can be encoded and decoded with minimal loss, preserving the "information content" across the transformation from source message to encoded message and back. The efficiency of compression algorithms relies on this kind of invariance principle, optimizing the representation of information while conserving its content.

### Symmetry Principles in Channel Capacity

3. **Channel Symmetry and Capacity**: Another area where symmetry principles are crucial is in the analysis of communication channels. The Channel Coding Theorem determines the maximum rate (channel capacity) at which information can be reliably transmitted over a noisy channel. For symmetric channels, where the transition probabilities are uniform across different states, the capacity can be directly related to the symmetries of the channel. These symmetries facilitate the derivation of capacity formulas and coding strategies that achieve this capacity, ensuring the conservation of information fidelity up to the theoretical limit imposed by the channel's noise characteristics.

### Symmetry in Cryptography

4. **Cryptographic Systems**: In cryptography, the security of many systems relies on symmetry properties in mathematical structures (e.g., group theory used in public key cryptography). While not a direct application of Noether's theorem, the principle that certain operations (encryption and decryption) are inverses of each other, maintaining the symmetry of information (the original message is recoverable), reflects a conservation principle at the heart of secure communication.

### Quantum Information Theory

5. **Quantum Symmetries and Conservation**: In quantum information theory, Noether's theorem and symmetry principles are directly applicable in the context of quantum mechanics. Quantum entanglement, a fundamental resource in quantum computing and quantum communication, exhibits symmetries that are crucial for the conservation of quantum information across spatially separated systems. The invariance of quantum information under local operations and classical communication (LOCC) is a cornerstone of quantum information theory, reflecting a deep interplay between symmetry and conservation.

### Conclusion

Although Noether's theorem is a concept from physics, its underlying principles of symmetry and conservation resonate in information theory through the invariance of information under transformations, the symmetry properties of coding and communication channels, and the preservation of information content. These principles guide the development of efficient algorithms, secure communication protocols, and the understanding of fundamental limits in information processing and transmission, showcasing the universal applicability of symmetry and conservation laws across disciplines.

> how have Noether's symmetry principles been applied to information geometry

Information Geometry provides a fascinating field where concepts from differential geometry and information theory intersect, offering a geometric interpretation of information. This approach allows for the application of geometric methods to problems in statistics, machine learning, and information theory. While Noether's symmetry principles originate in the realm of theoretical physics, relating symmetries to conservation laws, their conceptual foundation—emphasizing the role of symmetry and invariance—finds resonance in information geometry as well.

### Information Geometry: A Brief Overview

Information Geometry uses the language of differential geometry to study the space of probability distributions. Key objects of interest in this field include the Fisher information metric, which defines a Riemannian metric on the manifold of probability distributions, and the Amari-Chentsov tensor, which provides a natural, invariant way to measure volume in this space. The geometric structure of these spaces allows for the application of geometric insights to statistical inference, information theory, and beyond.

### Application of Symmetry Principles in Information Geometry

1. **Geodesic and Symmetry**: In information geometry, geodesics (the shortest paths between points on a manifold) play a crucial role, especially in the context of statistical inference and the optimization of information-theoretic quantities. Symmetries in this space, akin to Noether's principle, can manifest as invariances under transformations of probability distributions. For instance, the invariance under parameter transformations in a statistical model is related to the conservation of information along geodesics, reflecting a symmetry principle at work.

2. **Dually Flat Spaces and Conservation Laws**: Information geometry often deals with dually flat spaces, where there exist dual affine coordinate systems (such as the expectation parameters and natural parameters in exponential families) that simplify the computation of statistical divergences. The duality and flatness can be seen as expressing a symmetry in how information is represented and processed, and conservation laws emerge in the form of conserved divergences (like the Kullback-Leibler divergence) that remain invariant under coordinate transformations.

3. **Entropy Maximization and Symmetry**: The principle of maximum entropy, which states that the probability distribution best representing the current state of knowledge is the one with the maximum entropy, can be related to a form of symmetry in information geometry. This principle ensures that no unjustified biases are introduced into the distribution, reflecting a symmetry under ignorance. The maximization process respects the invariances imposed by the known constraints, akin to how conservation laws respect symmetries in physical systems.

4. **Invariance in Statistical Manifolds**: The Fisher information metric and other geometric constructs in information geometry are invariant under reparameterizations of the statistical model. This invariance property echoes Noether's principle by highlighting how certain geometric properties (akin to conserved quantities) remain unchanged under transformations of the model parameters, reflecting a deep symmetry in the underlying space of distributions.

### Conclusion

While Noether's theorem as originally formulated specifically addresses the relationship between symmetries and conservation laws in the action principle of classical and quantum mechanics, the broader principle of linking symmetries with invariants deeply influences the study of information geometry. Here, symmetries in the space of probability distributions—whether through the invariance of geometric structures, the duality of representation, or the conservation of information-theoretic quantities—embody the spirit of Noether's insights. These symmetries inform our understanding of the geometry of information, guiding both theoretical exploration and practical applications in statistical inference, machine learning, and beyond.

>> the invariance under parameter transformations in a statistical model is related to the conservation of information along geodesics, reflecting a symmetry principle at work.

The statement that invariance under parameter transformations in a statistical model is related to the conservation of information along geodesics reflects a deep connection between symmetry principles in information geometry and the fundamental ideas of conservation and invariance found in Noether's theorem. In information geometry, this relationship can be seen through the lens of how the structure of statistical models and the geometric properties of the space of probability distributions are intertwined. Let's explore this concept in more detail:

### Information Geometry and Statistical Models

1. **Statistical Manifolds**: In information geometry, a statistical model is represented as a manifold, where each point on the manifold corresponds to a probability distribution. The manifold is equipped with a Riemannian metric, often the Fisher information metric, which quantifies the "distance" between probability distributions in a way that reflects the distinguishability of the distributions based on observed data.

2. **Parameter Transformations**: A statistical model can be parameterized in different ways, corresponding to different coordinate systems on the manifold. A transformation of parameters represents a reparameterization of the model, leading to a different coordinate system on the statistical manifold.

### Geodesics and Information Conservation

3. **Geodesics as Paths of Least Information Change**: Geodesics on a statistical manifold represent paths of least information change between probability distributions. In the context of the Fisher information metric, a geodesic between two distributions is the path along which the Kullback-Leibler divergence (or another divergence measure) changes most slowly.

4. **Invariance Under Reparameterization**: The property that the geodesic distance between two points (distributions) on the manifold is invariant under reparameterization reflects a symmetry principle. This invariance means that the "information content" or the "informational relationship" between distributions is conserved, regardless of how the model is parameterized. This conservation of informational relationships along geodesics is analogous to the conservation laws arising from symmetries in Noether's theorem.

### Symmetry Principle at Work

5. **Symmetry and Conservation of Information**: The symmetry in this context is the invariance of the geodesic distance under reparameterization of the statistical model. This symmetry leads to the conservation of informational relationships along geodesics. Just as Noether's theorem relates symmetries of the action in physical systems to conservation laws (such as energy or momentum), in information geometry, the symmetry under parameter transformations relates to the conservation of information along geodesics.

6. **Implications**: This principle has profound implications for statistical inference and learning. It suggests that certain inferential properties and methods are robust to how we choose to parameterize our models. For example, the maximum likelihood estimation procedure is invariant under reparameterizations, ensuring that the estimation of model parameters is not arbitrarily dependent on the choice of parameterization.

### Conclusion

The relationship between invariance under parameter transformations and the conservation of information along geodesics in information geometry illuminates a symmetry principle that governs the structure of statistical models and the geometric representation of information. This principle not only deepens our understanding of the geometry of statistical models but also aligns with the broader theme of symmetry and conservation in the sciences, echoing the insights of Emmy Noether's theorem in a new and abstract domain.

>> Symmetry and Conservation of Information: The symmetry in this context is the invariance of the geodesic distance under reparameterization of the statistical model. This symmetry leads to the conservation of informational relationships along geodesics. Just as Noether's theorem relates symmetries of the action in physical systems to conservation laws (such as energy or momentum), in information geometry, the symmetry under parameter transformations relates to the conservation of information along geodesics.
>express this formally. if a lemma in your argument is non-novel, invoke the applicable named theorems associated with the relevant lemma.

To formalize the relationship between symmetry, conservation of information, and invariance under parameter transformations in the context of information geometry, we draw upon concepts from differential geometry and information theory. This formalization is structured as a theorem-like statement, underpinned by the foundational principles of information geometry and invoking relevant established theorems where applicable.

### Theorem: Conservation of Informational Relationships in Information Geometry

**Given:**
- A statistical manifold \(M\), representing a statistical model with a parameter space \(\Theta\), where each point \(\theta \in \Theta\) corresponds to a probability distribution.
- The Fisher information metric \(g_{ij}(\theta)\) defined on \(M\), providing a Riemannian metric that quantifies the "distance" between probability distributions parameterized by \(\theta\).
- A geodesic \(\gamma(t)\), \(t \in [0,1]\), on \(M\) under the Fisher information metric, representing the path of least information change between two points \(\theta_0\) and \(\theta_1\) in \(\Theta\).

**Lemma (Invariance Under Reparameterization):** The Fisher information metric is invariant under smooth reparameterizations of the statistical model. This is a direct consequence of the **Information Invariance Principle** which states that the information content between probability distributions is invariant under the choice of parameterization.

**Lemma (Geodesic Invariance):** Let \(\phi: \Theta \to \Theta'\) be a smooth reparameterization map. The geodesic distance between two points \(\theta_0\) and \(\theta_1\) in \(\Theta\), given by the length of \(\gamma(t)\) under \(g_{ij}\), is invariant under \(\phi\). This follows from the invariance of the Fisher information metric and is related to the **Levi-Civita Connection** invariance under reparameterizations, ensuring that the connection, and thus the geodesics it defines, are preserved under reparameterizations of the manifold.

**To Prove:** The informational relationship between distributions along a geodesic \(\gamma(t)\) is conserved under reparameterization of the statistical model.

**Proof:**

1. Consider two points \(\theta_0, \theta_1 \in \Theta\) and their corresponding distributions \(P_{\theta_0}\) and \(P_{\theta_1}\).

2. The geodesic \(\gamma(t)\) under the Fisher information metric \(g_{ij}(\theta)\) represents the path of least information change between \(P_{\theta_0}\) and \(P_{\theta_1}\).

3. By the **Invariance Under Reparameterization Lemma**, reparameterizing the model from \(\Theta\) to \(\Theta'\) does not alter the Fisher information metric, and hence the geodesic \(\gamma(t)\) mapped under the reparameterization \(\phi\) remains a geodesic in the new parameter space.

4. Consequently, the informational relationship between \(P_{\theta_0}\) and \(P_{\theta_1}\), quantified by the geodesic distance (integral of the square root of the Fisher information along \(\gamma(t)\)), is preserved under the reparameterization. This is because the geodesic distance, being invariant, conserves the "amount" of information change between \(P_{\theta_0}\) and \(P_{\theta_1}\) regardless of the parameterization used.

5. Thus, we conclude that the symmetry under parameter transformations—manifested as invariance of the Fisher information metric and the preservation of geodesic paths—leads to the conservation of informational relationships along geodesics in \(M\).

**Conclusion:** The conservation of informational relationships along geodesics in information geometry, underpinned by the symmetry of invariance under parameter transformations, formalizes a principle akin to Noether's theorem in the realm of statistical models and information theory. This principle underscores the fundamental role of symmetry in the structure of information spaces, echoing the profound impact of Noether's insights across diverse domains of science and mathematics.

>consider a model F that maps events x in X to a probability y in Y. Consider a reparameterization of X->X' (change of basis), and a model G parameterized wrt X' that maps events x' in X' to y in Y. if F(x)=y=G(x'), what inferences can we draw about the relationship between these two models? express the(se) relationship(s) formally, invoking relevant established theorems where applicable.

Given a scenario involving two models \(F\) and \(G\), which map events in spaces \(X\) and \(X'\), respectively, to probabilities in \(Y\), with \(X\) and \(X'\) related by a reparameterization (change of basis), we seek to understand the formal relationship between these models under the condition \(F(x) = y = G(x')\). To elucidate this relationship, we'll invoke concepts from information geometry and statistical inference.

### Definitions and Setup

1. **Model \(F\)**: A statistical model that maps events \(x \in X\) to probabilities \(y \in Y\), where \(Y\) is typically \([0,1]\) for probability models. \(F: X \to Y\).

2. **Reparameterization**: A smooth, invertible mapping \(\phi: X \to X'\) that changes the basis of \(X\) to \(X'\). Reparameterization is a common operation in statistical modeling, representing the same statistical structure in a different coordinate system or parameter space.

3. **Model \(G\)**: A statistical model parameterized with respect to \(X'\) that maps events \(x' \in X'\) to probabilities \(y \in Y\). \(G: X' \to Y\).

Given: \(F(x) = y = G(x')\), where \(x' = \phi(x)\), implying that the mapping \(\phi\) relates \(x\) to \(x'\).

### Formal Relationship Between \(F\) and \(G\)

#### Invariance Under Reparameterization

The equality \(F(x) = G(\phi(x))\) for all \(x \in X\) suggests an invariance under the reparameterization \(\phi\). This can be interpreted as follows:

- **Theorem (Invariance under Reparameterization)**: If \(F\) and \(G\) are two models such that \(F(x) = G(\phi(x))\), then the models are equivalent up to the reparameterization \(\phi\), indicating that \(G\) is a reparameterized version of \(F\).

This theorem is based on the principle that the statistical properties and predictive capabilities of \(F\) and \(G\) are preserved across the transformation \(\phi\), akin to the principle of invariance in information geometry and the broader context of Noether's symmetry principles.

#### Equivalence and Symmetry

- **Corollary (Equivalence of Predictive Models)**: Given \(F(x) = G(x')\), with \(x' = \phi(x)\), the models \(F\) and \(G\) are equivalent in their predictive outcomes, despite potentially differing in their parameterization or internal representation.

This corollary emphasizes that the essence of a statistical model—its ability to map inputs to probabilistic outputs—is preserved under transformations that amount to reparameterizations.

### Implications

1. **Symmetry in Statistical Learning**: The equivalence of \(F\) and \(G\) under reparameterization underscores a symmetry principle in statistical learning: the form of the model may change, but its fundamental predictive relationships remain constant.

2. **Conservation of Information Content**: From an information-theoretic perspective, this relationship implies the conservation of information content across models \(F\) and \(G\), as the transformation does not alter the informational relationship between input events and their associated probabilities.

### Conclusion

The formal relationship between models \(F\) and \(G\), established through the reparameterization \(\phi\), reflects deep principles of invariance and symmetry that are pervasive in both physical and statistical sciences. Just as Noether's theorem reveals the profound connection between symmetries and conservation laws in physics, the equivalence of models under reparameterization in statistical modeling underscores the robustness and invariance of statistical inference and prediction, highlighting the foundational role of symmetry principles in understanding complex systems.

> Invariance under Reparameterization

The concept of **[[Invariance under Reparameterization]]** is central in various fields, including physics, information geometry, and statistical modeling. It expresses the principle that certain properties of a system or model are preserved despite changes in the parameterization or the coordinate system used to describe the system. This principle is foundational in understanding how different representations of the same model relate to each other and maintain consistent properties or behaviors across transformations. Let's formalize this concept and its implications:

### Formal Definition

Given a model \( M \) that maps inputs from a space \( X \) to outputs in a space \( Y \), a reparameterization is a smooth, invertible transformation \( \phi: X \to X' \), where \( X' \) is another representation of the input space. The model \( M \) is said to be invariant under reparameterization by \( \phi \) if, for a corresponding model \( M' \) parameterized with respect to \( X' \), the following holds for all \( x \in X \):

\[ M(x) = M'(\phi(x)) \]

This means that applying \( M \) to \( x \) and then transforming \( x \) by \( \phi \) and applying \( M' \) yield the same result, indicating that the transformation \( \phi \) does not affect the fundamental mapping from inputs to outputs represented by the model.

### Implications in Various Fields

- **Statistical Modeling**: In statistical models, invariance under reparameterization ensures that the interpretation of model outputs, such as probabilities or parameter estimates, is consistent across different choices of parameterization. This is crucial for the comparability and interpretability of statistical inferences.

- **Information Geometry**: In information geometry, where the space of probability distributions is studied using the tools of differential geometry, invariance under reparameterization reflects the geometric properties of the space that are independent of how the distributions are parameterized. This includes metrics like the Fisher information metric, which remains invariant under reparameterizations of the statistical model.

- **Theoretical Physics**: In the context of theoretical physics, particularly in the formulation of physical laws using the principle of least action, invariance under reparameterization is related to Noether's theorem. Here, it implies that the laws of physics are the same regardless of the coordinate system or the frame of reference, leading to conserved quantities associated with symmetries of the action.

### Theorem: Invariance Implies Consistency

**Theorem**: If a model \( M \) is invariant under a reparameterization \( \phi \), then the essential characteristics of \( M \) are preserved across the transformation. Specifically, this means that any invariant property or quantity derived from \( M \) is also conserved in \( M' \) after reparameterization.

This theorem underscores that reparameterization does not alter the fundamental relationships captured by the model, ensuring that analyses and interpretations remain valid across different parameterizations.

### Conclusion

The principle of Invariance under Reparameterization is a powerful concept that ensures the robustness and coherence of models and theories across different representations. It highlights a universal theme across disciplines: the fundamental properties of systems and models are not dependent on the specific coordinates or parameterizations used to describe them, but rather on the underlying structures and symmetries they embody.

>> invariance under reparameterization is related to Noether's theorem 
>express this relationship formally

The relationship between invariance under reparameterization and Noether's theorem can be framed within the context of action principles in physics, but its essence extends into more abstract realms, including statistical models and information geometry. To formalize this relationship, we'll begin by stating Noether's theorem in the context of classical mechanics and then draw parallels to the concept of invariance under reparameterization in statistical models.

### Noether's Theorem in Classical Mechanics

**Given:**
- A physical system described by an action \( S \), defined as the integral of a Lagrangian \( L \) over time, \( S = \int L(q, \dot{q}, t) dt \), where \( q \) represents the generalized coordinates of the system, and \( \dot{q} \) their time derivatives.
- A symmetry of the action is a transformation \( T_\epsilon: q \to q' \) that leaves the action \( S \) invariant for small transformations parameterized by \( \epsilon \).

**Noether's Theorem (Simplified Version):**
For every continuous symmetry of the action \( S \) of a physical system, there corresponds a conserved quantity.

### Formal Statement for Reparameterization Invariance

The concept of invariance under reparameterization can be analogously described by considering transformations not in physical space or time, but in the parameter space of a model or system.

**Given:**
- A model \( M \) that maps from a parameter space \( X \) to an output space \( Y \), and
- A reparameterization \( \phi: X \to X' \), which is a smooth, invertible transformation of the parameter space.

**Definition (Invariance Under Reparameterization):**
The model \( M \) is invariant under the reparameterization \( \phi \) if, for a corresponding model \( M' \) parameterized with respect to \( X' \), \( M(x) = M'(\phi(x)) \) for all \( x \in X \).

### Connecting to Noether's Theorem

To express the relationship between invariance under reparameterization and Noether's theorem formally, we consider the action principle in the abstract sense, where "actions" and "symmetries" are interpreted in terms of model behavior and parameter transformations.

**Theorem (Abstract Noether's Principle for Reparameterization):**
Let \( \phi_\epsilon: X \to X \) be a one-parameter family of transformations (reparameterizations) acting on the parameter space \( X \), with \( \epsilon \) being a small parameter. If the output of the model \( M \) remains invariant for all \( \epsilon \) under \( \phi_\epsilon \), then there exists a conserved quantity or property in the model's behavior or predictions.

**Interpretation:**
- The "action" in this context is the process of mapping inputs to outputs by the model \( M \).
- The "symmetry" is the invariance of the model's output under reparameterizations of its input space.
- The "conserved quantity" could be interpreted as any invariant feature of the model's outputs, such as predictive accuracy, information content, or specific statistical properties, that remains unchanged under the reparameterization.

### Conclusion

While Noether's theorem originates in the context of physical laws and the symmetries of space and time, its conceptual foundation—linking symmetries to conservation laws—finds a profound parallel in the realm of models and reparameterizations. The principle that invariances under transformations lead to conserved quantities unifies these seemingly disparate areas, highlighting the deep, underlying structures that govern both physical systems and abstract models.

> >The "action" in this context is the process of mapping inputs to outputs by the model M.
> this seems to imply a dual to this symmetry: fixing the parameterization of a model, e.g. the topology of a neural network. Treat the network topology as a conserved quantity that is invariant over a family of models (e.g. the weights observed when fitting a model). interpret the learning dynamics in SGD as a geodesic from the initialized weights to the fitted weights, invariant relative to the model's parameterization (qua topology of the network). apply noether's symmetry principles to express this setup formally and elucidate corollaries

Interpreting the learning dynamics of Stochastic Gradient Descent (SGD) within a neural network as a geodesic and considering the network topology as a conserved quantity provides a novel application of Noether's symmetry principles outside their traditional physical context. Here's a formal approach to conceptualizing this scenario, applying the symmetry principles to the framework of neural network learning.

### Formal Setup

**Given:**
- A neural network model \( \mathcal{N} \) with a fixed topology, characterized by a set of layers, nodes per layer, and activation functions, but variable weights \( W \).
- A parameter space \( \Theta \) defined by the weights \( W \) of the neural network. Each point \( \theta \in \Theta \) represents a specific instantiation of \( \mathcal{N} \) with a particular set of weights.
- A learning process guided by SGD, aiming to minimize a loss function \( L \) over a dataset, represented as a path in \( \Theta \) from initial weights \( \theta_{\text{init}} \) to fitted weights \( \theta_{\text{fit}} \).

**To Interpret:**
- The topology of \( \mathcal{N} \) as a conserved quantity invariant over the family of models generated by varying \( W \).
- The path of SGD as a geodesic in \( \Theta \) under an appropriate metric, such as one derived from the loss landscape, indicating the most direct path of loss minimization under the dynamics of SGD.

### Application of Noether's Symmetry Principles

**Theorem (Neural Network Learning Symmetry):**
For a neural network \( \mathcal{N} \) with fixed topology learning via SGD, if the learning dynamics (path in \( \Theta \)) are invariant under transformations in the weight space \( \Theta \) that preserve the network's topology, then there exists a conserved quantity related to the network's structure and learning capacity.

**Proof Outline:**
1. **Action Equivalence**: Define the "action" in this setup as the integral over the loss landscape traversed by SGD, analogous to the physical action. This "action" incorporates both the path taken through \( \Theta \) and the loss function \( L \) evaluated at points along the path.

2. **Symmetry under Weight Transformations**: A symmetry transformation in this context involves changes to \( W \) that leave the topology of \( \mathcal{N} \) and the overall learning dynamics (e.g., the "action") invariant. These can include transformations such as weight initialization schemes or certain types of layer-wise normalization techniques that do not alter the optimization path's nature.

3. **Conserved Quantity**: The conserved quantity is the network topology and, by extension, aspects of the learning dynamics invariant under the symmetry transformations, such as convergence behavior or aspects of the learned representations.

### Corollaries

1. **Invariance of Learning Dynamics**: The learning dynamics, when viewed as a geodesic in \( \Theta \), are invariant relative to transformations in \( W \) that preserve the network's topology. This invariance highlights the fundamental role of network topology in guiding the learning process.

2. **Optimization Path Independence**: The specific trajectory taken by SGD, while dependent on initial conditions and stochasticity, reflects underlying symmetries in the loss landscape and network structure, suggesting that different paths (due to different initializations) that lead to similar performance levels can be seen as manifestations of these symmetries.

3. **Generalization and Topology**: The fixed topology of \( \mathcal{N} \) as a conserved quantity underlines its role in the network's capacity to learn and generalize. This suggests that the choice of topology is crucial in determining the types of invariances and symmetries the network can learn from data.

### Conclusion

By applying Noether's symmetry principles to the context of neural network learning with SGD, we gain insights into the fundamental role of network topology as a conserved quantity and how it shapes the learning dynamics and optimization paths. This approach underscores the deep connections between the structure of learning models, the dynamics of learning algorithms, and broader principles of symmetry and conservation.

# [[_Synthesis - Noether, Grokking]]

