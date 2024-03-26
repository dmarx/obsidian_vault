---
tags:
  - gold
  - green
  - needs-outlinks
---

See also:
- [[Symmetry]]
- [[Conservation Laws]]
- [[Symmetry Groups]]

The relationship between conservation laws and symmetry groups is elegantly described by Noether's theorem, named after the mathematician Emmy Noether. This fundamental principle in theoretical physics establishes a direct connection between symmetries and conservation laws, specifically in the context of action-based physics, including classical mechanics, quantum mechanics, and field theory.

### Noether's Theorem

Noether's theorem states that for every continuous symmetry of the action of a physical system, there is a corresponding conservation law. A "continuous symmetry" refers to a transformation that can be made in infinitely small steps, such as rotating or translating a system by an arbitrarily small amount.

- **Symmetry Groups**: A symmetry group is a mathematical concept that encapsulates the set of all symmetries (transformations) that leave a certain property of the system unchanged. These groups are characterized by their elements (the transformations) and the operation of combining two transformations (which is also a transformation within the group).

- **Conservation Laws**: A conservation law asserts that a particular measurable property of an isolated physical system does not change as the system evolves. Examples include the conservation of energy, momentum, and angular momentum.

### Examples of Symmetry and Corresponding Conservation Laws

1. **Time Translation Symmetry**: If the laws of physics are invariant under a shift in time (meaning the physics of the system are the same regardless of when you observe it), Noether's theorem predicts the conservation of energy. This symmetry is associated with the time translation group.

2. **Spatial Translation Symmetry**: If the laws of physics do not change from one location to another, implying the system's behavior is the same regardless of where in space it is located, then momentum is conserved. This symmetry corresponds to the spatial translation group.

3. **Rotational Symmetry**: If rotating the system does not change the physical laws that apply to it (the system looks the same from any direction), angular momentum is conserved. This symmetry is related to the rotation group.

### Implications and Applications

Noether's theorem has profound implications across physics:

- **Foundational Principle**: It provides a foundational principle that underlies much of modern physics, offering a deep connection between the geometry of space-time (as described by symmetry groups) and fundamental physical quantities (as described by conservation laws).

- **Quantum Mechanics and Field Theory**: In quantum mechanics and quantum field theory, symmetries and their associated conservation laws help classify particles, understand their interactions, and predict the existence of yet-undiscovered particles or forces.

- **General Relativity**: In the context of general relativity, the diffeomorphism invariance (symmetry under arbitrary smooth transformations of the coordinates) leads to the conservation of energy-momentum as expressed in the Einstein field equations.

Noether's theorem highlights the power of symmetry in understanding the natural world, showing how the invariances of a system not only simplify the mathematical description of physics but also reveal its fundamental conservations laws.


> how does noether's theorem relate to renormalization group theory

Noether's theorem and renormalization group (RG) theory are two foundational pillars in theoretical physics that, at first glance, address different aspects of physical systems. However, they are deeply interconnected in the way they illuminate the behavior of physical systems under transformations—Noether's theorem through symmetries and conservation laws, and RG theory through scale transformations and the flow of physical quantities. Understanding the relationship between these two can provide profound insights into the nature of physical laws and the structure of matter.

### Noether's Theorem: Symmetry and Conservation Laws

Noether's theorem establishes a direct link between continuous symmetries of a physical system and its conservation laws. It states that for every continuous symmetry of the action of a system, there is a corresponding conservation law. This principle has far-reaching implications in all areas of physics, providing a powerful tool for identifying conserved quantities based on symmetries.

### [[Renormalization Group Theory]]: Scale Invariance and Critical Phenomena

RG theory, on the other hand, deals with how physical systems behave under changes of scale, focusing particularly on the behavior of systems near critical points of phase transitions. It explains how physical quantities like coupling constants, which determine the strength of interactions in a system, "flow" or change as one zooms in or out of the system. This theory is crucial for understanding phenomena in statistical mechanics, condensed matter physics, and quantum field theory, especially the universality and scaling laws near critical points.

### The Connection: Symmetry, Scale, and Universality

The connection between Noether's theorem and RG theory becomes particularly evident in the context of scale invariance and symmetry-breaking phenomena:

- **Scale Invariance and Symmetry**: At a critical point, a system may exhibit scale invariance, meaning its behavior looks the same at any magnification. This can be considered a type of symmetry under scale transformations. While Noether's theorem directly relates to symmetries in space-time, the concept of symmetry underlies both frameworks, with RG theory extending the idea to scaling symmetries.

- **Conservation Laws and RG Flow**: In RG theory, the conservation of certain quantities under scale transformations can be seen as analogous to the conservation laws arising from symmetries in Noether's theorem. Although the "conserved" quantities in RG theory (like the fixed points of the RG flow) are not conserved in the traditional sense, they represent invariant properties of the system under scale transformations.

