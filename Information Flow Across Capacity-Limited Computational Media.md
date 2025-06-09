>  information flow across a gradient mediated by a computational medium with limited communication capacity

see also:
- [[Reaction Rate Density in Deep Learning Thermodynamics]]

## Formal Definition

Let $\mathcal{M}$ be a [[computational medium]] connecting two regions $A$ and $B$ with an [[information gradient]] $\nabla I$ between them. The medium has a finite [[communication capacity]] $C(\mathcal{M})$ that constrains the rate at which information can propagate across it.

## Mathematical Framework

The [[information flow]] $J_I$ across the medium can be modeled as:

$J_I = -D(\mathcal{M}) \nabla I$

where:
- $D(\mathcal{M})$ is the [[diffusion coefficient]] representing the medium's ability to transmit information
- $\nabla I$ is the spatial gradient of information density

This follows the form of [[Fick's first law]] but applied to information rather than particle diffusion.

## Capacity Constraints

The actual flow is bounded by the medium's capacity:

$|J_I| \leq C(\mathcal{M})$

This creates a [[bottleneck effect]] when the potential flow exceeds capacity:

$J_I^{\text{actual}} = \min(|D(\mathcal{M}) \nabla I|, C(\mathcal{M})) \cdot \text{sign}(\nabla I)$

## Information Accumulation

The temporal evolution of information density follows a [[modified diffusion equation]]:

$\frac{\partial I}{\partial t} = \nabla \cdot (D(\mathcal{M}) \nabla I)$ subject to $|J_I| \leq C(\mathcal{M})$

This creates characteristic behaviors:
1. [[Information pooling]] at boundaries when flow exceeds capacity
2. [[Gradient steepening]] near capacity-limited regions
3. [[Temporal decorrelation]] of information packets due to transmission delays

## Computational Implications

The capacity limitation introduces several key effects:

### Temporal Effects
- [[Processing latency]] $\tau_p \propto \frac{L^2}{D(\mathcal{M})}$ where $L$ is the characteristic length
- [[Information decay]] due to finite storage capacity
- [[Packet fragmentation]] when flow exceeds capacity

### Spatial Effects
- Formation of [[information gradients]]
- Development of [[bottleneck regions]]
- [[Spatial quantization]] of information density

## Applications

This framework applies to various domains:
- [[Neural information processing]]
- [[Distributed computing networks]]
- [[Quantum information transport]]
- [[Biological signaling networks]]

## Optimization Strategies

Several approaches exist for optimizing flow through capacity-limited media:

1. [[Gradient engineering]]: Controlling $\nabla I$ to maximize flow while respecting capacity
2. [[Adaptive routing]]: Dynamically adjusting paths based on local capacity
3. [[Temporal multiplexing]]: Interleaving different information streams
4. [[Compression coding]]: Reducing effective information density

## Theoretical Bounds

The [[maximum achievable throughput]] $T_{\text{max}}$ is bounded by:

$T_{\text{max}} \leq \min(C(\mathcal{M}), D(\mathcal{M}) \|\nabla I\|_{\infty})$

This creates a fundamental trade-off between:
- [[Gradient steepness]]
- [[Medium capacity]]
- [[Diffusion rate]]

The optimal balance depends on specific application constraints and requirements.