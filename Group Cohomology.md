---
aliases:
  - cohomology
---

see also:
- [[Geometric Group Theory]]
- [[Group Theory]]

Group cohomology is a mathematical framework that explores the properties and structures of groups using the tools of homological algebra. It provides a way to study group actions on modules (or more general abelian groups) and to understand the extensions, representations, and cohomological invariants of groups. Originating in algebraic topology, where it was used to study the topology of spaces with group symmetries, group cohomology has profound implications in various areas of mathematics and theoretical physics.

### Basic Concepts

- **Cohomology Groups**: For a group \(G\) acting on an [[Abelian Groups|abelian group]] \(A\) (considered as a \(G\)-module), the \(n\)-th cohomology group of \(G\) with coefficients in \(A\), denoted \(H^n(G, A)\), measures the obstructions to lifting \(n\)-1 cocycles to \(n\)-cocycles. These groups provide algebraic invariants that reflect both the structure of \(G\) and the nature of its action on \(A\).

- **Cochains, Cocycles, and Coboundaries**: The construction of cohomology groups involves defining cochains (functions from \(G^n\) to \(A\)), cocycles (cochains satisfying a certain condition that generalizes the notion of being closed), and coboundaries (cochains that can be expressed as the coboundary of another cochain). Cocycles that are not coboundaries represent nontrivial elements of cohomology groups.

### Significance and Applications

- **Extensions of Groups**: Group cohomology can be used to classify extensions of a group \(G\) by a \(G\)-module \(A\), where an extension is a group \(E\) fitting into an exact sequence \(0 \rightarrow A \rightarrow E \rightarrow G \rightarrow 0\). The second cohomology group \(H^2(G, A)\) parametrizes such extensions.

- **Representation Theory**: Cohomology groups, especially the first cohomology group, play a role in understanding and classifying the representations of \(G\) on various vector spaces or modules.

- **Obstructions and Deformations**: Higher cohomology groups often encode obstructions to certain deformations of structures, such as deformations of group actions or algebraic structures. For example, \(H^2(G, A)\) can provide information about the deformation of group representations.

- **Galois Cohomology**: In number theory, group cohomology is a key tool in Galois cohomology, where \(G\) is the Galois group of a field extension. It has applications in the study of number fields, algebraic varieties over fields, and the formulation of conjectures and theorems in arithmetic geometry, such as the Langlands program.

- **Topological and Geometric Applications**: In algebraic topology and geometric group theory, group cohomology connects the algebraic properties of fundamental groups with the topological properties of spaces, offering insights into the geometry and topology of manifolds and complexes associated with groups.

### Computational Aspects

Computing group cohomology can be challenging, especially for higher cohomology groups or for groups with complex actions on modules. Various techniques and algorithms have been developed, including spectral sequences and computer algebra systems, to aid in these computations.

Group cohomology remains a vibrant area of research with deep connections across mathematics. Its development has enriched our understanding of groups and their representations, provided tools for tackling problems in number theory and topology, and illuminated the connections between algebra and geometry.