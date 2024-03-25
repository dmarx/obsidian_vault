Parallel transport is a fundamental concept in [[differential geometry]], providing a method for moving vectors along curves on a [[Manifolds|manifold]] in a way that preserves their "direction" relative to the manifold's geometry. It is closely associated with the notion of a [[Connection on a Manifold|connection]], which offers a precise mathematical framework to describe how vectors are "transported" along paths or curves on the manifold.

### Mathematical Formulation

Given a [[smooth]] manifold $M$ equipped with a connection (which can be thought of as a rule specifying how to [[differentiate]] [[vector fields]]), parallel transport along a curve $\gamma: [a, b] \to M$ is defined by the condition that the vector being transported has a covariant derivative of zero along $\gamma$. If $V(t)$ is a vector field along $\gamma(t)$, then $V$ is said to be [[parallel]] along $\gamma$ if

$$\nabla_{\dot{\gamma}(t)} V = 0$$

for all $t \in [a, b]$, where $\dot{\gamma}(t)$ is the tangent vector to the curve $\gamma$ at $t$, and $\nabla$ denotes the covariant derivative associated with the connection on $M$.

### Properties and Significance

- **Path Dependence:** Unlike in [[Euclidean space]], parallel transport on a curved manifold is generally path-dependent. That is, the result of transporting a vector from one point to another may depend on the path taken between the points. This path dependence is a manifestation of the manifold's curvature.

- **[[Geodesics]]:** Geodesics, the generalization of straight lines to curved manifolds, can be characterized as curves along which the tangent vector is parallel transported along itself. This means that if $\gamma(t)$ is a geodesic, then $\nabla_{\dot{\gamma}(t)} \dot{\gamma} = 0$.

- **[[Curvature]]:** The failure of parallel transport to preserve the [[orientation]] of vectors after being transported around a [[closed loop]] is directly related to the curvature of the manifold. The [[Riemann curvature tensor]], a fundamental object in differential geometry, quantifies this failure and provides a measure of the manifold's intrinsic curvature.

- **Applications in Physics:** Parallel transport plays a crucial role in [[general relativity]], where the connection (specifically the [[Levi-Civita connection]]) is determined by the [[spacetime metric]], and parallel transport reflects the influence of gravity on the motion of particles and light. In [[gauge theories]] of [[particle physics]], parallel transport is related to the concept of gauge [[Covariant Derivatives]], which describe how fields change under local gauge transformations.

### Example: Parallel Transport on a Sphere

A classic example of parallel transport is moving a vector along the surface of a sphere. If a vector is parallel transported along the equator, then moved up to the north pole along a meridian, then transported back along another meridian to the equator, and finally moved along the equator back to its starting point, the vector will have rotated with respect to its original [[orientation]]. This illustrates the path dependence of parallel transport and is a manifestation of the sphere's curvature.

Parallel transport thus serves as a key concept in understanding the [[geometry]] of curved spaces and the dynamics of fields and particles within those spaces, bridging the realms of pure mathematics and theoretical physics.