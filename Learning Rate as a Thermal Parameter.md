# Modified Information Kinetics Model

## Fundamental Relations
Information flux for dataset i:
J_i = -D_i(η)∇μ_i

Diffusion coefficient scales with learning rate:
D_i(η) = D_i⁰exp(-E_i/η)

## Competition Dynamics
Occupancy evolution:
dθ_i/dt = k_i(η)(1-Σθ_j) - r_i(η)θ_i

where:
- k_i(η): absorption rate ∝ exp(-E_i/η)
- r_i(η): desorption rate ∝ η

## Steady State 
For cosine-annealed η(t):
θ_i* = K_i(η)α_i / (1 + ΣK_j(η)α_j)

where K_i(η) is effective equilibrium constant at learning rate η.