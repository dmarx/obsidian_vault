see also:
- [[Group Theory]]
- [[Groups]]

Abelian groups, named after the Norwegian mathematician [[Niels Henrik Abel]], are a fundamental concept in [[Abstract Algebra]]. An abelian group is a set equipped with an operation that combines any two elements to form a third element, satisfying the axioms of associativity, identity, inverse, and commutativity. The commutative property, which distinguishes abelian groups from more general groups, ensures that the order in which two elements are combined does not affect the outcome of their operation.

### Formal Definition

An abelian group $(G, +)$ consists of a set $G$ and an operation $+$ such that for all elements $a, b, c \in G$, the following axioms are satisfied:

1. **Associativity**: $(a + b) + c = a + (b + c)$
2. **Identity**: There exists an element $0 \in G$ (often called the identity element) such that $a + 0 = 0 + a = a$ for all $a \in G$.
3. **Inverse**: For every $a \in G$, there exists an element $-a \in G$ (called the inverse of $a$) such that $a + (-a) = (-a) + a = 0$.
4. **Commutativity**: $a + b = b + a$ for all $a, b \in G$.

The operation $+$ is often referred to as "addition," and the identity element is frequently denoted by $0$, reflecting the intuition from familiar numerical addition. However, the operation could represent any binary operation that satisfies the group axioms, not just numerical addition.

### Examples of Abelian Groups

- **The set of integers $\mathbb{Z}$ under addition** is an abelian group. The identity element is $0$, and the inverse of any integer $n$ is $-n$. The commutative property holds since $m + n = n + m$ for all integers $m$ and $n$.

- **The set of real numbers $\mathbb{R}$ under addition** forms an abelian group, with similar properties as the group of integers in terms of addition.

- **The set of all rational numbers $\mathbb{Q}$ (excluding $0$) under multiplication** forms an abelian group. The identity element is $1$, and the inverse of any rational number $q$ is $\frac{1}{q}$. Note that commutativity holds because $pq = qp$ for all rational numbers $p$ and $q$.

- **The set of $n \times n$ matrices over a field $F$ under matrix addition** forms an abelian group. The identity element is the zero matrix, and the inverse of a matrix is the matrix with each element being the additive inverse of the original matrix's elements.

### Importance and Applications

Abelian groups are a cornerstone in various areas of mathematics and its applications:

- **Algebraic Topology**: Homology groups, which capture topological properties of spaces, are abelian groups.

- **Algebraic Number Theory**: The study of number fields and algebraic integers frequently uses abelian groups to understand the structure of units and ideals within rings.

- **Cryptography**: Certain cryptographic algorithms, especially those based on elliptic curves, rely on the properties of abelian groups.

- **Quantum Mechanics**: The state spaces in quantum mechanics, specifically those related to the symmetry operations of quantum systems, can be understood through the lens of abelian groups.

Understanding abelian groups and their properties is essential for exploring more complex structures in algebra, such as rings and fields, where the abelian nature of addition plays a critical role in defining and analyzing these structures' properties.