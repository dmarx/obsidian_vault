---
tags:
  - sod/gold
---

see also:
- [[Duality]]
- [[Group Theory]]

Conjugacy classes are a fundamental concept in group theory, a branch of mathematics that studies symmetries and transformations. Understanding conjugacy classes is crucial for analyzing the structure of groups, particularly in abstract algebra and its applications in various mathematical and scientific fields, including chemistry, physics, and cryptography.

### Definition and Basics

In a group \( G \), two elements \( a \) and \( b \) are **conjugate** to each other if there exists an element \( g \) in \( G \) such that:

$$
b = g a g^{-1}
$$

Here, \( g^{-1} \) denotes the inverse of \( g \), and the operation is the group operation (which could be addition, multiplication, etc., depending on the group).

The set of all elements in \( G \) that are conjugate to a given element \( a \) forms the **conjugacy class** of \( a \). This class represents a subset of \( G \) where each member is related to \( a \) through conjugation by some element of \( G \).

### Properties

- **Equivalence Relation:** Conjugacy defines an equivalence relation on \( G \), partitioning \( G \) into disjoint conjugacy classes. All elements in a particular class share certain properties, such as their order (the smallest positive integer \( n \) such that \( a^n = e \), where \( e \) is the identity element of \( G \)).
- **Centralizer and Normalizer:** For any element \( a \) in \( G \), the set of all elements in \( G \) that commute with \( a \) forms a subgroup called the **centralizer** of \( a \), denoted \( C_G(a) \). The size of the conjugacy class of \( a \) is related to the index of the centralizer in \( G \) (i.e., \( |G : C_G(a)| \)).
- **Invariant Under Group Homomorphisms:** Conjugacy is preserved under group homomorphisms. If \( \phi: G \rightarrow H \) is a group homomorphism and \( a \) and \( b \) are conjugate in \( G \), then \( \phi(a) \) and \( \phi(b) \) are conjugate in \( H \).

### Importance in Group Theory

- **[[Class Equation]]:** The class equation of a group \( G \) relates the order of the group to the sizes of its conjugacy classes and is given by:
  
  $$
  |G| = |Z(G)| + \sum [G : C_G(a_i)]
  $$

  where \( |Z(G)| \) is the order of the center of \( G \) (elements that commute with all other elements in \( G \)), and \( a_i \) are representatives from the distinct non-central conjugacy classes.
- **[[Character Theory]]:** In the [[representation theory]] of groups, conjugacy classes play a central role in defining the characters of group representations, which are functions from the group to the complex numbers that are constant on conjugacy classes. These characters provide profound insights into the structure and representation of the group.
- **Classification of Elements:** In many practical applications, such as in solving polynomial equations using [[Galois theory]], understanding the conjugacy classes of the Galois group helps in determining the solvability of equations by radicals.

### Examples

- **The [[Symmetry Groups|Symmetric Group]] \( S_n \)**: In the symmetric group of degree \( n \), which consists of all permutations of \( n \) objects, two permutations are conjugate if and only if they have the same cycle type. Each conjugacy class corresponds to a distinct partition of \( n \) (a way of breaking down \( n \) into a sum of positive integers), which represents the cycle structure of the permutations in that class.

Conjugacy classes offer a way to understand the deep structure of groups by examining how elements can be transformed into one another through internal symmetries of the group. This understanding is pivotal for both theoretical explorations and practical applications of group theory.