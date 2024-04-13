
Carathéodory's theorem is a fundamental result in [[convex geometry]], named after Constantin Carathéodory. It states that if a point $x$ lies in the [[Convex Hull]] of points in $ \mathbb{R}^d $, then there is a subset of these points, consisting of $d+1$ or fewer points, such that $x$ is in the convex hull of just this subset.

### Formal Statement
Let $X \subset \mathbb{R}^d$. For any point $x$ in the convex hull of $X$, there exists a subset $\{x_1, x_2, \ldots, x_{d+1}\} \subseteq X$ such that
$$
x \in \text{conv}\{x_1, x_2, \ldots, x_{d+1}\},
$$
where $\text{conv}\{x_1, x_2, \ldots, x_{d+1}\}$ denotes the convex hull of the points $x_1, x_2, \ldots, x_{d+1}$.

### Mathematical Implications
This theorem is significant because it simplifies the analysis of convexity in higher dimensions by reducing the problem to a finite computation involving at most $d+1$ points, where $d$ is the dimension of the space. In practical terms, it implies that any point inside a convex set can be represented as a convex combination of at most $d+1$ vertices of that set.

### Proof Outline
1. **Base Case**: If $d=1$, the convex hull of a set of points in $\mathbb{R}^1$ (a line segment) is trivially spanned by at most two points.
   
2. **Inductive Step**: Assume the statement is true for $\mathbb{R}^{d-1}$. Consider a point $x$ in the convex hull of points in $\mathbb{R}^d$. The set of these points, say $X$, spans a polytope in $\mathbb{R}^d$. By the properties of convex polytopes, $x$ can be expressed as a convex combination of the vertices of a simplex containing $x$, involving at most $d+1$ points.

3. **Geometric Construction**: By projecting $x$ onto the affine hull formed by fewer than $d+1$ points and using the inductive hypothesis, one can show that $x$ can still be represented as a convex combination of no more than $d+1$ points.

### Applications
Carathéodory's theorem is crucial in various fields, including optimization, economics, game theory, and computational geometry. In optimization, it helps simplify problems by reducing the dimensionality of constraints. In economics and game theory, it provides a theoretical foundation for models involving mixed strategies or market equilibria.

For further technical insights and examples, you might explore its applications in [[Linear Programming]] and [[Computational Geometry]]. These topics illustrate how the theorem serves as a cornerstone in both theoretical and applied mathematics.