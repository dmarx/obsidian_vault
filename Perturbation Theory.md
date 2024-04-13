---
tags:
  - needs-outlinks
  - todo/merge
---
see also:
- [[Perturbation Methods]] - todo: merge

Perturbation theory is a mathematical approach used to find an approximate solution to a problem by starting from the exact solution of a simpler, related problem. This technique is widely employed in various domains of physics and engineering, such as quantum mechanics, classical mechanics, and fluid dynamics, to deal with problems that cannot be solved exactly due to their complexity. The essence of perturbation theory lies in introducing a small parameter, $\epsilon$, which measures the deviation of the complex problem from the simpler one. The solution is then expressed as a series expansion in terms of $\epsilon$.

### Overview and Formalism

The general idea behind perturbation theory is to take a problem for which the solution is unknown and express it in terms of a related problem with a known solution, plus a "perturbation" represented by a small parameter. The solution to the original problem is then developed as an expansion around the known solution, with terms that are powers of the small parameter.

#### Hamiltonian Example in Quantum Mechanics

A classical application of perturbation theory is in quantum mechanics, where one often deals with a [[Hamiltonian]] (the operator corresponding to the total energy of the system) that is a sum of two terms: $H = H_0 + \epsilon V$. Here, $H_0$ is the Hamiltonian for which the solution is known (the "unperturbed" Hamiltonian), and $\epsilon V$ represents a small perturbation. The eigenvalues and eigenfunctions of $H$ are sought as series expansions in $\epsilon$.

#### Mathematical Formulation

Let's consider a linear problem governed by the equation:
$$
L(y) = \epsilon N(y),
$$
where $L$ is a linear operator for which solutions can be easily obtained, $\epsilon$ is a small parameter, and $N$ represents a nonlinear perturbation. The solution $y$ can be expanded as a power series in $\epsilon$:
$$
y = y_0 + \epsilon y_1 + \epsilon^2 y_2 + \ldots,
$$
where $y_0$ is the solution to the unperturbed problem ($L(y_0) = 0$), and $y_1, y_2, \ldots$ represent the corrections due to the perturbation.

### Applications of Perturbation Theory

1. **Quantum Mechanics**: Used to calculate the energy levels and state functions of systems under small external fields or interactions not accounted for in the solvable part of the Hamiltonian.
2. **Celestial Mechanics**: Helps in studying the orbits of planets and satellites by treating the gravitational effects of other bodies as perturbations.
3. **Fluid Dynamics**: Employed to solve problems involving fluid flow at high Reynolds numbers, where exact solutions are not feasible.
4. **Elasticity Theory**: Used to solve problems in structural mechanics where the deformation of structures under external forces is analyzed.

### Advantages and Limitations

- **Advantages**: Perturbation theory provides a powerful tool for tackling problems that are otherwise unsolvable using exact methods. It gives a systematic way to approximate solutions and understand the effects of small changes or interactions in a system.

- **Limitations**: The main limitation is its reliance on the existence of a small parameter, $\epsilon$, which means it might not be applicable to strongly coupled systems where no clear small parameter exists. Moreover, the series obtained may not always converge, or its convergence might be slow, limiting the practical utility of the approach.

### Conclusion

Perturbation theory is a cornerstone of theoretical physics and applied mathematics, offering insight into the behavior of complex systems by building upon the solutions of simpler models. Despite its limitations, it remains an indispensable tool in the physicist's and engineer's toolkit, enabling the study of phenomena that would otherwise be beyond reach.