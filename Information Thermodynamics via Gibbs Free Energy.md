# Information Thermodynamic Framework

## Free Energy Decomposition
The information processing capacity expressed as Gibbs free energy:

$$
\Delta G_{info} = \Delta H_{info} - T\Delta S_{info}
$$

where:
- $\Delta H_{info} = -\sum_i p_i \log \frac{p_i}{q_i}$ (relative entropy between learned and true distributions)
- $\Delta S_{info} = -\sum_i p_i \log p_i$ (Shannon entropy of parameter distribution)

## Multi-Dataset Competition
For competing datasets, the chemical potential of information:

$$
\mu_i = \frac{\partial G_{info}}{\partial N_i} = k_BT\log\left(\frac{\theta_i}{1-\theta_i}\right) + \sum_j \phi_{ij}\theta_j
$$

where $\phi_{ij}$ represents information interaction potentials between datasets.

## Equilibrium Conditions
At equilibrium:

$$
\sum_i \mu_i\delta N_i = 0
$$

with constraint:
$$
\sum_i \theta_i \leq C_{capacity}
$$

where $C_{capacity}$ is the model's information capacity.

## Information Flow
The rate of information transfer:

$$
J_i = L_{ij}(\nabla\mu_j - T\nabla s_j)
$$

where $L_{ij}$ is the Onsager coefficient matrix and $s_j$ is the specific entropy.