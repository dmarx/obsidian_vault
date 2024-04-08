---
tags:
  - needs-outlinks
  - sod/gold
---
see also:
- [[Fourier's Law of Heat Conduction]]
- see also [[Ricci Flow]] - generalitzation

The heat equation is a [[Fundamental Partial Differential Equations|fundamental partial differential equation]] (PDE) in the field of mathematics and physics that describes how heat (or some analogous quantity) distributes itself over time in a given region. It is a cornerstone of classical heat conduction theory and plays a crucial role in various applications, including [[diffusion processes]], financial mathematics (e.g., the [[Black-Scholes equation]] for option pricing), and even in image processing techniques.

### Mathematical Formulation

In its simplest one-dimensional form, the heat equation for a homogeneous and isotropic medium can be written as:

$$\frac{\partial u}{\partial t} = \alpha \frac{\partial^2 u}{\partial x^2}$$

where:
- $u(x, t)$ is the temperature at position $x$ and time $t$,
- $\alpha$ is the [[thermal diffusivity]] of the medium, a positive constant that characterizes the rate at which heat diffuses through the material,
- $\frac{\partial u}{\partial t}$ is the partial derivative of temperature with respect to time, indicating how temperature changes over time,
- $\frac{\partial^2 u}{\partial x^2}$ is the second partial derivative of temperature with respect to space, representing the curvature of the temperature profile.

### Multi-Dimensional Heat Equation

The heat equation can be generalized to higher dimensions. For a three-dimensional space, it is expressed as:

$$\frac{\partial u}{\partial t} = \alpha \nabla^2 u$$

where $\nabla^2$ denotes the Laplace operator, defined in three dimensions as:

$$\nabla^2 u = \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} + \frac{\partial^2 u}{\partial z^2}$$

This general form encapsulates how heat diffuses in a three-dimensional medium.

### Boundary and Initial Conditions

To solve the heat equation for a particular physical situation, one must specify [[boundary conditions]] (conditions on the edges of the region of interest) and initial conditions (the temperature distribution at the start of observation, $t=0$). Common types of boundary conditions include:
- **[[Dirichlet boundary conditions]]**, which specify the temperature on the boundary,
- **[[Neumann boundary conditions]]**, which specify the heat flux on the boundary,
- **[[Robin boundary conditions]]**, a combination of Dirichlet and Neumann conditions.

### Solutions to the Heat Equation

The heat equation is a linear PDE, allowing it to be solved exactly for many configurations of boundary and initial conditions using various mathematical techniques, including [[separation of variables]], [[Fourier series]], and [[Fourier Transform|transform]] methods. The fundamental solution for the heat equation in an infinite domain is given by the [[Gaussian Kernel]] or heat kernel:

$$u(x,t) = \frac{1}{(4\pi \alpha t)^{n/2}} e^{-\frac{|x|^2}{4\alpha t}}$$

where $n$ is the dimension of the space. This solution represents the distribution of temperature at time $t$ resulting from an initial point heat source.

### Applications

- **Engineering**: The heat equation guides the design of heat sinks, insulation, and cooling systems.
- **Geosciences**: It models geothermal heat flow in Earth's crust.
- **Biology**: It can describe diffusion processes, such as the spread of a chemical substance in a cell or tissue.
- **Finance**: Analogous forms of the heat equation are used in modeling the evolution of prices in financial markets.

Understanding and solving the heat equation provides insights into the transient and steady-state behaviors of thermal systems, making it an essential tool in both theoretical and applied sciences.
