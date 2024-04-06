A **linear space**, more commonly referred to as a **vector space** in modern mathematical terminology, is a fundamental concept in [[linear algebra]]. It provides a framework for studying [[Vectors and Covectors|vectors]], which can be added together and multiplied ("scaled") by numbers, called scalars. Scalars are often taken from the real numbers $\mathbb{R}$, but they can also come from other fields such as the complex numbers $\mathbb{C}$. The formal definition and properties of a vector space encapsulate the algebraic structure necessary for such operations.

### Definition

A vector space over a field $F$ consists of a set $V$ along with two operations:

1. **Vector Addition**: An operation that takes two elements from $V$, say $u$ and $v$, and assigns to them a third element $u + v$ in $V$.
2. **Scalar Multiplication**: An operation that takes an element from $F$ (a scalar), say $a$, and an element from $V$, say $v$, and assigns to them an element $a \cdot v$ or $av$ in $V$.

These operations must satisfy the following axioms, for all $u, v, w \in V$ and $a, b \in F$:

1. **Additive [[Closure]]**: $u + v$ is in $V$.
2. **Additive [[Associativity]]**: $u + (v + w) = (u + v) + w$.
3. **Additive Identity**: There exists an element $0 \in V$, called the zero vector, such that $v + 0 = v$ for all $v \in V$.
4. **Additive Inverse**: For each $v \in V$, there exists an element $-v \in V$, called the additive inverse of $v$, such that $v + (-v) = 0$.
5. **Scalar Multiplication Closure**: $a \cdot v$ is in $V$.
6. **[[Distributivity]] of Scalar Multiplication with respect to Vector Addition**: $a \cdot (u + v) = a \cdot u + a \cdot v$.
7. **Distributivity of Scalar Multiplication with respect to [[Field]] Addition**: $(a + b) \cdot v = a \cdot v + b \cdot v$.
8. **Associativity of Scalar Multiplication with respect to Field Multiplication**: $a \cdot (b \cdot v) = (a \cdot b) \cdot v$.
9. **Multiplicative Identity**: There exists an element $1 \in F$, being the multiplicative identity in $F$, such that $1 \cdot v = v$ for all $v \in V$.

### Examples

1. **$\mathbb{R}^n$**: The set of all $n$-tuples of real numbers, with standard vector addition and scalar multiplication, is a vector space over $\mathbb{R}$.

2. **Function Spaces**: The set of all real-valued functions defined on an interval with function addition and scalar multiplication forms a vector space.

3. **Matrices**: The set of all $m \times n$ matrices over a field $F$, with matrix addition and scalar multiplication, is a vector space over $F$.

### Significance

Vector spaces are a central concept in mathematics and its applications. They provide the language for discussing and solving systems of linear equations, represent geometric shapes in graphics and simulations, and form the foundation for more complex structures like vector bundles and modules. Beyond pure mathematics, vector spaces are essential in physics, engineering, computer science, and economics, where they offer a powerful tool for modeling and problem-solving across diverse domains.