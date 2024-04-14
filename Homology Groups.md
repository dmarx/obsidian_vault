---
tags:
  - sod/gold
  - needs-outlinks
aliases:
  - homology
---

Homology is a fundamental concept in algebraic topology, providing a systematic way to study and classify topological spaces based on their shapes and the "holes" within those shapes. The essence of homology is to associate a sequence of algebraic objects, typically [[Abelian Groups]] or [[Vector Space|vector spaces]], with a topological space in such a way that these algebraic invariants reflect the space's topological structure. Homology groups are powerful tools for distinguishing between different types of topological spaces and for understanding their properties in an algebraic manner.

### Definitions and Concepts

The homology groups of a space are denoted $H_n(X)$, where $X$ is the space in question and $n$ is a non-negative integer representing the dimension. Intuitively:

- $H_0(X)$ describes the connected components of $X$.
- $H_1(X)$ captures information about loops in $X$ that do not bound a surface (1-dimensional holes).
- $H_2(X)$ relates to surfaces in $X$ that do not bound a volume (2-dimensional holes).
- Higher homology groups $H_n(X)$ for $n > 2$ generalize this notion to $n$-dimensional holes.

### Construction

Homology groups are constructed through a process involving chains, boundaries, and cycles:

1. **[[Chains]]**: A chain is a formal sum of $n$-dimensional simplices (for [[simplicial homology]]) or $n$-dimensional cells (for [[cellular homology]]) in $X$. The set of all such chains forms a group called the chain group, denoted $C_n(X)$.

2. **Boundaries**: The boundary of an $n$-dimensional [[simplex]] is the collection of its $(n-1)$-dimensional faces. This concept extends to chains, yielding the [[boundary operator]] $\partial_n: C_n(X) \rightarrow C_{n-1}(X)$, which maps each chain to its [[boundary chain]].

3. **[[Cycles]] and Boundaries**: A cycle is a chain whose boundary is zero. A boundary is a chain that is the boundary of some higher-dimensional chain. The cycles form a subgroup $Z_n(X)$ of $C_n(X)$, and the boundaries form a subgroup $B_n(X)$ of $Z_n(X)$.

4. **Homology Groups**: The $n$th homology group, $H_n(X)$, is the quotient group $Z_n(X) / B_n(X)$, representing cycles that are not boundaries of $(n+1)$-dimensional chains. Elements of $H_n(X)$ are called homology classes, and each class represents an [[equivalence class]] of cycles that differ by a boundary.

### Properties and Applications

- **[[Topological Invariants]]**: Homology groups are topological invariants, meaning they are preserved under homeomorphisms. Spaces that are homeomorphic have isomorphic homology groups.

- **[[Betti Numbers]]**: The rank of the $n$th homology group, denoted $\beta_n$, is called the $n$th Betti number. Betti numbers provide a count of $n$-dimensional holes in a space.

- **[[Euler Characteristic]]**: The Euler characteristic, a fundamental topological invariant, can be computed from the Betti numbers as $\chi(X) = \sum_{n=0}^{\infty} (-1)^n \beta_n$.

- **Applications**: Beyond pure mathematics, homology theory finds applications in various fields, including computer science (in [[topological data analysis]] and [[persistent homology]]), physics (in the study of topological phases of matter), and biology (in the analysis of the shapes and structures of molecules).

Homology offers a bridge between the geometric intuition about spaces and the rigor of algebraic formalism, making it an indispensable tool in the study of [[topological space|topological spaces]].

---

Homology groups are central algebraic structures in [[algebraic topology]] that provide a systematic way to quantify the topological features of a space, such as holes, voids, and disconnected components. They serve as [[algebraic invariants]] that can help classify and compare topological spaces based on their structure. Understanding homology groups involves constructing sequences of abelian groups or modules associated with a topological space and using these groups to capture essential topological information in an algebraic form.

### Construction of Homology Groups

The construction of homology groups generally follows a sequence of steps involving [[simplicial complexes]], [[singular simplices]], or [[cell complexes]], depending on the context and the specific type of homology being considered (e.g., simplicial homology, singular homology, cellular homology).

1. **Chains**: A chain is a formal sum of basic building blocks (like simplices or cells) with integer coefficients. The set of all such chains of dimension $n$ forms a group called the chain group, denoted $C_n$.

2. **Boundary Operator**: For each chain, a boundary operator $\partial_n: C_n \rightarrow C_{n-1}$ defines how to obtain the $(n-1)$-dimensional boundary of an $n$-dimensional chain. This operator is crucial for distinguishing between different types of topological features.

3. **Cycles and Boundaries**: A cycle is an $n$-dimensional chain whose boundary is zero, and a boundary is a chain that can be expressed as the boundary of some higher-dimensional chain. Cycles form a subgroup $Z_n \subseteq C_n$, and boundaries form a subgroup $B_n \subseteq Z_n$.

4. **Homology Groups**: The $n$-th homology group $H_n$ is defined as the quotient group $Z_n / B_n$. Intuitively, this group measures the $n$-dimensional holes in the space that are not merely boundaries of $(n+1)$-dimensional features.

### Features of Homology Groups

- **Betti Numbers**: The rank (or the number of generators) of the $n$-th homology group, denoted $\beta_n$, is known as the $n$-th Betti number. It gives a count of $n$-dimensional holes in the space.

- **Torsion Coefficients**: In addition to the Betti numbers, homology groups can also have torsion components, which provide information about how certain cycles wrap around holes in a non-trivial way.

- **Euler Characteristic**: The alternating sum of Betti numbers yields the Euler characteristic of the space, a scalar invariant that offers insight into the space's overall shape.

### Types of Homology

- **[[Simplicial Homology]]**: Applied to spaces that can be divided into simplices, where simplices are basic building blocks like points, line segments, triangles, etc.

- **[[Singular Homology]]**: More general and widely applicable, singular homology deals with continuous mappings from standard simplices into a topological space, allowing for the study of any space that can be described topologically.

- **[[Cellular Homology]]**: Used for spaces constructed from cells (e.g., [[CW complexes]]), offering a more computationally efficient way to compute homology in many cases.

### Applications

Homology groups have found applications in various areas of mathematics and science:

- **Topological Data Analysis (TDA)**: In analyzing high-dimensional data sets to identify shapes and features.
- **Quantum Field Theory**: In understanding the properties of space and fields.
- **Molecular Biology**: In studying the 3D structures of molecules, including DNA and proteins.
- **Robotics and Path Planning**: In understanding the configuration space of robotic systems.

Homology groups illuminate the underlying topological structure of spaces, providing a powerful tool for distinguishing between spaces that might otherwise seem similar, and offering insights into their more subtle properties.