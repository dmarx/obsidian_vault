---
tags:
  - needs-outlinks
  - sod/gold
---

see also:
- [[Taylor Series]]
- [[Taylor Expansion]]

Jet spaces are a sophisticated concept in [[differential geometry]] and [[algebraic geometry]] that generalize the notion of derivatives of functions between [[manifolds]], capturing the behavior of functions and their derivatives up to a certain order. The formalism of jet spaces provides a unified and powerful framework for studying the local behavior of [[mappings]], including [[singularities]] and [[differential equations]], from a geometric perspective.

### Basic Concepts

- **[[Jet]]**: Informally, the $k$-jet of a smooth function at a point encapsulates all the derivative information of the function up to order $k$ at that point. For functions between manifolds, this includes not just the values of derivatives but also the geometric relationship between the source and target manifolds.

- **Jet Space**: For a given manifold $M$, the $k$-jet space at a point $x \in M$, denoted as $J^k(M, \mathbb{R})$ (or more generally $J^k(M, N)$ for functions from $M$ to another manifold $N$), is the space of $k$-jets of functions at $x$. The entirety of $k$-jet spaces over $M$ forms a bundle over $M$, known as the jet bundle.

### Formal Definition

Let $M$ and $N$ be smooth manifolds, and consider smooth maps $f, g: M \to N$. The maps $f$ and $g$ are said to have the same $k$-jet at $x \in M$ if, in some (and hence any) local coordinate system around $x$ in $M$ and $f(x)$ in $N$, all partial derivatives of $f$ and $g$ of order up to $k$ agree at $x$. The equivalence class of all maps having the same $k$-jet at $x$ is denoted as $j^k_x f$ and represents a point in the jet space $J^k(M, N)$.

### Properties and Uses

- **[[Differential Equations]]**: Jet spaces are particularly useful in the study of differential equations, where solutions can be considered as sections of an appropriate jet bundle. The geometric structure of jet spaces allows for the elegant formulation and analysis of both ordinary and partial differential equations.

- **[[Singularities]] and [[Stability]]**: The framework of jet spaces provides tools for analyzing the stability of mappings and the structure of their singularities. By examining how jets extend or do not extend to higher orders, one can study the deformation and unfolding of singularities.

- **Symmetries and [[Conservation Laws]]**: In the context of physics, jet spaces are instrumental in the modern geometric formulation of symmetries and conservation laws, notably in the context of [[Noether's theorem]] and the theory of [[variational principles]].

### Examples

- **First-Order Jets**: The first-order jet space of functions from $\mathbb{R}$ to $\mathbb{R}$ at a point captures the value of the function and its first derivative at that point. This is analogous to the tangent space but includes the function's value as well.

- **Higher-Order Jets**: For a map $f: \mathbb{R}^n \to \mathbb{R}^m$, a $k$-jet includes information equivalent to all partial derivatives of $f$ up to order $k$, providing a rich geometric object that encapsulates the behavior of $f$ and its approximations up to that order.

### Mathematical Formalism and Challenges

Developing a comprehensive theory of jet spaces involves advanced techniques from differential geometry, including the theory of [[fiber bundles]] and [[connections]]. The construction and analysis of [[jet bundles]] require a deep understanding of local and global [[differential topology]], as well as the algebraic structure of [[differential operators]]. Moreover, the study of how jet spaces relate to the properties of differential equations and singularities brings in tools from algebraic geometry and [[singularity theory]], making the theory of jet spaces a rich and multifaceted area of modern mathematics.