Functionals are a fundamental concept in mathematics and physics, particularly within the fields of [[calculus of variations]], [[functional analysis]], and [[quantum mechanics]]. A functional is a type of function, but instead of mapping numbers to numbers (as in ordinary functions), it maps functions to numbers. This means that the input of a functional is an entire function, and its output is a scalar value. Functionals play a crucial role in various mathematical formulations and physical theories, providing a way to express quantities that depend on functions, such as energy, action, or probability.

### Definition

Formally, if $\mathcal{F}$ is a functional, and $\phi(x)$ is a function, then the functional applied to $\phi(x)$, denoted as $\mathcal{F}[\phi]$, produces a scalar:

$$\mathcal{F}[\phi] : \{\text{Functions}\} \rightarrow \mathbb{R} \text{ or } \mathbb{C}$$

### Examples of Functionals

1. **[[Integral]] Functionals**: Many common functionals are expressed as integrals of functions. For example, the functional giving the area under a curve $\phi(x)$ from $a$ to $b$ is:

$$A[\phi] = \int_a^b \phi(x) \, dx$$

2. **[[Action]] in Physics**: In classical mechanics, the action is a functional of the trajectory of a system. For a particle moving along a path $\mathbf{x}(t)$, the action $S$ can be expressed as:

$$S[\mathbf{x}] = \int_{t_1}^{t_2} L(\mathbf{x}(t), \dot{\mathbf{x}}(t), t) \, dt$$

where $L$ is the [[Lagrangian]] of the system, which depends on the path $\mathbf{x}(t)$, its time derivative $\dot{\mathbf{x}}(t)$, and time $t$.

3. **Functional Derivative and [[Euler-Lagrange Equation]]**: The concept of varying a functional to find its stationary points leads to the Euler-Lagrange equation in the calculus of variations. This equation provides conditions under which a functional reaches an extremum, analogous to finding the derivatives of functions and setting them to zero in basic calculus.

### Importance in Quantum Mechanics

In quantum mechanics, particularly in the [[path integral]] formulation, the [[probability amplitude]] of a particle's state transition is given by a functional integral over all possible paths the particle could take, each weighted by the exponential of the action (a functional of the path) divided by Planck's constant.

### Functional Analysis

Functional analysis is a branch of mathematical analysis that studies functionals and the spaces of functions on which they act, such as [[Banach spaces]] and [[Hilbert spaces]]. This field is fundamental to modern mathematical physics, [[partial differential equations]], and [[numerical analysis]].

### Applications

- **[[Optimization]]**: Finding the function that maximizes or minimizes a functional is a common problem in physics, engineering, and economics.
  
- **[[Variational Principles]]**: Many physical systems can be described by variational principles, where the laws of motion or field equations can be derived by finding stationary points of appropriate functionals.

- **Machine Learning**: In machine learning, particularly in the training of neural networks, loss functions can be considered as functionals that map the function represented by the network to a scalar value indicating the error or loss.

Functionals encapsulate the idea of operations on functions, extending the concept of functions to higher-dimensional spaces and providing a powerful tool for analysis and optimization in diverse scientific fields.