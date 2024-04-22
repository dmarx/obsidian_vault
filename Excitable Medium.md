### Definition of Excitable Medium

An **excitable medium** is a type of mathematical model used to describe systems that can exhibit [[self-sustaining]] [[wave propagation]] due to a local excitation response. These media are characterized by their ability to propagate a response over a distance far greater than the dimension of the initial disturbance, without an external input. Excitable media are commonly studied in contexts like cardiology, neurology, and chemical reactions, particularly in the study of phenomena such as cardiac arrhythmias, neural wave propagation, and the [[Belousov-Zhabotinsky reaction]].

### Mathematical Description

The dynamics of an excitable medium can be modeled using partial differential equations (PDEs) that describe the spatial and temporal evolution of state variables. A common model used to describe such a system is the [[FitzHugh-Nagumo model]], a simplification of the [[Hodgkin-Huxley model]] that describes nerve membrane action potentials. The FitzHugh-Nagumo model is composed of two equations:

1. **Voltage equation** (describes the electric potential across the membrane):
   $$\frac{\partial v}{\partial t} = v - \frac{v^3}{3} - w + D_v \nabla^2 v$$

2. **Recovery equation** (describes the recovery variable, which models processes that restore the system to its rest state):
   $$\frac{\partial w}{\partial t} = \epsilon (v + a - bw)$$

Here, $v$ represents the [[membrane potential]], $w$ is a recovery variable, $D_v$ is the diffusion coefficient for the potential, $\nabla^2$ is the [[Laplace Operator|Laplacian operator]] representing diffusion through the medium, and $\epsilon$, $a$, and $b$ are parameters that can be adjusted to fit specific biological or chemical conditions. The terms involving $v^3$ introduce nonlinearity, crucial for the excitability of the medium.

### Properties and Characteristics

- **[[Threshold Dynamics]]**: Excitable media have a threshold property; a small perturbation will decay, while a perturbation exceeding the threshold will initiate a self-propagating wave.
- **[[Refractory Period]]**: After an excitation, the medium enters a refractory period during which its ability to propagate further waves is either reduced or completely inhibited. This prevents the back-propagation of waves and is crucial for the unidirectional flow of signals in neural and cardiac tissues.
- **Wave Propagation**: In two or three dimensions, excitable media can support [[complex wave phenomena]], including [[spiral waves]] or [[target patterns]], which are often observed in both biological and chemical systems.

### Applications

- **Cardiology**: Modeling of cardiac tissue as an excitable medium helps to understand the propagation of electrical waves in the heart and the mechanisms behind arrhythmias.
- **Neuroscience**: Excitable media models are used to study the propagation of action potentials along nerve fibers and across brain structures.
- **Chemical Reactions**: The Belousov-Zhabotinsky reaction, a chemical oscillation of a stirred reaction mixture, is often studied as an excitable medium due to its wave propagation properties.

For a detailed understanding of the mathematical and physical implications of these models, a deeper dive into the FitzHugh-Nagumo model or other related models like the [[Hodgkin-Huxley model]] and [[Reaction-Diffusion Systems|reaction-diffusion systems]] would be beneficial. These models provide a rich framework for exploring the non-linear dynamics characteristic of excitable media.