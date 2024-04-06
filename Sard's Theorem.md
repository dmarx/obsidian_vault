see also:
- [[Intersection Theory]]

Sard's Theorem, named after the American mathematician [[Arthur Sard]], is a foundational result in [[differential topology]] that provides crucial insights into the structure of [[differentiable mappings]] between [[manifolds]]. This theorem concerns the "size" and properties of critical values of smooth functions, offering a surprisingly powerful tool for understanding how [[differentiable maps]] distort spaces.

### Statement of Sard's Theorem

Let $f: M \to N$ be a smooth map between [[differentiable manifolds]] $M$ and $N$, where $\dim(M) \geq \dim(N)$. A point $x \in M$ is called a **[[Critical Points|critical point]]** of $f$ if the differential $df_x: T_xM \to T_{f(x)}N$ (the linear map between the [[tangent space|tangent spaces]] at $x$ and $f(x)$, respectively) is not surjective. A value $y \in N$ is a **critical value** if there exists a critical point $x \in M$ such that $f(x) = y$; otherwise, $y$ is a **regular value**.

**Sard's Theorem** states that the set of critical values of $f$ has measure zero in $N$. In other words, "most" points in $N$ are regular values for the map $f$.

### Implications and Intuition

The theorem suggests that, despite the potentially infinite complexity of a smooth map's behavior, the "bad set" where this map fails to be locally invertible (due to critical points mapping to critical values) occupies an insignificantly small portion of the target space in terms of [[measure]]. This has profound implications:

- **Generic Properties**: It implies that for almost every point in the target space, the pre-image under a smooth map behaves nicely, often resembling a smooth submanifold of the source space. This supports the intuition that "most" situations or configurations one might randomly choose are not pathological.

- **[[Transversality]] and Perturbations**: Sard's Theorem underlies many results in transversality, suggesting that small perturbations of a smooth map can avoid creating undesirable intersections or critical points, thus facilitating generic conditions for smoothness and regularity in intersections of manifolds.

### Applications

- **[[Inverse Function Theorem]] and [[Implicit Function Theorem]]**: Sard's Theorem provides the groundwork for these fundamental results, ensuring that smooth maps are locally invertible away from a set of measure zero.

- **[[Morse Theory]]**: In Morse theory, Sard's Theorem guarantees that almost all level sets of a Morse function are smooth manifolds, which is crucial for analyzing the topological structure of the underlying space via critical points of the function.

- **[[Singularity Theory]]**: The theorem is instrumental in singularity theory, where it aids in the study of spaces of mappings and the classification of singularities by showing that singular mappings are rare.

### Mathematical Formalization

In more formal terms, consider a smooth map $f: \mathbb{R}^n \to \mathbb{R}^m$ and let $C \subset \mathbb{R}^n$ be the set of critical points, where the [[Jacobian]] matrix of $f$ at each point of $C$ has rank less than $m$. Sard's Theorem asserts that the image $f(C) \subset \mathbb{R}^m$ has [[Lebesgue measure]] zero, which means that for almost every point $y \in \mathbb{R}^m$, the pre-image under $f$ is a set of points where the map $f$ behaves like a [[submersion]], allowing for local inverses and implying regularity of the level sets and [[fibers]] over $y$.

### Versions and Generalizations

Sard's Theorem has been extended to various contexts beyond smooth maps between finite-dimensional manifolds, including maps of [[Sobolev spaces]] and certain classes of nonsmooth maps. These generalizations maintain the spirit of Sard's result, emphasizing the predominance of regularity in the behavior of mathematical objects under general conditions.