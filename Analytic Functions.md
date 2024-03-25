see also:
- [[Complex Analysis]]
- [[Analysis]]
- [[Harmonic Functions]]
- [[Harmonic Function]]
- [[Analyticity]]

Analytic functions, a cornerstone of complex analysis, are functions that can be locally expressed by a [[convergent]] [[power series]] around every point within their domain. This concept of analyticity reveals deep insights into the behavior and properties of functions, extending well beyond the initial definitions found in real analysis to encompass functions of complex variables.

### Definition of Analytic Functions

A function $f$ of a complex variable $z$ is said to be analytic at a point $z_0$ if, in some neighborhood of $z_0$, it can be represented as a convergent power series:

$$f(z) = \sum_{n=0}^{\infty} a_n (z - z_0)^n$$

where $a_n$ are complex coefficients, and the series converges to $f(z)$ for $z$ near $z_0$. A function is analytic on a domain if it is analytic at every point in that domain.

### Properties

- **[[Differentiability]]:** A hallmark of analytic functions is that if a function is analytic at a point, it is infinitely differentiable at that point, and its derivatives can be obtained by differentiating the power series term-by-term.

- **Uniqueness:** If two analytic functions agree on any set of points with an accumulation point within their common domain, they agree on the entire domain. This property underscores the rigidity of analytic functions.

- **[[Identity Theorem]]:** The uniqueness property leads to the identity theorem for analytic functions, stating that if two analytic functions are equal on any non-discrete subset of their domain, then they are equal everywhere in their domain.

- **[[Analytic Continuation]]:** The concept of analytic continuation allows extending an analytic function beyond its original domain of convergence by linking [[power series expansions]]. This process can reveal unexpected connections between different areas of mathematics.

- **[[Cauchy-Riemann Equations]]:** For functions of a complex variable, being analytic implies satisfying the Cauchy-Riemann equations, which are conditions on the partial derivatives that signify a deep interplay between the real and imaginary parts of the function.

### Real vs. Complex Analytic Functions

While the notion of analyticity applies to both real and complex functions, complex analytic functions—often referred to as holomorphic functions—exhibit richer properties due to the complex structure. Every complex analytic function is [[Holomorphic Functions|holomorphic]], and conversely, every holomorphic function is analytic, a result of the complex version of the [[Taylor series]]. In contrast, real analytic functions are defined similarly by [[power series]] but only over the real numbers, and their properties, while still powerful, do not encapsulate the full depth seen in the complex case.

### Examples and Applications

- **[[Elementary Functions]]:** Many elementary functions, including exponential, logarithmic, trigonometric, and their inverses, are analytic in their domains within the complex plane. For instance, $e^z$ and $\sin(z)$ are analytic everywhere in $\mathbb{C}$.

- **Zeta Function:** The [[Riemann zeta function]], central to number theory, is defined via a series that converges for complex numbers with real part greater than 1 and can be analytically continued to other parts of the complex plane.

- **Quantum Mechanics:** In physics, analytic functions find applications in quantum mechanics and the theory of wave functions, where analyticity conditions relate to physical constraints.

Analytic functions, through their structure and the wealth of properties they exhibit, play a crucial role in the interplay between analysis, geometry, and physics. They provide a fundamental framework for understanding complex systems, solving differential equations, and exploring the vast landscape of mathematical functions.