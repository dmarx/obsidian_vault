The Riemann integral, named after [[Bernhard Riemann]], is a method of assigning a number to define the area under a curve within a certain interval on the real line. It is one of the earliest formal definitions of an integral, specifically designed to rigorously define the concept of the area under a curve. The Riemann integral plays a fundamental role in calculus and analysis, particularly in the theory of integration.

### Definition

Consider a function $f:[a,b] \rightarrow \mathbb{R}$, where $[a,b]$ is a closed interval on the real number line. The Riemann integral of $f$ over $[a,b]$ is defined if the limit of the sum of the areas of rectangles under the curve, as the widths of the rectangles approach zero, exists and is the same regardless of how the heights of these rectangles are chosen (as long as they are chosen to lie on the function).

Mathematically, this process involves partitioning the interval $[a,b]$ into smaller subintervals, and then on each subinterval, selecting a point and forming a rectangle whose height is determined by the value of $f$ at this selected point. The Riemann integral is the limit of the sum of the areas of these rectangles as the maximum length of the subintervals approaches zero.

### Formal Construction

1. **Partition of $[a,b]$:** A partition $P$ of the interval $[a,b]$ is a finite sequence $a = x_0 < x_1 < \ldots < x_n = b$. Each $[x_{i-1}, x_i]$ is a subinterval of the partition.

2. **Sample Points and [[Riemann Sums]]:** For each subinterval $[x_{i-1}, x_i]$, choose a sample point $c_i$ in this interval. The sum $$S(P,f) = \sum_{i=1}^{n} f(c_i) \Delta x_i$$ where $\Delta x_i = x_i - x_{i-1}$, is called the Riemann sum of $f$ over $[a,b]$ with respect to the partition $P$ and the choice of sample points.

3. **Definition of the Riemann Integral:** The function $f$ is said to be Riemann integrable on $[a,b]$ if there exists a real number $I$ such that for every $\epsilon > 0$, there exists a $\delta > 0$ such that for any partition $P$ of $[a,b]$ with $\max\{\Delta x_i\} < \delta$ and any choice of sample points $\{c_i\}$, $$|S(P,f) - I| < \epsilon$$ In this case, $I$ is called the Riemann integral of $f$ over $[a,b]$ and is denoted by $$\int_a^b f(x) dx$$

### Properties

- **[[Linearity]]:** The Riemann integral is linear, meaning that $\int_a^b (cf(x) + dg(x)) dx = c\int_a^b f(x) dx + d\int_a^b g(x) dx$ for any functions $f$ and $g$ that are Riemann integrable over $[a,b]$ and any constants $c$ and $d$.
  
- **Additivity over intervals:** If $a < c < b$, then $\int_a^b f(x) dx = \int_a^c f(x) dx + \int_c^b f(x) dx$.

### Limitations and Extensions

While the Riemann integral is suitable for many functions, it cannot handle functions with too many discontinuities or peculiarities. For such functions, more general concepts of integration, like the [[Lebesgue Integral]], provide a more powerful and flexible framework. The Lebesgue integral extends the idea of integration to a wider class of functions and measures, offering tools for dealing with functions that are not Riemann integrable.

The development of the Riemann integral laid the groundwork for much of modern analysis and its applications to physics and engineering. Its formulation is a cornerstone in the history of mathematical analysis, illustrating the rigorous treatment of the concept of area under a curve.