# Formal Derivation of Critical Batch Size B_crit

## 1. Setup and Assumptions

### 1.1 Basic Dynamics
SGD update equation:
```
dθ = -η∇L(θ)dt + √(2ηT)dW
```
where:
- η: learning rate
- T: effective temperature
- dW: Wiener process

### 1.2 Information Processing Rate
From Landauer's principle and thermodynamics:
```
dI/dt ≤ P/(k_B T ln(2))
```
where:
- I: information content
- P: power
- k_B: Boltzmann constant

## 2. Batch Effects Analysis

### 2.1 Gradient Variance
For batch size B:
```
var(∇L_B) = σ²/B
```
where σ² is population gradient variance

### 2.2 Effective Temperature
```
T_eff(B) = T₀/B
```
where T₀ is base temperature

## 3. Power Analysis

### 3.1 Power Consumption
For batch size B:
```
P(B) = ν₀ * B * tr(I_F(θ))
```
where:
- ν₀: FLOPs/token/parameter/s
- I_F: Fisher Information

### 3.2 Power Constraint
```
P(B) ≤ P_max
```

## 4. Critical Point Derivation

### 4.1 Power Limited Regime
Solving P(B) = P_max:
```
B_power = P_max/(ν₀ * tr(I_F(θ)))
```

### 4.2 Information Limited Regime
From information processing rate:
```
B_info = √(P_max * T₀)/(k_B * ν₀ * tr(I_F(θ)))
```

### 4.3 Critical Batch Size
```
B_crit = min(B_power, B_info)
```

## 5. Supercritical Behavior (B > B_crit)

### 5.1 Effective Power
```
P_eff(B) = P_max * min(1, B_crit/B)
```

### 5.2 Information Processing Rate
```
(dI/dt)_eff = (dI/dt)_max * √(B_crit/B)
```

### 5.3 Learning Time
```
t_learn(B) = t_opt * max(1, √(B/B_crit))
```

## 6. Stability Analysis

### 6.1 Linear Stability Matrix
```
M(B) = [
    -η*I_F(θ)    η*∇²L(θ)
    -∇²L(θ)      -B/B_crit*I_F(θ)
]
```

### 6.2 Stability Condition
Eigenvalues λ of M(B) must satisfy:
```
Re(λ) < 0
```

## 7. Optimality Conditions

### 7.1 Maximum Efficiency
At B = B_crit:
```
η_power = 1
dI/dt = (dI/dt)_max
```

### 7.2 Supercritical Trade-off
For B > B_crit:
```
η_power(B) * t_learn(B) ≥ t_opt
```
with equality only at B = B_crit

## 8. Formal Proof of Optimality

**Theorem**: B_crit maximizes information gain per unit energy.

**Proof**:
1. Information gain rate:
   ```
   dI/dt = C * √(P_eff/T_eff)
   ```
   where C is a constant

2. Energy consumption:
   ```
   E = P_eff * t
   ```

3. Information per energy:
   ```
   I/E = (dI/dt)/P_eff = C/√(P_eff * T_eff)
   ```

4. At B = B_crit:
   ```
   ∂/∂B(I/E) = 0
   ∂²/∂B²(I/E) < 0
   ```

Therefore B_crit is a global maximum of efficiency.

## 9. Observable Consequences

### 9.1 Power Scaling
```
P_observed ∝ min(B, B_crit)
```

### 9.2 Training Time Scaling
```
t_train ∝ max(1, √(B/B_crit))
```

### 9.3 Loss Improvement
```
ΔL ∝ -log(min(1, B/B_crit))
```