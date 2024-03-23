A continuity equation or transport equation is an equation that describes the transport of some quantity. It is particularly simple and powerful when applied to a conserved quantity, but it can be generalized to apply to any extensive quantity. Since mass, energy, momentum, electric charge and other natural quantities are conserved under their respective appropriate conditions, a variety of physical phenomena may be described using continuity equations.

Continuity equations are a stronger, local form of [[Conservation Laws]]. For example, a weak version of the law of conservation of energy states that energy can neither be created nor destroyed—i.e., the total amount of energy in the universe is fixed. This statement does not rule out the possibility that a quantity of energy could disappear from one point while simultaneously appearing at another point. A stronger statement is that energy is locally conserved: energy can neither be created nor destroyed, nor can it "teleport" from one place to another—it can only move by a continuous flow. A continuity equation is the mathematical way to express this kind of statement. For example, the continuity equation for electric charge states that the amount of electric charge in any volume of space can only change by the amount of electric current flowing into or out of that volume through its boundaries.
### Conservation of Mass: The Continuity Equation

In [[Fluid Dynamics]], the [[Conservation Laws|conservation]] of mass is expressed by the continuity equation. In its differential form for a fluid of density ($\rho$) and velocity field ($\vec{v}$), the continuity equation is written as:
$$ \frac{\partial \rho}{\partial t} + \nabla \cdot (\rho \vec{v}) = 0 $$
When translated into the language of [[Differential Forms]], the mass flux ($\rho \vec{v}$) can be represented by a differential form whose exterior derivative corresponds to the divergence term ($\nabla \cdot (\rho \vec{v})$). Integrating this form over a volume ($V$) and applying the [[Generalized Stokes' Theorem]] transforms the volume integral of the divergence into a surface integral over the boundary ($\partial V$) of the volume, representing the net flow of mass through the boundary:
$$
\int_{\partial V} \rho \vec{v} \cdot d\vec{A} = -\frac{d}{dt}\int_{V} \rho \, dV
$$
This equation states that the rate of mass leaving the volume through its boundary is equal to the negative rate of change of mass within the volume, encapsulating the principle of mass conservation in a [[Geometry|geometric]] form.

See also:
- [[Flux]]
- 