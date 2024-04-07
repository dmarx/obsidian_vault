Burnside's lemma, also known as Burnside's counting theorem or the orbit-counting theorem, is a powerful result in group theory and [[combinatorics]] that provides a method for counting the number of orbits in a group action. Named after William Burnside, a pioneer in the [[theory of finite groups]], this lemma bridges the study of [[group actions]] with combinatorial enumeration, offering a formula that relates the sizes of orbits and stabilizers within a finite group action.

### Statement of Burnside's Lemma

Let $G$ be a finite group acting on a set $X$. An **[[orbit]]** of an element $x \in X$ under the action of $G$ is the set $\{g \cdot x | g \in G\}$, and a **[[stabilizer]]** (or **[[isotropy subgroup]]**) of $x$ is the set $\{g \in G | g \cdot x = x\}$. Burnside's lemma states that the number of distinct orbits, denoted as $|X/G|$, is given by the average number of [[fixed points]] under the elements of $G$, formally expressed as:
$$
|X/G| = \frac{1}{|G|} \sum_{g \in G} |\text{Fix}(g)|,
$$
where $|\text{Fix}(g)|$ denotes the number of elements in $X$ fixed by the group element $g$ (i.e., $g \cdot x = x$ for $x \in \text{Fix}(g)$).

### Intuition and Applications

- **Intuition**: The lemma offers a way to count orbits without having to enumerate them directly. It essentially says that to find the number of orbits, one can average the counts of points in $X$ that remain unchanged (fixed) under the action of each element of $G$.

- **Applications**: Burnside's lemma is widely used in combinatorial problems involving [[symmetry]], such as counting the number of distinct colorings of objects under rotational or reflective symmetries, enumerating the number of necklaces with beads of different colors, and solving puzzles where the arrangement of pieces is subject to symmetry constraints.

### Example: Coloring Problem

Consider a simple example where $G$ is a group of rotations acting on a set $X$ of colorings of the vertices of a square, with two colors available (say, red and blue). Using Burnside's lemma, one can count the number of colorings up to rotation by examining each group element's fixed points: the identity rotation (which fixes all colorings), a 180-degree rotation (which fixes colorings that are symmetric across the square's center), and two 90-degree rotations (each fixing only the uniformly colored squares). Calculating the average number of fixed points over these rotations gives the number of distinct colorings under the action of $G$.

### Importance

Burnside's lemma is fundamental in both theoretical and applied mathematics. It exemplifies how group theory concepts can be applied to count and classify combinatorial arrangements, providing a bridge between abstract algebra and practical enumeration problems. Beyond its direct applications, the lemma also enriches the understanding of symmetry and its implications in various mathematical contexts, from geometry to algebraic topology.