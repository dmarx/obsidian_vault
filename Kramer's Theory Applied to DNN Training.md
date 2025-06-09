# Kramers Theory Applied to Neural Network Training

## 1. Classical Kramers Theory

### 1.1 Basic Setup
In classical Kramers theory, we study a particle in a potential well subject to thermal noise:

```
mẍ + γẋ = -∇V(x) + √(2γkT)ξ(t)
```

where:
- m: particle mass
- γ: friction coefficient
- V(x): potential energy
- T: temperature
- ξ(t): white noise

### 1.2 Escape Rate
The escape rate from a metastable minimum at x₀ over a barrier at x* is:

```
k = (ω₀/2π)(ωᵦ/γ)exp(-ΔV/kT)
```

where:
- ω₀: well frequency = √|V''(x₀)|/m
- ωᵦ: barrier frequency = √|V''(x*)|/m
- ΔV = V(x*) - V(x₀)

## 2. SGD Mapping

### 2.1 Overdamped Limit
SGD corresponds to the overdamped limit (γ >> ω₀) of Kramers equation:

```
dθ = -η∇L(θ)dt + √(2ηT)dW
```

where:
- η: learning rate (replaces 1/γ)
- L(θ): loss landscape (replaces V(x))
- T: effective temperature from batch noise
- dW: Wiener process

### 2.2 Modified Escape Rate
In the SGD context, the escape rate becomes:

```
k_SGD = (ω₀ωᵦ/2πη)exp(-ΔL/T)
```

where:
- ω₀ = √|∇²L(θ₀)|: local minimum curvature
- ωᵦ = √|∇²L(θ*)|: saddle point curvature
- ΔL = L(θ*) - L(θ₀): barrier height

## 3. Effective Temperature in SGD

### 3.1 Temperature from Batch Noise
The effective temperature comes from batch sampling:

```
T = η⟨||∇L_B(θ) - ∇L(θ)||²⟩/2d
```

where:
- L_B: batch loss
- d: parameter dimension
- ⟨...⟩: batch average

### 3.2 Batch Size Dependence
For batch size B:

```
T ∝ η/B
```

This explains why larger batches need larger learning rates.

## 4. Transition State Theory for SGD

### 4.1 Reaction Coordinate
Define progress variable q(θ):

```
q(θ) = (θ - θ₀)·v*
```

where v* is the dominant eigenvector of ∇²L at the saddle.

### 4.2 Committor Probability
Probability of escaping to new minimum:

```
P(θ) = ∫_{-∞}^{q(θ)} exp(-βL(θ'))dq'/Z
```

where Z is the partition function.

## 5. Optimal Training Schedule

### 5.1 Critical Temperature
For each barrier:

```
T_c = ΔL/ln(τω₀)
```

where τ is available training time.

### 5.2 Annealing Schedule
Optimal temperature schedule:

```
T(t) = T_c(1 + ln(τ/t))/ln(τω₀)
```

This gives learning rate schedule:

```
η(t) = η₀(1 + ln(τ/t))/ln(τω₀)
```

## 6. Practical Implications

### 6.1 Escape Time Distribution
Time to escape local minimum:

```
P(t_escape > t) = exp(-kt)
```

### 6.2 Optimal Batch Size
For target escape rate k:

```
B_opt = η⟨||∇L_B(θ) - ∇L(θ)||²⟩/(2dkΔL)
```

### 6.3 Training Termination
Stop when:

```
k < 1/(remaining_time × compute_cost)
```

## 7. Multiple Barriers

### 7.1 Parallel Pathways
Total escape rate:

```
k_total = Σᵢ kᵢ
```

### 7.2 Sequential Barriers
Effective rate:

```
1/k_eff = Σᵢ 1/kᵢ
```

## 8. Loss Landscape Analysis

### 8.1 Barrier Height Estimation
From parameter diversity:

```
ΔL ≈ -T ln(|det(∇²L(θ₀))/det(∇²L(θ*))|)/2
```

### 8.2 Transition Path Sampling
Probability of trajectory θ(t):

```
P[θ(t)] ∝ exp(-∫(dθ/dt + η∇L(θ))²/4ηTdt)
```

This framework explains:
1. Why high learning rates can get stuck
2. How batch size affects exploration
3. When to reduce learning rate
4. Why some models train easier than others