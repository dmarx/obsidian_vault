see also:
- [[Analytic Functions]]

Holomorphic functions, central to the field of [[Complex Analysis]], are complex-valued functions of one or more complex variables that are [[differentiable]] in a [[neighborhood]] of every point in their domain. The concept of holomorphy extends the idea of differentiability known in real analysis to the context of complex numbers, offering rich properties and deep insights into the behavior of functions. These functions are also known as analytic functions, though some authors make a distinction in terms for functions defined on subsets of the complex plane.

### Definition and Properties

A function $f: U \rightarrow \mathbb{C}$, with $U$ being an open subset of the complex plane $\mathbb{C}$, is said to be holomorphic at a point $z_0 \in U$ if the limit

$$f'(z_0) = \lim_{z \rightarrow z_0} \frac{f(z) - f(z_0)}{z - z_0}$$

exists. This definition mirrors the definition of differentiability in real analysis but is applied to complex functions. If $f$ is holomorphic at every point in $U$, it is said to be holomorphic on $U$.

Holomorphic functions have several remarkable properties:

- **Complex Differentiability:** A key difference between real and complex differentiability is that if a complex function is differentiable at a point, it is infinitely differentiable at that point. Furthermore, complex differentiability implies that the function satisfies the Cauchy-Riemann equations, a set of partial differential equations.

- **[[Analytic Functions|Analyticity]]:** Holomorphic functions are analytic, meaning they can be locally represented by a convergent power series. This implies that knowing the behavior of a holomorphic function in a small region (in principle, an arbitrarily small one) determines its behavior everywhere within its domain of convergence.

- **Conformality:** At points where their derivative is non-zero, holomorphic functions preserve angles and the shape of small figures, though they may alter their size and orientation. This property makes them [[conformal mappings]].

- **Path Independence:** The integral of a holomorphic function over a path in its domain depends only on the endpoints of the path, a consequence of Cauchy's integral theorem. This leads to the powerful Cauchy integral formula, which provides an expression for the values of a holomorphic function inside a contour in terms of the values on the contour.

- **Maximum Modulus Principle:** Holomorphic functions cannot attain a local maximum of the absolute value |f(z)| inside their domain of definition. If the absolute value of the function has a local maximum, it must be constant over the connected component of the domain.

### Examples

- **Polynomials:** Complex polynomials are holomorphic everywhere in $\mathbb{C}$, making them entire functions.
  
- **Exponential Function:** The complex exponential function $e^z$ is holomorphic everywhere in $\mathbb{C}$ and shares many properties with its real counterpart, including the formula $e^{z+w} = e^z e^w$.

- **Trigonometric Functions:** Functions like $\sin(z)$ and $\cos(z)$, extended to the complex plane, are holomorphic everywhere.

### Importance

Holomorphic functions form the backbone of complex analysis and have profound implications in various branches of mathematics and physics. They are instrumental in solving problems in number theory, fluid dynamics, and electrical engineering, among other fields. The rich properties of holomorphic functions, such as their infinite differentiability and the strong constraints imposed by the Cauchy-Riemann equations, make them a powerful tool for theoretical investigation and practical problem-solving.