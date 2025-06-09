see also:
- [[statistical physics]]
- [[Particle Physics]]
- [[Potential Theory]]
- [[Hydraulic Analogy]]
- [[Electrodynamics]]
- [[Electromagnetic Field Theory]]
- [[conserved quantities]]

Ohm's Law is a fundamental principle in [[electrical engineering]] and [[Physics]] that describes the relationship between voltage, current, and resistance in an electrical circuit. It states that the current ($I$) flowing through a conductor between two points is directly proportional to the voltage ($V$) across the two points and inversely proportional to the resistance ($R$) of the conductor. The law is mathematically expressed as:

$$ V = IR $$

where:
- $V$ is the voltage across the conductor (measured in volts, V),
- $I$ is the current flowing through the conductor (measured in amperes, A),
- $R$ is the electrical resistance of the conductor (measured in ohms, Ω).

### Derivation and Explanation

Ohm's Law can be derived from the basic principles of electromagnetism and the nature of electrical charge. Here's a step-by-step explanation:

1. **Electric Field and Potential Difference**: The electric field ($\vec{E}$) in a conductor creates a potential difference which drives the current. The voltage $V$ across the conductor is defined as the work done per unit charge to move the charge between two points, given by the integral of the electric field along the path of the conductor:
   $$ V = \int \vec{E} \cdot d\vec{l} $$

2. **Current and Charge Flow**: Current is defined as the rate of flow of electric charge. If $q$ is the charge and $t$ is the time, then current $I$ is given by:
   $$ I = \frac{dq}{dt} $$

3. **Conductivity and Resistance**: The electrical conductivity ($\sigma$) of a material describes its ability to conduct electric current. It is the reciprocal of the resistivity ($\rho$), which relates the electric field within the conductor to the current density ($\vec{J}$) by:
   $$ \vec{J} = \sigma \vec{E} $$
   For a uniform conductor with constant cross-sectional area $A$ and length $L$, the resistance $R$ is given by:
   $$ R = \frac{\rho L}{A} $$

4. **Relating Current and Voltage**: Combining these relations, for a uniform electric field and steady current, the voltage can be related directly to the current through the resistance:
   $$ V = IR $$

### Applications and Limitations

- **Applications**: Ohm's Law is widely used to analyze electrical circuits, to calculate the power dissipation using the formula $P = VI = I^2R = \frac{V^2}{R}$, and to design electrical and electronic equipment.
- **Limitations**: Ohm's Law holds accurately only for ohmic materials (those that have a linear relationship between voltage and current) and under steady-state conditions. Non-ohmic materials, such as diodes and transistors, do not follow Ohm's Law. Additionally, at very high frequencies or under very high voltage conditions, deviations from Ohm's Law can occur due to additional complex interactions in materials.

For deeper study, you might consider linking Ohm's Law to its microscopic basis via the [[Drude Model]], which explains electrical conduction using classical electron theory. This can also lead into discussions of quantum mechanical models in solid-state physics.