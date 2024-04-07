see also:
- [[Orthogonality]]

Orthogonality relations for the characters of irreducible representations of finite groups are among the most powerful tools in character theory, providing deep insights into the structure of groups and their representations. These relations derive from the [[inner product]] of characters, defined in a way that reflects the [[Symmetry|symmetries]] and structure inherent in the group.

### Inner Product of Characters

Given two characters $\chi$ and $\psi$ of a finite group $G$, the inner product of $\chi$ and $\psi$ is defined as
$$
\langle \chi, \psi \rangle = \frac{1}{|G|} \sum_{g \in G} \chi(g) \overline{\psi(g)},
$$
where $|G|$ is the order of the group, and the bar denotes complex conjugation. This definition is designed so that the characters, viewed as functions on the group, are orthogonal under this inner product if they correspond to different irreducible representations.

### Orthogonality Relations

The orthogonality relations come in two main flavors: relations between characters of different irreducible representations (inter-representation orthogonality) and relations between characters within the same irreducible representation (intra-representation orthogonality).

- **Inter-representation Orthogonality**: For irreducible characters $\chi$ and $\psi$ corresponding to different irreducible representations of $G$, we have
$$
\langle \chi, \psi \rangle = 0.
$$
This states that the characters of distinct irreducible representations are orthogonal with respect to the defined inner product.

- **Intra-representation Orthogonality**: For an irreducible character $\chi$ of $G$, the inner product of $\chi$ with itself is
$$
\langle \chi, \chi \rangle = 1.
$$
This indicates that each irreducible character is "normalized" in a sense, having unit length under this inner product.

### Consequences and Applications

- **Counting Irreducible Representations**: The orthogonality relations imply that the number of distinct irreducible representations of a finite group $G$ (up to isomorphism) is equal to the number of its conjugacy classes. This provides a direct method for determining the "size" of the group's representation theory from its algebraic structure.

- **Decomposing Representations**: The orthogonality relations enable the decomposition of any representation of $G$ into its irreducible components. Specifically, if $\chi$ is the character of some representation, the multiplicity of the irreducible representation with character $\psi$ in this decomposition is given by $\langle \chi, \psi \rangle$.

- **Character Tables**: The orthogonality relations are instrumental in constructing character tables, which encapsulate the characters of all irreducible representations of $G$ evaluated on each conjugacy class. These tables are a compact and powerful tool for studying the group's properties and the behavior of its representations.

- **Fourier Analysis on Groups**: The principles underlying the orthogonality relations of characters resemble those of Fourier analysis, where characters play the role of basis functions, and representations can be analyzed in terms of these basis functions. This analogy extends the utility of Fourier analysis to abstract group structures, providing a method for analyzing functions defined on groups.

The orthogonality relations for characters illuminate the deep structure of finite groups and their representations, serving as a foundational aspect of character theory and representation theory at large.