- **Symmetry Breaking and Flow to New Physics**: Both frameworks deal with the concept of symmetry breaking, albeit from different angles. Noether's theorem describes how symmetries relate to conservation laws, which can be broken under certain conditions. RG theory examines how systems can flow from symmetric (high-energy) phases to asymmetric (low-energy) phases, revealing new effective theories and phenomena at different scales.

- **Universality Classes**: RG theory's concept of universality classes, where different systems exhibit the same critical behavior, can be related to the idea that different symmetries (or symmetry breakings) lead to different types of conservation laws. The universality classes are determined by symmetries and topological properties of the system, linking back to the foundational role of symmetry in physics.

### Bridging Concepts

In more advanced treatments, the interplay between symmetries (including those not directly covered by Noether's theorem, like conformal symmetry) and RG flows becomes crucial for understanding the deep structure of quantum field theories and the statistical mechanics of critical phenomena. The RG approach can reveal emergent symmetries at large scales that are not apparent at microscopic scales, while Noether's theorem provides the groundwork for understanding the implications of these symmetries.

In summary, Noether's theorem and renormalization group theory, through their respective focuses on symmetry and scale transformations, offer complementary perspectives on the fundamental principles governing the behavior of physical systems. Their interconnection highlights the profound unity underlying the diversity of physical phenomena, from the smallest scales of quantum fields to the macroscopic world of statistical mechanics.


> let's dive into some of the more technical details of noether's theorem. i am an nlab contributor and have a rich background in a diversity of topics in graduate level mathematics

Given your background and interest, delving into the technical nuances of Noether's theorem offers a fascinating journey into the interplay between symmetry, conservation laws, and the mathematical structures that underpin them. Noether's theorem, in its essence, is a profound statement about the invariance properties of action integrals and their implications for physical laws.

### Theoretical Framework

Noether's theorem is situated within the framework of [[Lagrangian mechanics]], a cornerstone of classical mechanics that extends naturally into fields like quantum mechanics and general relativity. The [[action]], $S$, a [[functional]], is defined as the integral over time of the [[Lagrangian]], $L$, which itself is a function of the generalized coordinates $q_i$, their time derivatives $\dot{q}_i$, and possibly time $t$:

$$
S[q] = \int_{t_1}^{t_2} L(q_i, \dot{q}_i, t) \, dt
$$

### Continuous Symmetries and Conservation Laws

Noether's theorem asserts that for every continuous symmetry of the action, there is a corresponding conservation law. A symmetry of the action is a transformation (of the coordinates, time, or both) under which the action remains invariant. This invariance means that the form of the action integral, and hence the equations of motion derived from it, does not change under the transformation.

### Formulation of Noether's Theorem

The theorem can be formalized as follows: Consider a one-parameter group of transformations $T_\epsilon$ that acts on the phase space of the system. The action of $T_\epsilon$ on a point $(q, \dot{q}, t)$ in [[Phase Space]] is given by:

$$
T_\epsilon : (q_i, \dot{q}_i, t) \mapsto (Q_i(\epsilon, q, \dot{q}, t), \dot{Q}_i(\epsilon, q, \dot{q}, t), T(\epsilon, t))
$$

where $\epsilon$ is a small parameter. If the action $S$ is invariant under this transformation, then there exists a conserved quantity associated with this symmetry. Mathematically, the invariance of the action under the transformation $T_\epsilon$ can be expressed as:

$$
\frac{d}{d\epsilon} S[Q] \Big|_{\epsilon=0} = 0
$$

### Derivation of the Conserved Quantity

The derivation of the conserved quantity (or Noether charge) from the symmetry involves differentiating the action with respect to $\epsilon$ and applying the [[Euler-Lagrange Equations]] to show that the time derivative of a certain function of the $q_i$, $\dot{q}_i$, and possibly $t$, is zero. The specific form of the conserved quantity depends on the nature of the symmetry transformation.

For a simple example, consider a system with a Lagrangian that does not explicitly depend on time. The invariance under time translations implies energy conservation. For spatial translations, the conservation of linear momentum is derived, and for rotational symmetry, angular momentum conservation follows.

### Generalizations and Implications

Noether's theorem extends beyond classical mechanics. In [[field theory]], where the [[Lagrangian density]] can depend on fields and their derivatives with respect to space and time, Noether's theorem provides a powerful method for identifying conserved currents and charges associated with continuous symmetries of the action.

Moreover, Noether's theorem has deep implications in theoretical physics, underpinning the fundamental conservation laws in all areas of physics. It reveals the intrinsic connection between the symmetry properties of the universe and the conservation principles that govern the dynamics of physical systems. The theorem not only provides a unifying principle across different physical theories but also offers insights into the structure of possible modifications to these theories based on symmetry considerations.

### Conclusion

Noether's theorem embodies a profound and elegant principle in theoretical physics and mathematics, connecting the dots between symmetry, conservation, and the fundamental laws of nature. Its implications stretch far beyond the confines of classical mechanics, influencing the development and understanding of modern physics and mathematics.