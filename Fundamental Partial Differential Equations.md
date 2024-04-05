Partial Differential Equations (PDEs) are mathematical equations that involve functions of several variables and their partial derivatives. They are fundamental to describing various physical, chemical, biological, and financial phenomena where quantities change with respect to multiple variables. PDEs are crucial in modeling waves, heat flow, fluid dynamics, quantum mechanics, and many other processes. Below, we discuss some of the fundamental PDEs that play pivotal roles across different scientific disciplines.

### 1. [[Heat Equation]]

The heat equation models the distribution and evolution of heat (or temperature) in a given region over time. It is a parabolic PDE that reflects how temperature changes due to conduction:

$$ \frac{\partial u}{\partial t} = \alpha \nabla^2 u $$

where $u$ represents the temperature, $\alpha$ is the thermal diffusivity, $t$ is time, and $\nabla^2$ denotes the Laplacian operator, which generalizes the concept of curvature to higher dimensions.

### 2. [[Wave Equation]]

The wave equation describes the propagation of waves (e.g., sound waves, electromagnetic waves) through a medium. It is a second-order hyperbolic PDE:

$$ \frac{\partial^2 u}{\partial t^2} = c^2 \nabla^2 u $$

where $u$ is the wave function, $c$ is the speed of the wave in the medium, and $\nabla^2$ is the Laplacian.

### 3. [[Laplace's Equation]]

Laplace's equation is a second-order elliptic PDE used in potential theory, electrostatics, and fluid dynamics, among other fields. It represents stationary (time-independent) solutions where there is no net change in a quantity:

$$ \nabla^2 u = 0 $$

The solutions to Laplace's equation, known as harmonic functions, have no local maxima or minima.

### 4. [[Poisson's Equation]]

Poisson's equation is a generalization of Laplace's equation that includes a source term, making it applicable to a wider range of physical situations, such as gravitational and electrostatic potentials in the presence of density or charge distributions:

$$ \nabla^2 u = f $$

where $f$ represents the source term.

### 5. [[Schrodinger Equation|Schrödinger Equation]]

The Schrödinger equation is fundamental to quantum mechanics, describing how the quantum state of a physical system changes over time. It is a first-order PDE in time, but involves second-order spatial derivatives:

$$ i\hbar \frac{\partial \psi}{\partial t} = -\frac{\hbar^2}{2m} \nabla^2 \psi + V \psi $$

where $\psi$ is the wave function of the system, $\hbar$ is the reduced Planck constant, $m$ is the mass, and $V$ represents the potential energy.

### 6. [[Navier-Stokes Equations]]

The Navier-Stokes equations describe the motion of fluid substances such as liquids and gases. They are a set of nonlinear PDEs that account for viscosity, pressure, and external forces:

$$ \frac{\partial \mathbf{v}}{\partial t} + (\mathbf{v} \cdot \nabla) \mathbf{v} = -\frac{1}{\rho} \nabla p + \nu \nabla^2 \mathbf{v} + \mathbf{f} $$

where $\mathbf{v}$ is the fluid velocity field, $\rho$ is the density, $p$ is the pressure, $\nu$ is the kinematic viscosity, and $\mathbf{f}$ represents external forces.

Each of these PDEs serves as a cornerstone in its respective domain, embodying the mathematical principles required to model and understand complex phenomena in nature and engineered systems. The study and solution of these equations require a deep understanding of calculus, differential equations, and numerical methods, underscoring their significance in applied mathematics and theoretical physics.