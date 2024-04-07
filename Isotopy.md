Isotopy is a concept from topology, particularly from the field of [[geometric topology]], that describes a continuous deformation between two geometric objects within a given space. It is a specific type of homotopy, which is restricted to embeddings, meaning it deals with ways of continuously transforming one embedding of an object into another without "tearing" or "gluing" parts of the object. This concept is crucial for understanding the equivalence of geometric figures and structures under continuous transformations that preserve the object's topology.

### Formal Definition

Two [[embeddings]] $f, g: X \rightarrow Y$ of a [[topological space]] $X$ into a topological space $Y$ are **isotopic** if there exists a continuous family of embeddings $h_t: X \rightarrow Y$ for $t \in [0, 1]$ such that:

- $h_0 = f$ and $h_1 = g$.
- For each $t \in [0, 1]$, $h_t$ is an embedding.

The function $H: X \times [0, 1] \rightarrow Y$ defined by $H(x, t) = h_t(x)$ is called an **isotopy** between $f$ and $g$. Essentially, isotopy provides a "continuous path" of embeddings from $f$ to $g$, showing that one can be transformed into the other without intersecting itself or breaking apart.

### Isotopy vs. Homotopy

While both concepts involve continuous transformations, the distinction lies in their restrictions and applications:

- **[[Homotopy]]** requires only the continuity of the transformation and applies to continuous functions in general. It is a broader concept used to understand the equivalence of spaces and functions in a topological sense.

- **Isotopy**, on the other hand, applies specifically to embeddings and preserves the embedded object's "intactness" and "separateness" throughout the transformation. This makes isotopy a stricter condition than homotopy.

### Applications of Isotopy

- **[[Knot Theory]]**: In knot theory, isotopy is used to define when two knots are considered the same. Two knots are equivalent if there is an isotopy of $\mathbb{R}^3$ (or $S^3$) that takes one knot onto the other. This concept helps classify knots and links.

- **Surface Classification**: Isotopy is used in the classification of surfaces and the study of [[surface homeomorphisms]], determining when two surface embeddings are equivalent.

- **[[Differential Topology]]**: In differential topology, isotopy can distinguish between different smooth structures on [[manifolds]], helping to understand the manifold's geometry and topology.

### Examples

- **Plane Curves**: Two simple closed curves on the plane are isotopic if one can be continuously deformed into the other without crossing itself.

- **Knots and Links**: Two knots in three-dimensional space are considered the same (or isotopic) if one can be transformed into the other through a continuous deformation of space that doesn't break or pass the string through itself.

Isotopy serves as a powerful tool in topology and geometry, providing a precise way to discuss the equivalence of geometric structures and embeddings. It captures the intuitive notion of shapes being "the same" if they can be transformed into each other through bending, twisting, and stretching, without tearing or gluing.