# A Thermodynamic Framework for Understanding SGD Dynamics

## 1. Setup and Notation

### 1.1 Basic Variables

Statistical/Mathematical | Physics/Einstein | Description
------------------------|------------------|-------------
θ ∈ ℝᵈ                 | xᵢ               | Network parameters
L(θ)                   | V(x)             | Loss landscape (potential)
η                      | μ                | Learning rate (mobility)
D                      | D                | Diffusion constant
β = 1/T               | β = 1/kᵦT        | Inverse temperature
t                      | t                | Time
p(θ,t)                | ρ(x,t)           | Parameter distribution

### 1.2 SGD Dynamics

Statistical Form:
```
dθ = -η∇L(θ)dt + √(2D)dW
```

Einstein Notation:
```
dxᵢ = -μ∂ᵢV(x)dt + √(2D)dWᵢ
```

Where dW is a Wiener process representing batch noise.

## 2. Entropy Decomposition

### 2.1 System Entropy

The system entropy represents the information content of the parameter distribution:

Statistical:
```
s(t) = -ln p(θ(t),t)
```

Einstein:
```
s(t) = -ln ρ(x(t),t)
```

Information Theory Interpretation:
- This is the pointwise surprisal of the current parameter configuration
- Measures how "unlikely" the current state is under the evolving distribution
- Units are nats when using natural logarithm

### 2.2 Medium Entropy

The medium entropy represents the computational work done through parameter updates:

Statistical:
```
sm(t) = (1/T)∫₀ᵗ ∇L(θ)·dθ
```

Einstein:
```
sm(t) = (1/T)∫₀ᵗ ∂ᵢV(x)dxᵢ
```

Information Theory Interpretation:
- Represents information extracted from training data
- Each gradient step transfers information from data to parameters
- T scales the information content of each update

## 3. Fokker-Planck Evolution

The parameter distribution evolves according to:

Statistical:
```
∂ₜp(θ,t) = ∇·[η∇L(θ)p(θ,t) + D∇p(θ,t)]
```

Einstein:
```
∂ₜρ(x,t) = ∂ᵢ[μ∂ᵢV(x)ρ(x,t) + D∂ᵢρ(x,t)]
```

Information Theory Interpretation:
- First term: directed information flow from loss landscape
- Second term: diffusive information spreading from batch noise
- Balance determines exploration vs exploitation

## 4. Entropy Production Rate

### 4.1 Total Rate

Statistical:
```
s˙tot(t) = -∂ₜln p(θ,t) + (1/T)∇L(θ)·θ̇
```

Einstein:
```
s˙tot(t) = -∂ₜln ρ(x,t) + (1/T)∂ᵢV(x)ẋᵢ
```

### 4.2 Steady State Analysis

At loss convergence:
1. Loss stops changing: ∂ₜL(θ) ≈ 0
2. But parameters continue diffusing: θ̇ ≠ 0
3. Distribution keeps evolving: ∂ₜp(θ,t) ≠ 0

This gives steady-state entropy production:

Statistical:
```
⟨s˙tot⟩ = ∫ j(θ)²/[Dp(θ)]dθ > 0
```

Einstein:
```
⟨s˙tot⟩ = ∫ jᵢ(x)²/[Dρ(x)]dx > 0
```

Where j is the probability current in parameter space.

## 5. Distance Growth Prediction

The distance from initialization R(t) = ||θ(t) - θ(0)|| grows as:

```
R(t) ∝ exp(⟨s˙tot⟩t/d)
```

Where d is the parameter dimension. This predicts log-linear growth because:
1. Steady state entropy production rate ⟨s˙tot⟩ is constant
2. Taking log of both sides: ln R(t) ∝ t
3. This matches empirical observations

Information Theory Interpretation:
- Distance growth measures accumulated information from data
- Continues even after loss converges due to neutral directions
- Rate determined by balance of gradient and noise strength

## 6. Fluctuation Theorem

The system obeys Seifert's integral fluctuation theorem:

```
⟨exp(-Δstot)⟩ = 1
```

This implies:
1. Some trajectories can temporarily decrease entropy
2. But entropy-decreasing trajectories are exponentially suppressed
3. Average behavior still produces entropy
4. Sets fundamental bounds on training efficiency

Information Theory Interpretation:
- Places limits on how efficiently we can extract information from data
- Quantifies unavoidable computational costs of learning
- Similar to Landauer's principle relating computation and entropy