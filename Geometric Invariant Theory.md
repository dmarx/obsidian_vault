---
tags:
  - sod/gold
  - needs-outlinks
---

Geometric Invariant Theory (GIT) is a fundamental area of mathematics that lies at the intersection of [[algebraic geometry]], [[group theory]], and [[representation theory]]. Introduced by [[David Mumford]] in the 1960s, GIT provides a rigorous framework for studying the actions of groups on algebraic varieties and constructing quotients of these actions, especially when the groups are reductive (a class of groups that includes, for example, all finite groups and many important Lie groups). The theory is essential for understanding the [[moduli spaces]] of algebraic varieties, which are spaces parameterizing families of algebraic objects up to some [[equivalence relation]].

### Core Concepts and Goals

- **[[Group Actions|Group Action]]**: In the context of GIT, one considers the action of a group $G$ on an algebraic variety $X$, which intuitively means that $G$ "moves points" of $X$ around in a way that respects the algebraic structure of both $G$ and $X$.

- **Quotients**: One of the central problems GIT addresses is how to construct a "good" [[quotient space]] $X//G$, representing the orbit space of the action (i.e., a space whose points correspond to orbits of $G$ acting on $X$). In general, forming quotients in the algebraic setting is fraught with difficulties, especially when the action has orbits of different dimensions.

- **[[Stability Under Group Action|Stability]]**: A key concept in GIT is the notion of stability, which classifies points of $X$ into stable, semistable, and unstable points under the $G$-action. Stability is crucial for determining which points of $X$ can be "nicely" quotiented out by the group action.

### Applications and Importance

- **Moduli Spaces**: GIT is instrumental in the construction of moduli spaces, which are geometric spaces that classify mathematical objects (such as algebraic curves, vector bundles, or sheaves) according to some equivalence relation. Moduli spaces are central objects in algebraic geometry and string theory.

- **Symplectic Reduction**: GIT has a counterpart in symplectic geometry, known as [[symplectic reduction]], which constructs quotient spaces for actions of Lie groups on symplectic manifolds. This connection provides deep links between algebraic geometry and mathematical physics, especially in the study of phase spaces in classical mechanics and gauge theory in quantum field theory.

- **[[Invariant Theory]]**: GIT extends classical invariant theory by providing methods to construct quotients by group actions in settings where traditional methods fail, particularly for non-finite groups. It helps in understanding the structure of invariants and orbit spaces for these actions.

### Methods and Techniques

