[[Systems Dynamics]] is a methodology and analytical approach used to understand and model complex systems, particularly those involving feedback loops, time delays, accumulations, and nonlinearities. Developed in the late 1950s by Jay Forrester at the Massachusetts Institute of Technology (MIT), Systems Dynamics seeks to illuminate how system structure influences behavior over time, facilitating the exploration of potential changes to system behavior through simulation and modeling. It is employed across various domains, such as business, public policy, environmental studies, and healthcare, to anticipate the behavior of complex systems under different scenarios and to design more effective policies and interventions.

### Core Concepts of Systems Dynamics

#### Stock and Flow Structures
- **Stocks**: Represent the accumulations within a system, such as the amount of water in a reservoir, population in a city, or capital in a business. Stocks change over time through the flow of resources or entities into and out of the stock.
- **Flows**: Define the rates at which stocks change, representing the movement into or out of stocks. Flows are influenced by decisions, policies, or natural processes.

#### Feedback Loops
Feedback loops are circuits of causation that lead back to themselves, either reinforcing (positive feedback) or balancing (negative feedback) the system's behavior. 
- **Reinforcing Feedback Loops** accelerate system behavior; for example, compound interest in a bank account leads to exponential growth of wealth.
- **Balancing Feedback Loops** aim to stabilize the system around a certain state or goal, such as a thermostat regulating room temperature.

#### Time Delays
Time delays are intervals between actions and their visible effects in a system. They are critical in determining the stability and responsiveness of systems, often causing oscillations or overshoots if not properly accounted for.

### Mathematical Modeling in Systems Dynamics

Systems Dynamics models are typically constructed using differential or difference equations to describe the rates of change in stocks due to flows. The basic mathematical representation involves equations that describe how flows affect stocks, coupled with equations that capture the feedback mechanisms influencing those flows. For instance, the rate of change of a stock $S$ can be described by:

$$\frac{dS}{dt} = I(t) - O(t)$$

where $\frac{dS}{dt}$ is the derivative of the stock $S$ over time, representing the net flow rate into the stock. $I(t)$ and $O(t)$ are the inflow and outflow rates at time $t$, respectively. 

These models can be simulated over time to study how systems evolve, identify leverage points, and test the impact of potential interventions. Simulation software for Systems Dynamics, like Vensim or Stella, allows users to construct complex models involving multiple interacting feedback loops and time delays, and to visualize the system's behavior over time through graphical outputs.

### Applications of Systems Dynamics

Systems Dynamics has been applied in various fields to address complex problems:
- **Environmental and Resource Management**: Modeling population growth, resource depletion, and environmental impacts to inform sustainable policies.
- **Healthcare**: Understanding the dynamics of disease outbreaks, patient flows in hospitals, and the impacts of public health interventions.
- **Business Strategy**: Analyzing market dynamics, product life cycles, and organizational change to improve strategic planning.
- **Public Policy**: Evaluating the long-term effects of policies on economic systems, education, and social issues.

Through its emphasis on the structural basis of system behavior and its capacity for holistic analysis, Systems Dynamics provides a powerful tool for decision-making and strategic planning in the face of complexity and uncertainty.