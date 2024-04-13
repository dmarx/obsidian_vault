[[Delaunay Triangulation]] is a fundamental structure in computational geometry, widely used in scientific computing, computer graphics, numerical simulations, and geographic information systems. It is named after the Russian mathematician Boris Delaunay for his work in this area in 1934.

### Definition
For a given set of discrete points in a Euclidean space $\mathbb{R}^d$, a Delaunay Triangulation is a triangulation such that no point in the set is inside the circumcircle of any triangle in the triangulation. In two dimensions, this means that for each triangle formed by the points, the circle passing through the vertices of the triangle contains no other point in its interior.

### Properties
The Delaunay Triangulation of a set of points has several notable properties:
1. **Uniqueness**: The Delaunay Triangulation is unique if no four points are cocircular. When four or more points are cocircular, there are multiple valid triangulations.
2. **Max-Min Angle Property**: It maximizes the minimum angle of all the angles of the triangles in the triangulation, helping to avoid skinny triangles.
3. **Duality with Voronoi Diagrams**: There is a dual relationship between the Delaunay Triangulation and the Voronoi diagram of the same set of points. Each vertex of the Voronoi diagram corresponds to a circumcircle of a Delaunay triangle.

### Mathematical Description
Formally, let $P$ be a finite set of points in $\mathbb{R}^2$. A triangulation $T$ of $P$ is Delaunay if for any triangle $\triangle abc \in T$, the circumcircle of $\triangle abc$ does not contain any other point $p \in P$ in its interior. The circumcircle condition can be checked using the determinant of a specific matrix derived from the coordinates of the points $a$, $b$, $c$, and $p$:
$$
\text{det} \begin{bmatrix}
a_x & a_y & a_x^2 + a_y^2 & 1 \\
b_x & b_y & b_x^2 + b_y^2 & 1 \\
c_x & c_y & c_x^2 + c_y^2 & 1 \\
p_x & p_y & p_x^2 + p_y^2 & 1 
\end{bmatrix} > 0
$$
This determinant is positive if and only if the point $p$ lies outside the circumcircle of the triangle formed by $a$, $b$, and $c$.

### Algorithms
There are several algorithms to compute the Delaunay Triangulation:
- **Incremental Insertion**: Points are added one at a time, updating the triangulation as necessary.
- **Divide and Conquer**: The set of points is divided into smaller subsets, which are triangulated separately and then merged.
- **Sweep Line and Plane Sweep**: These algorithms are similar to those used in computational geometry for other problems involving sorting points and processing them as they are "swept" across.

### Applications
Delaunay Triangulations are used in:
- **Mesh Generation**: For finite element methods and 3D reconstruction.
- **Interpolation**: Natural neighbor interpolation and other methods that need to find neighboring points.
- **Pathfinding in Games and Robotics**: Creating navigation meshes.

### Further Exploration
To explore more about how Delaunay Triangulations interact with other geometrical and topological concepts, you might look into topics like [[Triangulation Algorithms]] and the broader implications of their dual, the [[Voronoi Diagram]].

Understanding the complex relationships and applications of Delaunay Triangulation provides deep insights into spatial data structure and algorithm design, crucial for advanced studies and applications in many scientific and engineering fields.