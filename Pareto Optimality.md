---
tags:
  - sod/gold
  - empty-hub
---
see also:
- [[Resource Allocation]]
- [[Resource Distribution]]
- [[Optimization]]
- [[Game Theory]]

Pareto Optimality, named after the Italian economist [[Vilfredo Pareto]], is a concept within the field of economics and game theory that represents a state of allocation of resources from which it is impossible to reallocate so as to make any one individual or preference criterion better off without making at least one individual or preference criterion worse off. This concept is a fundamental criterion for [[efficiency]] in [[economics]] and [[game theory]], indicating an [[optimal distribution of resources in a society or system]], [[assuming that utility or benefit can be measured and compared across individuals or entities]].

### Formal Definition

An allocation $(x_1, x_2, \ldots, x_n)$ of resources among $n$ individuals is Pareto optimal if there is no other feasible allocation $(y_1, y_2, \ldots, y_n)$ such that:

1. At least one individual prefers $y_i$ to $x_i$, and
2. No individual prefers $x_i$ to $y_i$.

Mathematically, let $U_i(x)$ be the utility function of individual $i$, where $x$ represents a bundle of goods or allocation. An allocation $x^*$ is Pareto optimal if there does not exist another allocation $y$ such that:

$$
U_i(y) \geq U_i(x^*) \quad \text{for all } i, \text{ with strict inequality for at least one } i.
$$

### Implications and Criticisms

- **Efficiency vs. Equity**: While Pareto Optimality focuses on efficiency, it does not necessarily imply [[equity]] or [[fairness]] in the distribution of resources. An allocation where one individual holds all the resources can be Pareto optimal if reallocating any resource would make that individual worse off, regardless of the distribution among others.
- **[[Pareto Improvement]]**: A change from one allocation to another that makes at least one individual better off without making anyone else worse off is called a Pareto improvement. The concept of making Pareto improvements until reaching a point where no further Pareto improvements can be made underlies many economic policies aimed at increasing [[social welfare]].
- **Use in [[Welfare Economics]]**: Pareto Optimality is a central concept in welfare economics, which studies how the allocation of resources affects economic well-being. It provides a criterion for evaluating policies and economic states based on their efficiency rather than their fairness.

### Mathematical Extensions and Applications

Pareto Optimality extends beyond simple resource allocation problems to more complex scenarios, including [[public economics]], [[environmental economics]], and [[multi-objective optimization]] in engineering and [[management science]]. For instance, in environmental economics, an allocation of environmental resources is Pareto optimal if no environmental quality improvement can be achieved without worsening economic output or vice versa.

In multi-objective optimization, a solution is considered Pareto optimal if it is not dominated by any other solution in all objectives. Mathematically, a solution $x^*$ is Pareto optimal if there does not exist another solution $x$ such that $f_i(x) \leq f_i(x^*)$ for all objectives $i$ and $f_j(x) < f_j(x^*)$ for at least one objective $j$, where $f_i(x)$ is the value of objective $i$ at solution $x$.

Pareto Optimality represents a foundational principle in understanding the [[trade-offs]] and potential improvements in systems involving multiple agents or criteria, highlighting the complexities of achieving efficiency and the challenges inherent in balancing efficiency with other [[societal values]] such as [[equity]] and [[justice]].