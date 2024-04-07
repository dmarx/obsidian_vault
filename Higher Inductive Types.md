see also:
- [[Homotopy]]
- [[Homotopy Groups]]
- [[Homotopy Theory]]

[[Higher Inductive Types]] (HITs) are a sophisticated concept in the realm of [[Homotopy Type Theory]] (HoTT), extending traditional inductive types to incorporate higher-dimensional structures. They are pivotal in representing spaces and constructions that are common in [[Algebraic Topology]] within the type-theoretical framework. HITs enable the encoding of not just points (0-dimensional objects) but also paths (1-dimensional objects), homotopies between paths (2-dimensional objects), and higher-dimensional analogs, directly within types. This capacity significantly enriches the expressiveness of [[type theory]], especially for mathematical and computational applications that involve complex spatial and equivalence relations.

### Basic Concepts

To understand HITs, it's useful to first grasp traditional inductive types. An [[inductive type]] is defined by specifying its constructors, which can be thought of as ways to build instances (or "terms") of that type. For example, the natural numbers can be defined inductively with two constructors: one for the number zero and another for the successor function, which takes a natural number to its successor.

HITs extend this concept by including constructors for paths, which represent equalities or equivalences between terms, as well as higher-dimensional paths (homotopies) that relate these paths. This capability allows HITs to express complex mathematical objects and relationships directly.

### Formal Definition

In formal terms, a higher inductive type might include:

- **Point constructors**, similar to the constructors of traditional inductive types, which define the points (0-cells) of the space.
- **Path constructors**, which specify paths (1-cells) between points, representing equalities or equivalences.
- **Higher path constructors**, which define homotopies (2-cells) between paths, and so on, potentially up to arbitrary dimensions. These higher paths express relations between relations (i.e., equivalences between equivalences).

An example of a higher inductive type is the circle, $S^1$, which can be defined with:

- A point constructor, say $base : S^1$, giving a base point on the circle.
- A path constructor, say $loop : base = base$, which represents a path from the base point back to itself, effectively tracing the circle.

### Examples and Applications

- **The Circle $S^1$**: As mentioned, the circle can be defined as a HIT with a single base point and a loop path that connects this point to itself.

- **[[Suspension (type theory)|Suspension]]**: Given a type $A$, the suspension $\Sigma A$ is a HIT that forms a sphere by connecting all points of $A$ to two distinct points, north and south poles, essentially stretching $A$ into a spherical shape.

- **[[Cell Complexes]]**: HITs can define cell complexes used in algebraic topology, representing spaces constructed by attaching cells (of various dimensions) together in specific ways.

### Implications for Homotopy Type Theory

HITs are crucial for HoTT because they allow the representation of homotopical and topological concepts directly within type theory, bridging the gap between abstract mathematical structures and computational frameworks. This capability is essential for leveraging the full power of HoTT in both mathematical reasoning and in the design and verification of computer systems.

- **Mathematical Expressiveness**: HITs provide a language for expressing complex mathematical ideas, such as [[Homotopy Groups]] and [[cohomology]], in the precise and formal setting of [[type theory]].

- **Proof Assistants**: In computational logic and the development of proof assistants, HITs enable the encoding and manipulation of sophisticated mathematical objects, facilitating proofs and constructions that were previously challenging or infeasible.

- **Foundational Insights**: By incorporating higher-dimensional paths and equivalences, HITs offer new insights into the nature of equality and equivalence in mathematics, highlighting the rich structure and relationships that exist between mathematical objects.

Higher Inductive Types represent a profound expansion of type theory's capacity to model mathematical reality, providing a flexible and powerful tool for both theoretical exploration and practical application.