see also:
- [[Ohm's Law]]

The Drude model, developed by Paul Drude in 1900, is a theoretical model in the field of solid-state physics that provides a classical explanation for the transport properties of electrons in metals. It's particularly useful for describing electrical and thermal conductivities in metals by treating the electrons as a gas of free particles subjected to random thermal motion.

### Key Assumptions of the Drude Model

1. **Free Electron Approximation**: Electrons in a metal are considered to be free and classical particles that can move almost without interaction with each other, except for collisions.
   
2. **Collisions**: Electrons experience collisions primarily with the atoms or ions in the metal lattice, which scatter them randomly. These collisions are assumed to be instantaneous and completely randomize the velocities of the electrons without any preferred direction.

3. **Relaxation Time**: Between collisions, electrons accelerate under the influence of an electric field. The average time between collisions is characterized by the relaxation time ($\tau$), which is a measure of the average time an electron travels before scattering.

### Mathematical Formulation

The fundamental equation describing the motion of electrons under the Drude model is:

$$ \vec{F} = m \vec{a} = -e \vec{E} - \frac{m \vec{v}}{\tau} $$

where:
- $\vec{F}$ is the net force acting on the electron,
- $m$ is the electron mass,
- $\vec{a}$ is the acceleration,
- $e$ is the elementary charge (positive value),
- $\vec{E}$ is the electric field,
- $\vec{v}$ is the drift velocity of the electrons,
- $\tau$ is the relaxation time.

This equation can be solved to find the steady-state velocity ($\vec{v}$) under the influence of an electric field, leading to:

$$ \vec{v} = -\frac{e \tau}{m} \vec{E} $$

### Electrical Conductivity

The current density $\vec{J}$, which is the amount of charge per unit area per unit time, is given by:

$$ \vec{J} = n e \vec{v} $$

where $n$ is the number of conduction electrons per unit volume. Substituting the expression for $\vec{v}$ from the Drude model, we get:

$$ \vec{J} = -\frac{n e^2 \tau}{m} \vec{E} $$

Defining the electrical conductivity $\sigma$ as:

$$ \sigma = \frac{n e^2 \tau}{m} $$

leads to the relation:

$$ \vec{J} = \sigma \vec{E} $$

### Limitations of the Drude Model

While the Drude model successfully explains the linear relationship between current density and electric field (Ohm's Law) and gives reasonable values for conductivity and the Hall effect, it has several limitations:

1. **Quantum Effects**: The Drude model ignores quantum mechanical effects, which are essential for understanding the behavior of electrons at smaller scales and lower temperatures.

2. **Temperature Dependence**: The model does not correctly predict the temperature dependence of resistivity in metals; resistivity decreases with temperature, whereas the Drude model would predict an increase as scattering (and thus collision frequency) should increase.

3. **Specific Heat**: The Drude model incorrectly predicts the electronic contribution to the specific heat of metals, as it does not take into account the Fermi-Dirac statistics governing electrons.

4. **Mean Free Path**: The simplifications regarding collision processes and mean free path do not always hold, particularly in metals with complex electronic structures.

Despite these shortcomings, the Drude model is a cornerstone in the study of conductive materials and lays the groundwork for more refined models, such as the Drude-Lorentz and the nearly-free electron models. For a deeper understanding, exploring how quantum corrections are incorporated in models like the [[Quantum Drude Model]] can provide insights into the behaviors that classical theories like Drude's fail to capture.