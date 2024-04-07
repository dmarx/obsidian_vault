see also:
- [[Homotopy Groups]]

Homotopy is a central concept in [[topology]], a branch of mathematics concerned with the properties of space that are preserved under continuous transformations. The notion of homotopy provides a formal way to understand when two mathematical objects can be considered "equivalent" or "the same" in a topological sense, by allowing one object to be continuously deformed into another. This concept is foundational not only in topology but also in areas of mathematics and physics where the idea of continuous deformation is relevant, such as in the study of [[Homotopy Type Theory]] and [[Algebraic Topology]].

### Formal Definition

Two continuous functions $f, g: X \rightarrow Y$ between topological spaces $X$ and $Y$ are said to be **homotopic** if there is a continuous function $H: X \times [0, 1] \rightarrow Y$ (called a homotopy) such that for every point $x \in X$:
- $H(x, 0) = f(x)$
- $H(x, 1) = g(x)$

The function $H$ provides a continuous path of points in $Y$ for each point in $X$, showing how $f(x)$ can be continuously transformed into $g(x)$. The parameter in $[0, 1]$ often represents "time," with $H(x, t)$ showing the intermediate stages of the transformation from $f$ to $g$.

### Importance and Applications

- **[[Topological Invariants|Topological Invariance]]**: Homotopy is a way of classifying spaces and maps up to deformation, which is more flexible than rigid geometric shapes. Two spaces that are homotopy equivalent (there exist continuous maps between them that are homotopic to the identity map) share many topological properties, such as their fundamental groups and higher homotopy groups.

- **[[Fundamental Group]]**: The set of all loops (closed paths) at a point in a space, modulo homotopy, forms a group structure known as the fundamental group. This group captures information about the space's "holes" or loops that cannot be contracted to a point.

- **Higher Homotopy Groups**: While the fundamental group deals with loops, higher homotopy groups generalize this idea to spheres of higher dimensions, providing further information about the space's structure.

- **[[Homotopy Type Theory]]**: In HoTT, homotopy is a key idea, where types are viewed as spaces and equalities as paths. This leads to a rich interplay between logic, mathematics, and computer science, offering new ways to think about proofs, programs, and constructions in mathematics.

### Homotopy vs. [[Isotopy]]

It's worth noting the distinction between homotopy and isotopy, another concept of equivalence. Isotopy is a stricter form of equivalence applicable in differential topology and geometry, where the deformation between objects must preserve not just the continuity but also the smooth structure of the space. In contrast, homotopy requires only continuity, making it a more general notion.

Homotopy provides a powerful lens through which to understand and classify spaces based on their essential shape, rather than their precise geometric details, reflecting the core idea in topology that sometimes, being "essentially the same" is more significant than being "exactly the same."