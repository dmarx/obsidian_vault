see also:
- [[Information Flow Across Capacity-Limited Computational Media]]

>  assume a fixed time budget (GPU hours) to train a model. assume unrestricted access to unique tokens. assume that every time we increase the batch size by a factor of `k`, the loss-decrease-per-sample (i.e. the sample efficiency) decreases by a factor of `1/sqrt(k)`. increasing batch size can potentially increase throughput, but up to a point there are dimensioning returns, i.e. there exists some sweet-spot batch size that maximizes throughput efficiently to result in the most time-efficient training that achieves the smallest loss achievable within the constraint of the time budget.
## Problem Formalization

Given:
- Fixed time budget $T$ (in GPU-hours)
- [[Loss function]] $\mathcal{L}(\theta)$ to be minimized
- Base batch size $b_0$
- Base throughput rate $r_0$ (samples/second at $b_0$)
- Base sample efficiency $e_0$ (loss decrease per sample at $b_0$)

## Efficiency-Batch Size Relationship

For batch size $b = kb_0$, the [[sample efficiency]] follows:

$e(k) = \frac{e_0}{\sqrt{k}}$

This reflects the empirical observation that larger batch sizes reduce the information gained per sample.

## Throughput-Batch Size Relationship

The [[computational throughput]] typically follows:

$r(k) = r_0 \cdot f(k)$

where $f(k)$ is a [[hardware utilization function]] that depends on:
- [[Memory bandwidth]]
- [[Computational parallelism]]
- [[Hardware architecture]]

Common approximation:
$f(k) = \min(k, k_{\text{max}})$ where $k_{\text{max}}$ is the [[hardware saturation point]]

## Total Progress Metric

The [[training progress]] $P$ over time $T$ can be expressed as:

$P(k) = T \cdot r(k) \cdot e(k)$

Substituting the relationships:

$P(k) = T \cdot r_0 \cdot f(k) \cdot \frac{e_0}{\sqrt{k}}$

## Optimal Batch Size

To find the optimal $k^*$, solve:

$k^* = \arg\max_k P(k)$

Taking the derivative:

$\frac{d P}{dk} = T r_0 e_0 \left(\frac{f'(k)}{\sqrt{k}} - \frac{f(k)}{2k^{3/2}}\right)$

### Case Analysis

1. Pre-saturation $(k < k_{\text{max}})$:
   - $f(k) = k$
   - $f'(k) = 1$
   - Optimal $k_1^* = 4$ 

2. Post-saturation $(k \geq k_{\text{max}})$:
   - $f(k) = k_{\text{max}}$
   - $f'(k) = 0$
   - No local maximum

Therefore:
$k^* = \min(4, k_{\text{max}})$

## Practical Implementation

The [[optimal batch sizing algorithm]]:

1. Measure base metrics:
   ```python
   b0 = minimum_viable_batch_size()
   r0 = measure_throughput(b0)
   e0 = measure_efficiency(b0)
   ```

2. Determine hardware saturation:
   ```python
   k_max = find_throughput_plateau()
   ```

3. Set optimal batch size:
   ```python
   k_opt = min(4, k_max)
   b_opt = b0 * k_opt
   ```

## Trade-off Analysis

The key trade-offs involved:

1. [[Memory-Compute Trade-off]]:
   - Larger batches → Better hardware utilization
   - Until [[memory bandwidth]] saturates

2. [[Statistical-Computational Trade-off]]:
   - Larger batches → Lower sample efficiency
   - But higher throughput up to saturation

3. [[Time-Quality Trade-off]]:
   - Fixed time budget
   - Need to maximize (throughput × efficiency)

## Optimization Extensions

1. [[Dynamic Batch Sizing]]:
   - Adjust batch size during training
   - Based on loss landscape characteristics

2. [[Gradient Accumulation]]:
   - Simulate larger batches
   - Without memory overhead

3. [[Mixed-Precision Training]]:
   - Increase effective batch size
   - Through reduced precision computation

## Theoretical Guarantees

Under mild assumptions about the [[loss landscape]]:

1. [[Convergence Rate]]:
   $\mathbb{E}[\|\nabla \mathcal{L}(\theta_T)\|^2] \leq \mathcal{O}\left(\frac{1}{\sqrt{T \cdot P(k^*)}}\right)$

2. [[Generalization Bound]]:
   $\mathbb{E}[\mathcal{L}_{\text{test}}] - \mathcal{L}_{\text{train}} \leq \mathcal{O}\left(\sqrt{\frac{k^*}{n}}\right)$

where $n$ is the dataset size.