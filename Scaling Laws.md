---
tags:
  - empty-hub
  - green
  - gold
  - stub
---
Yes, apart from the well-known [[Rushbrooke's equality]], [[Widom's scaling law]], and [[Fisher's Scaling Law]], there are several other scaling laws and relations in the theory of critical phenomena that further elucidate the interdependencies among critical exponents. These scaling laws help in understanding the universal behavior near critical points and in characterizing phase transitions. Here are a few notable ones:

### [[Hyperscaling Relation]]

The hyperscaling relation connects the critical exponents \(\nu\), \(d\) (the dimensionality of the system), and \(\alpha\) (related to the specific heat):

$$ d\nu = 2 - \alpha $$

This relation suggests that the singular part of the free energy density scales with the correlation length. Hyperscaling is particularly relevant in lower dimensions and may break down in higher-dimensional systems due to upper critical dimensionality constraints.

### Josephson's Scaling Law

Named after the British physicist Brian D. Josephson, this scaling law relates the correlation length exponent \(\nu\) to the shift in the critical temperature \(T_c\) with the system size \(L\) in finite-size scaling analysis:

\[ T_c(L) - T_c(\infty) \sim L^{-1/\nu} \]

Josephson's scaling law is instrumental in finite-size scaling analyses, where it's used to estimate critical temperatures and exponents from numerical simulations of finite systems.

### Griffiths-Kelly-Sherman (GKS) Inequalities

While not directly a scaling law, the GKS inequalities provide bounds on the correlation functions and their derivatives, establishing relationships that must be satisfied near the critical point. These inequalities are useful in proving the existence of phase transitions and in studying the behavior of spin systems.

### Scaling Relations for Dynamical Exponents

In addition to the static critical phenomena described by the aforementioned exponents, there are dynamical critical phenomena characterized by dynamical exponents like \(z\), which describe the critical slowing down of dynamics near the critical point:

\[ \tau \sim \xi^z \]

where \(\tau\) is the relaxation time and \(\xi\) is the correlation length. The dynamical exponent \(z\) relates the time scales of fluctuations to the spatial correlation length, providing insight into how quickly a system near criticality returns to equilibrium after a disturbance.

### Ohta-Jasnow-Kawasaki (OJK) Scaling Law

In the context of phase ordering kinetics, the OJK scaling law provides a way to understand the growth of domains following a quench to below the critical temperature. It predicts that the characteristic domain size \(R(t)\) grows with time \(t\) as:

\[ R(t) \sim t^{1/z} \]

This law is particularly relevant for systems undergoing phase separation and is a cornerstone in the study of coarsening dynamics.

### Kadanoff's Scaling Picture

While not a scaling law per se, Leo Kadanoff's scaling picture forms the conceptual foundation for understanding critical phenomena and scaling laws. Kadanoff's idea of block-spin transformations, where spins are grouped into blocks to effectively study the system at different scales, underpins the RG approach and has been instrumental in deriving the scaling laws mentioned above.

These scaling laws and relations, derived from the renormalization group theory and scaling hypothesis, are crucial for a deep understanding of the critical phenomena observed in various physical systems, from magnetic materials and superconductors to liquid-gas transitions and beyond. They highlight the intrinsic connections between different physical quantities as systems approach criticality, revealing the universal nature of phase transitions.