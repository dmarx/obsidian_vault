---
tags:
  - needs-outlinks
  - sod/green
---

see also:
- [[Philosophy of Probability]]

The do-calculus is a formalism developed by [[Judea Pearl|Judea Pearl]] as part of his framework for causal inference, which allows researchers to mathematically analyze and draw conclusions about causal relationships from data. This calculus is a set of rules for manipulating expressions involving do-operators, which represent interventions in a causal model. The do-operator, denoted as $do(X=x)$, signifies an intervention where the value of a variable $X$ is set to $x$ by external means, distinguishing it from mere observation or conditioning on $X$ being $x$.

### Key Concepts of Do-Calculus

- **[[Causal Models]]**: Underlying the do-calculus is the concept of causal models, which are typically represented by [[directed acyclic graphs]] (DAGs). These models depict variables as nodes and causal relationships between them as directed edges. The models provide a visual and mathematical way to describe the assumptions about the [[causal structure]] of a system.

- **[[Interventions]]**: An intervention, represented by the do-operator, simulates the act of externally setting a variable to a specific value, irrespective of its previous causes. This is distinct from observing that variable in a particular state, as observation does not alter the underlying causal structure.

- **[[Counterfactuals]]**: Do-calculus facilitates reasoning about counterfactuals, which are statements about what would happen under hypothetical scenarios, including interventions. Counterfactual reasoning is essential for understanding the effect of changes in one part of a system on another.

### Rules of Do-Calculus

The do-calculus consists of three rules that allow for the transformation of expressions involving do-operators under certain conditions. These rules are designed to eliminate the do-operator and express the causal effect in terms of probabilities that can be estimated from observational data:

1. **Rule 1 (Insertion/Deletion of Observations)**: This rule allows for the insertion or removal of observations on variables that are not affected by the intervention, under certain conditions related to the graph structure.

2. **Rule 2 (Action/Observation Exchange)**: This rule allows for the exchange between actions (interventions) and observations when certain independence conditions are met.

3. **Rule 3 (Insertion/Deletion of Actions)**: This rule enables the insertion or deletion of actions under certain conditions, particularly when the action does not affect the variables under consideration.

### Applications and Impact

Do-calculus has profound implications for empirical research, as it provides a systematic way to identify the causal effects from observational data and to estimate the outcomes of potential interventions. Its applications span various fields, including epidemiology, economics, social sciences, and artificial intelligence. By formalizing causal inference, do-calculus helps to clarify the assumptions needed for causal conclusions, enhances the interpretability of statistical models, and guides the design of experiments and data analysis strategies.

In essence, do-calculus is a cornerstone of causal inference, offering a rigorous mathematical foundation for understanding and estimating causal effects, thereby bridging the gap between observational data and causal reasoning.