- **[[Mumford's Numerical Criteria]]**: Mumford provided numerical criteria for stability in terms of linearized group actions, which can be used to determine whether a point is stable, semistable, or unstable. These criteria are fundamental for the practical application of GIT.

- **Construction of Quotients**: GIT employs sophisticated methods from algebraic geometry to construct quotients, involving sheaves, line bundles, and ample line bundles on varieties, and uses these to define quotients as projective varieties or schemes.

- **Examples and Classifications**: GIT has been used to study and classify various geometric objects, including toric varieties, algebraic surfaces, and configurations of points on projective spaces. It also plays a crucial role in the geometric Langlands program, a research area connecting number theory, representation theory, and algebraic geometry.

Geometric Invariant Theory is a vibrant and rich field of study, intertwining deep theoretical insights with practical tools for understanding the geometry and algebra of group actions on spaces. Its development has had a profound impact on modern mathematics, influencing areas as diverse as algebraic geometry, mathematical physics, and the theory of moduli spaces.

>A key concept in GIT is the notion of stability, which classifies points of $X$ into stable, semistable, and unstable points under the $G$-action.

In Geometric Invariant Theory (GIT), the concepts of stability, semistability, and instability play crucial roles in understanding the quotient construction of algebraic varieties under group actions. These concepts help in determining which points in a variety under the action of a group $G$ can be considered equivalent, and they facilitate the formation of "good" quotient spaces that retain geometric and algebraic structure.

### Stability

- **Stable Points**: A point $x \in X$ is said to be **stable** under the action of $G$ if its orbit under $G$ is closed (in the Zariski topology), has finite stabilizer, and the orbit represents an open subset in the quotient space. Stable points lead to a well-behaved geometric structure in the quotient, allowing for the construction of geometric objects like moduli spaces.

### Semistability

- **Semistable Points**: A point $x \in X$ is **semistable** if it does not meet the strict criteria for stability but still can be included in the quotient space in a meaningful way. Specifically, a point is semistable if there exists a limit point in its closure under the $G$-action that is stable. Semistable points are crucial for ensuring that the quotient space is compact or complete, an important property for many applications in algebraic geometry.

### Unstable Points

- **Unstable Points**: Points that are not semistable are considered **unstable**. These points are omitted from the quotient construction because their orbits under $G$ do not lend themselves to a nice geometric interpretation. Unstable orbits either do not close or do not contain a stable point in their closure, making them unsuitable for forming quotients that have good geometric properties.

### Mumford's Numerical Criterion

David Mumford provided a numerical criterion for determining the stability and semistability of points, which involves checking certain conditions related to line bundles and their associated Hilbert-Mumford numerical invariants. This criterion is especially useful for practical computations and theoretical considerations in algebraic geometry.

### Applications of Stability Concepts

- **Moduli Spaces**: In constructing moduli spaces, such as those classifying algebraic curves or vector bundles, the stability of objects being classified is a key consideration. Stable objects correspond to points in the "interior" of the moduli space, while semistable objects may correspond to boundary points.

- **Quotients and GIT**: The quotient space $X//G$, formed from the semistable points of $X$ under the $G$-action, retains significant geometric and algebraic information about the original space $X$ and the group action. This quotient space is central to many investigations in algebraic geometry and theoretical physics.

- **Symplectic Reduction and Physics**: The concepts of stability and semistability also find parallels in symplectic geometry and theoretical physics, particularly in the study of gauge theories and the geometric quantization process.

The classification of points into stable, semistable, and unstable categories under group actions provides a powerful framework for analyzing and constructing spaces with rich geometric structure, illustrating the deep interplay between group actions, algebraic geometry, and representation theory in GIT.

---

In Geometric Invariant Theory (GIT), the concepts of stability, semistability, and instability are central to understanding the quotient construction when a group $G$ acts on an algebraic variety $X$. These notions help to categorize the points of $X$ based on their behavior under the group action, facilitating the formation of "good" quotients, which are geometric spaces that capture the essence of the $G$-action on $X$ in a coherent and structured manner.

### Stability, Semistability, and Instability

- **Stable Points**: A point $x \in X$ is considered stable if the orbit $G \cdot x$ under the action of $G$ is closed (in the Zariski topology) and the stabilizer of $x$ in $G$ (the set of elements in $G$ that fix $x$) is finite. Intuitively, stable points have "well-behaved" orbits that do not approach the orbits of other points, allowing them to be nicely represented in the quotient space.

- **Semistable Points**: A point $x \in X$ is semistable if its orbit closure (the closure of $G \cdot x$) intersects the set of stable points. Semistable points may have orbits that come arbitrarily close to other orbits, but they can still be included in the quotient in a meaningful way, often by identifying points whose orbits share common closure points.

- **Unstable Points**: Points that are not semistable are considered unstable. The orbits of unstable points do not lend themselves to forming a good geometric quotient, as they cannot be separated nicely in the quotient space. Unstable points are often excluded from the quotient construction.

### The Quotient Space $X//G$

The quotient space $X//G$, also known as the GIT quotient, is constructed using the semistable points of $X$. It represents the space of orbits of the $G$-action, with certain identifications made among the orbits of semistable points to ensure that the quotient is well-defined and geometrically meaningful. The quotient space captures the "essence" of the $G$-action on $X$, abstracting away the details of individual orbits to focus on the overall structure imposed by the action.

### Mumford's Numerical Criterion

David Mumford provided a numerical criterion for determining the stability and semistability of points in $X$ with respect to a linearized $G$-action. This criterion is particularly useful when $G$ is a reductive group and the action is linearized, meaning it is lifted to an action on a line bundle over $X$. The criterion involves checking certain conditions related to the weights of the $G$-action on the fibers of the line bundle, offering a practical way to identify stable and semistable points.

### Applications and Significance

- **Moduli Spaces**: Stability conditions are crucial in constructing moduli spaces as GIT quotients, where each point in the moduli space represents an equivalence class of geometric objects (e.g., curves, surfaces) under the action of a group (e.g., changes of coordinates).

- **[[Symplectic Geometry]]**: In symplectic geometry, analogous concepts of stability arise in the context of symplectic reduction, showing a deep connection between GIT and Hamiltonian dynamics.

- **Algebraic Geometry and Beyond**: GIT and its stability criteria have profound implications in algebraic geometry, providing tools to study geometric objects under group actions and contributing to the understanding of vector bundles, algebraic curves, and more complex structures.

The concepts of stability, semistability, and instability in GIT provide a nuanced and powerful language for analyzing and constructing quotients under group actions, highlighting the interplay between algebraic geometry and group theory in the study of geometric structures.

---

[[Geometric Invariant Theory|Geometric Invariant Theory (GIT)]] is a sophisticated area of algebraic geometry that deals with the action of a group on a variety of algebraic structures. It provides a method for constructing "quotients" of algebraic varieties by group actions, particularly in contexts where traditional quotient constructions (like topological or differential quotients) do not make sense algebraically. Developed primarily by [[David Mumford]] in the 1960s, GIT is instrumental in moduli theory and the study of algebraic stacks.

### Key Concepts of GIT

#### Group Actions
In GIT, a *group action* is a formal way in which a group $G$ interacts with an algebraic variety $X$. Specifically, for each element $g \in G$, there is a corresponding automorphism of $X$ (i.e., a bijective morphism from $X$ to itself that respects the algebraic structure). The group action is typically denoted as $g \cdot x$, where $x \in X$.

#### Stability
A central notion in GIT is the concept of stability, which determines which points in a variety can be considered to form a "good" quotient. Stability is defined with respect to a linearization of the group action, often involving a line bundle over the variety. Points can be classified into types:
- **Stable points** ($x \in X^{s}$): Points that admit a well-behaved quotient under the group action and have finite stabilizers.
- **Semistable points** ($x \in X^{ss}$): Points that may be included in a quotient space in some meaningful way, though possibly in a more degenerate form than stable points.
- **Unstable points** ($x \in X^{us}$): Points that cannot be included in a quotient.

The precise definitions of these depend on the choice of a linearization, and different choices can lead to different notions of stability.

#### Quotients
The GIT quotient, denoted $X /\!\!/ G$, is constructed using the set of semistable points $X^{ss}$. This quotient is a projective variety that represents an "algebraic" category-theoretical quotient of $X^{ss}$ by the equivalence relation induced by $G$. Notably, the GIT quotient is not just a set-theoretic quotient but rather a quotient in the category of schemes, which respects the underlying algebraic geometry.

### Mathematical Formalism
Mathematically, GIT can be understood through the lens of invariant theory and ring theory. If $k[X]$ denotes the ring of regular functions on $X$, and $G$ acts on $X$, then $G$ induces an action on $k[X]$. The [[Invariant Ring]] $k[X]^G$ consists of all functions in $k[X]$ that are invariant under the action of $G$. The spectrum of this ring, $\operatorname{Spec}(k[X]^G)$, can be interpreted as the GIT quotient of $X$ by $G$ under suitable conditions.

### Applications and Importance
GIT is crucial in various branches of mathematics and theoretical physics, particularly in the construction of moduli spaces, where one needs to classify geometric objects up to some notion of equivalence. For example, in the study of vector bundles, algebraic curves, or complex manifolds, GIT provides a way to construct spaces that parametrize classes of these objects modulo some group action, typically arising from automorphisms.

In summary, GIT intertwines group theory, algebraic geometry, and the theory of linear algebraic groups to address the problem of forming quotients in a non-trivial algebraic setting. This interplay allows GIT to provide powerful tools for constructing and understanding moduli spaces in many areas of mathematics.