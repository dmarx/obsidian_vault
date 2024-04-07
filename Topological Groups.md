Topological groups form a central concept in mathematics, blending the structures of [[group theory]] with those of [[topology]]. A topological group is a group equipped with a [[Topology On A Set|topology]] that makes the group operations—namely, multiplication (or addition, for abelian groups) and inversion—continuous. This intertwining of algebra and topology allows for the study of groups in a geometric context, providing deep insights into their properties and behaviors.

### Definition

Formally, a topological group $G$ is a set equipped with both a group structure and a topological structure such that:
1. The group operation $\cdot : G \times G \to G$, defined by $(g, h) \mapsto g \cdot h$, is continuous with respect to the product topology on $G \times G$ and the topology on $G$.
2. The inversion operation $^{-1}: G \to G$, defined by $g \mapsto g^{-1}$, is continuous with respect to the topology on $G$.

These conditions ensure that topological group actions behave nicely in both an algebraic and topological sense, facilitating the study of groups using topological methods.

### Examples

- **The Real Numbers, $\mathbb{R}$**: With standard addition as the group operation and the usual topology, $\mathbb{R}$ forms an abelian topological group. This extends to $\mathbb{R}^n$ with vector addition.
- **The Unit Circle, $S^1$**: The set of complex numbers of absolute value 1, under multiplication, forms a topological group. It's a fundamental example in the study of compact topological groups.
- **The General Linear Group, $GL(n, \mathbb{R})$**: The group of all invertible $n \times n$ matrices over $\mathbb{R}$, with matrix multiplication as the group operation and the topology induced by viewing $GL(n, \mathbb{R})$ as a subset of $\mathbb{R}^{n^2}$, is a non-compact, non-abelian topological group.

### Properties and Applications

- **Homogeneity**: Every point in a topological group "looks" the same as every other point, in the sense that for any two points $g$ and $h$ in the group, there exists a homeomorphism of the group that maps $g$ to $h$. This stems from the group operation and the continuity requirements, making topological groups intrinsically [[homogeneous spaces]].

- **[[Haar Measure]]**: In locally compact topological groups, there exists a unique (up to a scalar multiple) translation-invariant measure known as the Haar measure. This measure is crucial for defining integrals over the group, leading to the development of [[Harmonic Analysis On Groups]].

- **[[Lie Groups]]**: A significant class of topological groups are Lie groups, which are smooth manifolds that allow for the study of group properties through differential geometry. Lie groups play a pivotal role in physics, especially in the study of symmetry and conservation laws.

### Significance

Topological groups are foundational in various areas of mathematics and physics. They are essential in the study of symmetry, mathematical analysis, algebraic topology, and quantum mechanics, among other fields. The interplay between the algebraic structure of groups and the geometric structure of topology allows for a rich theory with both theoretical and practical applications, illuminating the structure of spaces and the behavior of symmetries in mathematical and physical systems.