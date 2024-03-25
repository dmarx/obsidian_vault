see also:
- [[Inner Product]]

The Leibniz Rule, named after the German mathematician [[Gottfried Wilhelm Leibniz]], is a fundamental principle in calculus that describes how to differentiate a product of two functions. It's a manifestation of the product rule in differentiation and plays a crucial role in various areas of mathematics, including [[differential calculus]], [[differential equations]], and the [[Theory of Distributions]]. The rule is essential for computing [[derivatives]] efficiently and is foundational in both basic and advanced calculus.

### Statement of the Leibniz Rule

For two [[differentiable functions]] $f(x)$ and $g(x)$, the Leibniz Rule states that the derivative of their product with respect to $x$ is given by:

$$\frac{d}{dx}(f(x)g(x)) = f(x)\frac{d}{dx}g(x) + g(x)\frac{d}{dx}f(x)$$

This means that to differentiate the product of two functions, one multiplies the derivative of the first function by the second function as it is, and adds to it the product of the first function as it is with the derivative of the second function.

### Generalizations

- **Higher Derivatives:** The Leibniz Rule can be extended to higher-order derivatives of products of two functions, often required in the study of differential equations and mathematical [[Analysis]]. For the $n$-th derivative, the rule takes the form of a binomial expansion:

$$\frac{d^n}{dx^n}(f(x)g(x)) = \sum_{k=0}^{n} \binom{n}{k} \frac{d^{n-k}}{dx^{n-k}}f(x) \cdot \frac{d^k}{dx^k}g(x)$$

where $\binom{n}{k}$ are the binomial coefficients.

- **[[Integration by Parts]]:** The Leibniz Rule is closely related to the technique of [[Integral|integration]] by parts, which is essentially the integral form of the product rule. Integration by parts allows for the integration of products of functions to be simplified based on their derivatives and is given by:

$$\int f(x)g'(x)dx = f(x)g(x) - \int f'(x)g(x)dx$$

- **Differential Equations:** In the context of differential equations, particularly linear differential operators, the Leibniz Rule is essential for expressing how [[operators]] act on products of functions or solutions.

### Applications

The Leibniz Rule finds applications across mathematics and physics. It's used in solving differential equations, in the derivation of physical laws from principles of calculus, and in computational techniques for evaluating derivatives. The rule's simplicity and power make it a staple in the toolkit of students and researchers alike, facilitating the analysis of complex problems in engineering, physics, economics, and beyond.

Overall, the Leibniz Rule exemplifies the elegance and utility of calculus as a mathematical discipline, providing a straightforward yet profound method for dealing with the derivatives of product functions.