Homotopy groups are fundamental concepts in algebraic topology, providing a powerful algebraic tool to study and classify topological spaces based on their higher-dimensional loop structures. These groups encapsulate information about how spaces can be continuously deformed, offering insights into the spaces' intrinsic topological properties.

### [[Fundamental Group]] (First Homotopy Group)

The **fundamental group** or the first homotopy group, denoted as $\pi_1(X, x_0)$, is the group of loops based at a point $x_0$ in a space $X$, where two loops are considered equivalent if one can be continuously deformed into the other (homotopy). This group captures information about the space's 1-dimensional hole structures. For example, the fundamental group of a circle $S^1$ is isomorphic to $\mathbb{Z}$, the set of integers, reflecting the fact that loops around the circle can wind around any number of times in either direction.

### Higher Homotopy Groups

Higher homotopy groups, denoted $\pi_n(X, x_0)$ for $n > 1$, generalize the concept of the fundamental group to $n$-dimensional spheres. $\pi_n(X, x_0)$ consists of the equivalence classes of maps from the $n$-dimensional sphere $S^n$ into $X$ that fix a base point $x_0$. Like the fundamental group, two such maps are considered equivalent if there exists a continuous family of maps between them, keeping the base point fixed.

- **Second Homotopy Group $\pi_2(X, x_0)$**: This group captures information about "holes" that can trap 2-dimensional spheres. For instance, $\pi_2(S^2) \cong \mathbb{Z}$, indicating that the 2-sphere has a single type of "hole" that can be wrapped around itself in a quantifiable way.

- **Higher Groups $\pi_n(X, x_0)$ for $n > 2$**: These explore the space's structure concerning $n$-dimensional spheres. The higher the value of $n$, the more subtle and complex the captured features of $X$.

### Properties and Applications

- **[[Abelian Groups]]**: While the fundamental group $\pi_1$ may be non-Abelian, all higher homotopy groups $\pi_n$ for $n > 1$ are Abelian. This reflects the fact that, in higher dimensions, the way loops (or spheres) wrap around each other doesn't matter in terms of the group operation.

- **[[Topological Invariants]]**: Homotopy groups are topological invariants, meaning they are preserved under homeomorphisms (continuous deformations with continuous inverses). They provide a way to classify spaces up to homotopy equivalence, a weaker condition than homeomorphism that still preserves much of the spaces' qualitative structure.

- **Calculating Homotopy Groups**: Computing these groups can be highly nontrivial, especially for higher $n$. The fundamental group $\pi_1$ is often the easiest to determine. For certain spaces like spheres, some homotopy groups are known, but for others, the groups remain a subject of active research.

- **Applications**: Homotopy groups have applications across mathematics and physics. In topology, they are used to prove important theorems like the [[Brouwer Fixed Point Theorem]] and the [[Poincare Conjecture|Poincaré Conjecture]] (for $\pi_2$). In physics, they help in the study of [[topological defects]] in materials and the classification of phases of matter in condensed matter physics.

Homotopy groups offer a window into the "shape" of spaces beyond the reach of intuition, revealing the deep and often surprising structure underlying seemingly simple spaces.