A connection on a manifold is a mathematical tool used in [[differential geometry]] to systematically describe how to "compare" or "connect" tangent spaces at different points on the [[Manifolds|manifold]]. Since a manifold is a generalization of surfaces and curves into higher dimensions, and it locally resembles [[Euclidean Space]], we need a way to navigate its [[curvature]] and [[topology]] smoothly. A connection provides a framework for this, enabling the [[differentiation]] of [[vector fields]] along curves on the manifold and thus laying the groundwork for defining [[parallel transport]], curvature, and [[geodesics]].

### Definition and Intuition

Intuitively, a connection gives a rule for how to "slide" vectors along paths in the manifold in a way that respects the manifold's geometry. This is crucial for formulating concepts like the derivative of a [[vector field]] along another vector field, which cannot be directly defined in curved spaces as it can in Euclidean space due to the lack of a global [[frame of reference]].

### Formal Description

Mathematically, a connection on a smooth manifold $M$ is often described using a connection form in the context of [[Principal Bundles]], or more concretely, through its [[Action]] on vector fields. One common approach is to define a connection as a [[covariant derivative]], denoted $\nabla$, which is a rule that takes a vector field $X$ and another vector field $Y$ and produces a new vector field $\nabla_X Y$. This derivative has to satisfy certain properties like [[linearity]] in $X$ and the [[Leibniz Rule]] in $Y$:

1. $\nabla_{fX + gY}Z = f\nabla_X Z + g\nabla_Y Z$ for any scalar functions $f, g$ on $M$,
2. $\nabla_X(Y + Z) = \nabla_X Y + \nabla_X Z$,
3. $\nabla_X(fY) = f\nabla_X Y + (Xf)Y$ for any scalar function $f$ on $M$.

### Parallel Transport and Geodesics

One of the main applications of a connection is to define what it means to "move" a vector along a curve in the manifold without "turning" it with respect to the manifold's geometry. This process is called parallel transport. A vector is said to be parallel along a curve if its covariant derivative along the curve is zero at all points. Using the concept of parallel transport, one can define geodesics as curves that parallel transport their own tangent vectors, serving as the generalization of "straight lines" to curved spaces.

### Curvature

The curvature of a connection, a measure of how the geometry of the manifold deviates from flat Euclidean space, can be computed from the connection itself. Formally, the curvature is a 2-form that takes two vector fields and returns a new operator on vector fields, embodying the [[noncommutativity]] of [[Covariant Derivatives]]: the [[Riemann curvature tensor]].

### Applications and Significance

Connections are indispensable in modern geometry and theoretical physics. In [[general relativity]], for instance, the [[Levi-Civita connection]] (a type of connection determined uniquely by the manifold's [[Measure|metric]] with no torsion) is used to describe spacetime's curvature. Connections also play a critical role in [[gauge theories]] in particle physics, where they appear as [[Potential Fields|potential fields]] mediating the [[fundamental forces]].

Overall, the concept of a connection on a manifold is a fundamental building block for describing and understanding the geometric structures of spaces encountered in mathematics and physics, enabling the rigorous treatment of dynamics, curvature, and topology on curved spaces.