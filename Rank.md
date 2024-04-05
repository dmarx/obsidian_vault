see also:
- [[Linear Algebra]]

In mathematics, the concept of "rank" is utilized in various contexts, such as matrices, tensors, and abstract algebra, each with a slightly different definition depending on the structure being considered. However, at its core, rank is a measure of the [[dimensionality]] or the degree of complexity of the mathematical object in question. Here, we'll focus on tensor rank, while also touching upon matrix rank for foundational understanding.

### Matrix Rank

The rank of a matrix is the maximum number of linearly independent column vectors in the matrix or equivalently, the maximum number of linearly independent row vectors. Mathematically, for a matrix $A$, its rank can be denoted as $\text{rank}(A)$. This concept is foundational in linear algebra and informs about the matrix's properties, such as whether the system of linear equations it represents has a unique solution, and the dimension of its column and row space.

- **Example**: A matrix $A \in \mathbb{R}^{m \times n}$ has rank $r$ if the maximum number of linearly independent columns (or rows) is $r$. This also means there exists at least one $r \times r$ submatrix with a non-zero determinant, while any larger submatrix has a determinant of zero.

### Tensor Rank

Moving beyond matrices (which are rank-2 tensors), the concept of rank in the context of tensors (multidimensional arrays of numerical values) becomes more nuanced. Tensors are generalizations of scalars (rank-0 tensors), vectors (rank-1 tensors), and matrices (rank-2 tensors) to higher dimensions.

#### Definition

Tensor rank, especially when discussing higher-order tensors (rank-3 or higher), can refer to several different concepts, depending on the context:

1. **Tensor Rank in Multilinear Algebra**: In its most traditional sense, the rank of a tensor is the smallest number of simple tensors (outer products of vectors) that sum to the tensor. This definition generalizes the concept of matrix rank and is related to tensor decompositions, such as the CANDECOMP/PARAFAC (CP) decomposition.

2. **Mode-$n$ Rank**: For an $n$-th order tensor, the mode-$n$ rank refers to the rank of the matrix obtained by unfolding or flattening the tensor along its $n$-th dimension. This concept is utilized in operations like the Tucker decomposition, where a tensor is decomposed into a core tensor multiplied by a matrix along each mode.

#### Challenges and Importance

- **[[Computational Complexity]]**: Unlike matrix rank, computing the rank of a tensor (as defined in multilinear algebra) is an NP-hard problem, making exact computations infeasible for large tensors.
- **Applications**: Understanding and utilizing tensor rank is crucial in many applications, including [[signal processing]], quantum physics, machine learning, and data compression. For example, low-rank tensor approximations can significantly reduce the amount of data needed to represent high-dimensional data sets efficiently.

### Example

Consider a third-order [[tensor]] (a three-dimensional array) $\mathcal{T}$ with dimensions $I \times J \times K$. Its rank according to [[multilinear algebra]] would be the minimum number of rank-1 tensors (which can be visualized as the simplest possible tensors that cannot be decomposed further) required to express $\mathcal{T}$ as their sum.

### Conclusion

Whether in the context of matrices or tensors, the concept of rank provides insight into the structure and complexity of mathematical objects. While the rank of a matrix is a well-understood and computationally tractable property, the rank of higher-order tensors introduces additional complexity and richness, reflecting the challenges and opportunities in understanding multidimensional data.