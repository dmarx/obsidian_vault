see also:
- [[Transport Phenomena]]
- [[Dimensional Analysis]]

The Péclet Number (\(Pe\)) is a dimensionless quantity used in the fields of [[fluid dynamics]] and mass/heat transfer. It characterizes the relative importance of [[advection]] to [[diffusion]] in transporting properties like heat, mass, or momentum within a flow. Essentially, the Péclet Number helps in understanding how a substance moves through a fluid, indicating whether the transport is dominated by bulk motion (advection) or by molecular diffusion.

### Definition

The Péclet Number is defined as the product of the Reynolds Number (\(Re\)) and the Prandtl Number (\(Pr\)) for heat transfer, or the Schmidt Number (\(Sc\)) for mass transfer:

- For **heat transfer**:
  
  $$Pe = Re \cdot Pr = \frac{uL}{\alpha}$$

  where \(u\) is the fluid velocity, \(L\) is a characteristic length scale (such as diameter of a pipe), and \(\alpha\) is the thermal diffusivity of the fluid.

- For **mass transfer**:
  
  $$Pe = Re \cdot Sc = \frac{uL}{D}$$

  where \(D\) is the mass diffusivity of the substance being transported.

### Interpretation

- **\(Pe \gg 1\)**: Advection (or convection) dominates the transport process. This means that the bulk motion of the fluid is the primary mechanism by which properties (heat, mass) are transported.
- **\(Pe \ll 1\)**: Diffusion dominates the transport process. Here, molecular diffusion is the primary means of transport, and the flow's bulk motion has little effect on the distribution of the property being transported.
- **\(Pe \approx 1\)**: Advection and diffusion contribute equally to the transport process.

### Applications

- **Environmental Engineering:** In modeling pollutant dispersion in water bodies or the atmosphere, the Péclet Number helps determine whether dispersion is primarily governed by the flow of the medium or by molecular diffusion.
- **Chemical Engineering:** In reactor design and process engineering, understanding the dominance of advection or diffusion is crucial for efficient mixing and reaction processes.
- **Heat Exchangers:** In the design and analysis of heat exchangers, the Péclet Number informs on the relative importance of convective heat transfer compared to conductive heat transfer.

### Practical Examples

- In a river, pollutants introduced at a point source might spread downstream primarily through the river's flow (high \(Pe\)), while diffusion plays a secondary role.
- In a thin film or a boundary layer where the fluid velocity is low, diffusion might dominate the transport of heat or mass (\(Pe \ll 1\)).

The Péclet Number is a versatile dimensionless quantity that bridges the understanding of physical phenomena across different scales and substances, providing insights into the mechanisms that govern the transport of properties within a fluid. Its utility spans across many disciplines, highlighting the interconnectedness of advection and diffusion processes in determining system behavior.