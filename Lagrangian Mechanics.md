---
tags:
  - stub
  - sod/green
---

Lagrangian mechanics is based on the [[Principle of Stationary Action]] (also known as the principle of least action). It uses the [[Lagrangian]], $L$, a function that represents the difference between the kinetic energy, $T$, and potential energy, $V$, of a system:

$$
L = T - V
$$

The dynamics of the system are derived by finding the path for which the action, $S$, defined as the integral of the Lagrangian over time, is stationary (i.e., does not change for small variations of the path). This leads to the Euler-Lagrange equations:

$$
\frac{d}{dt} \left( \frac{\partial L}{\partial \dot{q}_i} \right) - \frac{\partial L}{\partial q_i} = 0
$$

where $q_i$ are the generalized coordinates of the system, and $\dot{q}_i$ are their time derivatives.