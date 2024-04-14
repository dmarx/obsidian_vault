---
tags:
  - sod/gold
---
see also:
- [[Harmonic Forms]]
- [[Harmonic Maps]]
- [[Harmonic Functions]]
- [[Harmonic Analysis]]
- [[Harmonic Analysis On Groups]]
- [[Spherical Harmonics]]
- [[Harmonic Oscillator]]
- [[Fourier Analysis]]
- [[Functional Analysis]]

The concept of **harmonicity** is central in various mathematical disciplines, especially in differential geometry, complex analysis, and potential theory. Harmonicity describes functions or objects that satisfy a specific condition derived from the Laplacian operator. This operator, which measures how a function deviates from its mean value at a point, is pivotal in understanding the behavior of functions and forms under diffusion and wave propagation, as well as in physical and geometric contexts.

### Definition

A function $u: \mathbb{R}^n \rightarrow \mathbb{R}$ (or from a subset of $\mathbb{R}^n$) is called **harmonic** if it satisfies the Laplace equation:
$$ \Delta u = 0 $$
where $\Delta$ is the Laplacian operator given by:
$$ \Delta = \sum_{i=1}^n \frac{\partial^2}{\partial x_i^2} $$

### Mathematical Formalism

#### [[Laplace Operator|Laplacian Operator]]
The Laplacian $\Delta$ is a second-order differential operator in the Euclidean space defined as the divergence of the gradient of a function. In mathematical terms, for a function $u: \mathbb{R}^n \rightarrow \mathbb{R}$, the Laplacian is:
$$ \Delta u = \nabla \cdot \nabla u = \sum_{i=1}^n \frac{\partial^2 u}{\partial x_i^2} $$

This operator plays a crucial role in physics and mathematics, particularly in the theories of heat, light, and sound, which are based on the diffusion equation (a parabolic partial differential equation involving the Laplacian).

#### Properties of Harmonic Functions
- **Mean Value Property**: Harmonic functions have the mean value property, which states that the value of a harmonic function at a point is equal to the average value of the function over any spherical surface centered at that point. Mathematically, for a harmonic function $u$ and a ball $B(x,r)$ centered at $x$ with radius $r$,
  $$ u(x) = \frac{1}{|S(x, r)|} \int_{S(x, r)} u \, dS $$
  where $|S(x, r)|$ is the surface area of the sphere.

- **Maximum Principle**: Harmonic functions also obey the maximum principle, which posits that a harmonic function defined within a bounded domain attains its maximum and minimum on the boundary of the domain, not in the interior (unless the function is constant).

### Examples and Applications

1. **Potential Theory**: In potential theory, the potential functions arising from mass distributions (gravitational potential) or charge distributions (electrostatic potential) are harmonic in regions without mass or charge.

2. **Fluid Dynamics**: The velocity potential of an incompressible, irrotational fluid flow is a harmonic function, providing insights into flow dynamics around objects.

3. **Riemann Surfaces and Complex Analysis**: In complex analysis, the real and imaginary parts of a holomorphic function (complex function differentiable in the neighborhood of every point in its domain) are harmonic functions. This interplay is central in the study of conformal mappings and complex potentials.

### Generalization in Differential Geometry

In the context of differential geometry, the concept of harmonicity extends to differential forms and tensors. For example, a differential form $\omega$ on a Riemannian manifold is harmonic if it satisfies:
$$ \Delta \omega = 0 $$
Here, $\Delta$ is the Laplace-de Rham operator defined earlier.

The theory of harmonic maps, which are maps between Riemannian manifolds that minimize the energy functional, also heavily relies on the Laplacian and its generalizations. This is crucial in the study of geometric morphisms and deformations.

### Conclusion

Harmonicity thus emerges as a foundational property in various branches of mathematics and physics, linking concepts from differential equations, geometric analysis, and theoretical physics. Its pervasive nature underscores the deep interconnectedness of natural phenomena and mathematical abstraction.