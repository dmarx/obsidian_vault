# Stability-Limited Training Speed

## 1. Characteristic Time Scales

### 1.1 Power Time Scale
From raw power limit:
```
τ_power = ΔI/(P_max/(k_B T ln(2)))
```

### 1.2 Stability Time Scale
From parameter dynamics:
```
τ_stability = √(λ_max(I_F(θ))/η_max)
```
where:
- λ_max(I_F): largest eigenvalue of Fisher Information
- η_max: maximum stable learning rate

## 2. Instability Mechanisms

### 2.1 Fast Mode Instability
For update frequency ω:
```
ω > √(2/λ_max(I_F(θ))) ⟹ instability
```

### 2.2 Mode Coupling
Coupling strength:
```
g = ⟨∂²L/∂θᵢ∂θⱼ⟩
```
Instability when:
```
g > g_c = 1/τ_stability
```

## 3. Power vs Stability Limits

### 3.1 Power-Limited Updates
Maximum power-limited update size:
```
|Δθ|_power = √(P_max * dt/tr(I_F))
```

### 3.2 Stability-Limited Updates
Maximum stable update size:
```
|Δθ|_stable = 1/√λ_max(I_F)
```

### 3.3 Critical Comparison
**Key Point**: Always find
```
|Δθ|_stable < |Δθ|_power
```
at sufficiently high power

## 4. Why Stability Dominates

### 4.1 Information Geometry
1. Parameter space curvature sets minimum update time
2. No amount of power can violate causality in information propagation
3. Updates must respect local geometric structure

### 4.2 Lyapunov Analysis
For perturbation δθ:
```
d|δθ|²/dt ≤ (2η_max λ_max(I_F) - 2/τ_stability)|δθ|²
```
Stability requires:
```
η_max < 1/(τ_stability * λ_max(I_F))
```

## 5. Practical Implications

### 5.1 Maximum Learning Rate
```
η_max = min(
    P_max/(|∇L|² * tr(I_F)),  # Power limit
    1/(τ_stability * λ_max(I_F))  # Stability limit
)
```

### 5.2 Batch Size Limit
```
B_max = min(
    B_crit,  # Power limit
    1/(η_max * λ_max(I_F))  # Stability limit
)
```

## 6. Testing for Limits

### 6.1 Power-Limited Regime
```
|Δθ| ∝ √P_max
```

### 6.2 Stability-Limited Regime
```
|Δθ| = constant
```
regardless of power increase

### 6.3 Diagnostic
If increasing power doesn't speed up training:
```
Stability_limited = (∂t_train/∂P_max ≈ 0)
```