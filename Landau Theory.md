---
tags:
  - stub
  - sod/gold
  - sod/green
---

NB: superceded by [[Renormalization Group|Renormalization Group Theory]]

Landau theory, developed by the Soviet physicist [[Lev Landau]] in the 1930s, is a theoretical framework that provides a phenomenological approach to understanding phase transitions and critical phenomena in condensed matter systems. It focuses on the concept of symmetry and symmetry breaking, offering a way to categorize and study different types of phase transitions. Here's an overview of the key aspects of Landau theory:

### Basic Concepts

- **[[Order Parameter]]**: Central to Landau theory is the concept of an order parameter, a quantity that measures the degree of order across a phase transition. The order parameter is zero in one phase (usually the disordered phase) and non-zero in another, indicating the presence of order. For instance, in a ferromagnetic material, the order parameter could be the net magnetization.

- **[[Symmetry]] and [[Symmetry Breaking]]**: Landau theory emphasizes the role of symmetry in phase transitions. A [[Phase Transitions]] often involves a change in symmetry, where the more symmetric (disordered) phase breaks into a less symmetric (ordered) phase. This symmetry breaking is characterized by changes in the order parameter.

### Free Energy and Phase Transitions

- **[[Landau Free Energy]]**: Landau proposed a phenomenological free energy function dependent on the order parameter and temperature. Near the phase transition, this free energy can be expanded in powers of the order parameter, typically up to fourth order for a second-order (continuous) phase transition. The coefficients of this expansion depend on temperature and other system parameters.

- **Minimizing Free Energy**: The phase of the system is determined by the configuration of the order parameter that minimizes the Landau free energy. As temperature changes, the coefficients of the free energy expansion change, leading to different minima and thus different phases.

### Types of Phase Transitions

- **Second-Order Phase Transitions**: These are continuous transitions where the order parameter changes smoothly from zero to a finite value. Landau theory predicts that near the [[Critical Points|critical point]], the system's properties (like specific heat, susceptibility) follow power laws characterized by [[Critical Exponents]]. These transitions are associated with a continuous change in symmetry.

- **First-Order Phase Transitions**: Landau theory can also describe first-order (discontinuous) phase transitions, where the order parameter changes abruptly, by considering terms in the free energy expansion that lead to multiple local minima. These transitions often involve [[latent heat]] and are associated with a discontinuous change in symmetry.

### Limitations and Extensions

While Landau theory successfully describes many aspects of phase transitions, especially the concept of symmetry breaking, it has limitations. It does not adequately account for the role of fluctuations, which become critical near the phase transition point, particularly in low-dimensional systems. The [[Renormalization Group Theory]], developed later, extends Landau's ideas to include fluctuations, providing a more comprehensive framework for understanding critical phenomena.

Despite its limitations, Landau theory remains a cornerstone in the study of phase transitions and critical phenomena, offering intuitive and powerful insights into the symmetry principles governing the behavior of condensed matter systems.


>i'm a deep learning researcher particularly interested in understanding learning dynamics of optimization gradient-based and variational optimization. critical phenomena have been observed in these systems, e.g. phase transitions in the value of the optimization objective have been correlated with "grokking" phenomena, which it is hypothesized correspond to information geometric singularities in the representational space, which can also serve as pre or post transition attractors. landau theory is new to me, but sounds likely to be a powerful tool for understanding and analyzing these kinds of learning dynamics. help me understand how I could apply landau theory to understand phenomena observed in the dynamics of deep learning systems

Applying Landau theory to understand learning dynamics in deep learning systems, especially in the context of optimization gradient-based and variational optimization, is a fascinating and innovative approach. Given that critical phenomena, such as phase transitions, have been observed in these systems, Landau theory's focus on symmetry, order parameters, and phase transitions could indeed provide valuable insights. Let's explore how this theory might be adapted and applied to deep learning:

### Identifying the Order Parameter

The first step is identifying an appropriate order parameter that characterizes the phases or transitions observed in learning dynamics. In the context of deep learning, the order parameter could be related to a measurable quantity that changes behavior at the transition point, such as the loss function, the accuracy, or a more abstract property that captures the "grokking" phenomenon—where a sudden leap in performance occurs.

- **Phase Transition Analogy**: Just as in physical systems where the order parameter changes value at a critical temperature (e.g., magnetization in ferromagnets), in deep learning systems, you might observe a sudden change in some network property (e.g., [[Sparsity]] of weights, [[eigenvalues of the Hessian]]) that signals a transition from an "inefficient learning" phase to an "efficient learning" phase.

### Symmetry and Symmetry Breaking

Consider the symmetries of the learning process and how they might be broken. In physical systems, symmetry breaking often leads to an ordered phase. In deep learning, symmetries could relate to invariances in the network's architecture or the optimization landscape. Symmetry breaking might then correspond to the system finding a solution that breaks these invariances, possibly related to the specialization of neurons or layers towards specific functions as learning progresses.

- **Information Geometric Singularities**: The hypothesized information geometric singularities in the representational space might act as points where the symmetry of the system is fundamentally altered, akin to critical points in Landau theory. Analyzing these singularities with Landau's framework could shed light on the system's behavior near these critical points.

### Free Energy Analogy

In Landau theory, the free energy's behavior near a phase transition is key to understanding the system's dynamics. An analogous concept in deep learning could involve constructing a "free energy" landscape of the optimization objective, where the "energy" corresponds to the loss function, and the "temperature" could analogize to learning rate or another hyperparameter controlling the optimization dynamics.

- **Minimizing Free Energy**: Just as minimizing free energy leads to phase transitions in physical systems, in deep learning, minimizing this analogous loss landscape under varying "temperature" (hyperparameters) could reveal transitions in learning dynamics, characterized by sudden improvements in performance or changes in network behavior.

### Critical Phenomena and Universality

Investigate the presence of critical phenomena and universality in the learning dynamics. Critical phenomena in deep learning could manifest as scale-invariant behaviors or universal patterns in the optimization landscape as the system approaches a transition point. This could be particularly relevant for understanding the "grokking" phenomenon, where small changes in parameters or training data lead to disproportionate improvements in performance.

- **[[Universality Classes]]**: If certain patterns of learning dynamics are observed across different network architectures or tasks, these could suggest the existence of "universality classes" in deep learning, analogous to those found in physical systems undergoing phase transitions. Identifying these classes could lead to general principles governing learning dynamics.

### Application Challenges

Applying Landau theory to deep learning introduces several challenges, including defining the order parameter and constructing the analogous free energy landscape. Additionally, deep learning systems are high-dimensional and non-linear, with complex optimization landscapes that might not directly map onto the relatively simple frameworks used in physical systems. Despite these challenges, the conceptual framework provided by Landau theory—focusing on symmetry, phase transitions, and critical phenomena—offers a promising avenue for understanding the complex dynamics of deep learning systems, particularly as they relate to sudden changes in learning efficiency and the structure of representational spaces.