see also:
- [[Evolutionary Game Theory]]
- [[Evolution]]
- [[Evolutionary Dynamics]]
- [[Disruption]]

Disruptive selection, also known as diversifying selection, is a type of [[natural selection]] that favors extreme values of a trait over intermediate values. This form of selection can lead to increased genetic variance in a population and may eventually result in the formation of distinct subpopulations or even new species. Disruptive selection occurs when environmental conditions create multiple niches that favor individuals with extreme phenotypes.

## Mechanisms of Disruptive Selection

### Environmental Heterogeneity

Disruptive selection often arises in environments that have multiple distinct niches or resources. Each niche favors individuals with specific adaptations, leading to selection against intermediate phenotypes that do not perform well in any niche.

### Competition

Intraspecific competition can drive disruptive selection. When individuals with intermediate traits face higher competition for resources, those with extreme traits may have a competitive advantage in exploiting different resources or habitats.

### Predation

Predation pressure can also contribute to disruptive selection if predators preferentially target individuals with intermediate traits. In this case, individuals with extreme traits may have a higher survival rate.

## Mathematical Modeling of Disruptive Selection

### Fitness Function

Consider a population with a trait \( x \) that influences fitness. The fitness \( w(x) \) of individuals with trait \( x \) can be represented as a bimodal function:

$$
w(x) = 1 - \alpha (x - \mu_1)^2 + \beta (x - \mu_2)^2
$$

Here, \( \mu_1 \) and \( \mu_2 \) are the means of two distinct niches, and \( \alpha \) and \( \beta \) are selection coefficients. This function peaks at the extreme values \( \mu_1 \) and \( \mu_2 \), representing the two niches.

### Selection Gradient

The selection gradient \( g(x) \) indicates the direction of evolutionary change in the trait \( x \):

$$
g(x) = \frac{d w(x)}{d x}
$$

For the given fitness function:

$$
g(x) = -2 \alpha (x - \mu_1) + 2 \beta (x - \mu_2)
$$

### Evolutionary Dynamics

The change in the trait \( x \) over time can be modeled using the replicator dynamics or adaptive dynamics framework. Assuming the trait value evolves according to the selection gradient:

$$
\frac{d x}{dt} = g(x)
$$

In the case of disruptive selection, this differential equation will have stable equilibria at the extreme values \( \mu_1 \) and \( \mu_2 \) and an unstable equilibrium at the intermediate value.

### Adaptive Dynamics Perspective

In adaptive dynamics, the evolutionary trajectory of the trait \( x \) can be analyzed using the invasion fitness \( f(y, x) \) of a rare mutant with trait \( y \) in a resident population with trait \( x \):

$$
f(y, x) = w(y) - w(x)
$$

The selection gradient \( g(x) \) is given by:

$$
g(x) = \left. \frac{\partial f(y, x)}{\partial y} \right|_{y=x}
$$

In a disruptive selection scenario, \( g(x) \) will have a shape that pushes the trait values towards the extremes, creating conditions for potential branching.

## Examples of Disruptive Selection

### Finch Beak Size

One of the classic examples of disruptive selection is observed in the beak size of Darwin's finches on the Galápagos Islands. Finches with large beaks can crack hard seeds, while those with small beaks are better at handling small seeds. Intermediate beak sizes are less efficient at handling either type of seed, leading to selection for extreme beak sizes.

### Cichlid Fish

In African cichlid fish, different species exploit different feeding niches within the same lake. Some cichlids have evolved specialized jaws for scraping algae off rocks, while others have evolved for eating invertebrates or other fish. The diverse feeding strategies have led to disruptive selection and the emergence of distinct species.

### Plant Height

In certain environments, plant height may be subject to disruptive selection. For example, in a meadow with variable light conditions, short plants may be favored in shaded areas, while tall plants may be favored in open areas with more light. Intermediate-height plants may be less competitive in both environments.

## Evolutionary Consequences of Disruptive Selection

### Increased Genetic Variance

Disruptive selection increases genetic variance within the population by favoring multiple extreme phenotypes. This increased variance can provide a rich substrate for further evolutionary processes.

### Speciation

Over time, disruptive selection can lead to reproductive isolation and speciation. If individuals with extreme traits preferentially mate with similar individuals, this can create distinct genetic lineages and eventually result in the formation of new species.

### Niche Differentiation

Disruptive selection promotes niche differentiation, where different subpopulations exploit different ecological niches. This can reduce intraspecific competition and allow for the coexistence of multiple specialized forms within the same environment.

### Branching Points

In the context of adaptive dynamics, disruptive selection creates evolutionary branching points where a population can split into distinct subpopulations with different trait values. These branching points are critical for understanding the adaptive radiation and diversification of species.

## Mathematical Example: Evolution of Body Size

Consider a population with individuals of different body sizes \( x \). The fitness function might be bimodal due to the presence of two distinct ecological niches:

$$
w(x) = \exp\left(-\alpha (x - \mu_1)^2\right) + \exp\left(-\beta (x - \mu_2)^2\right)
$$

Here, \( \mu_1 \) and \( \mu_2 \) are the optimal body sizes for two niches, and \( \alpha \) and \( \beta \) determine the strength of selection around these optima.

The selection gradient \( g(x) \) is:

$$
g(x) = \frac{d w(x)}{d x} = -2 \alpha (x - \mu_1) \exp\left(-\alpha (x - \mu_1)^2\right) - 2 \beta (x - \mu_2) \exp\left(-\beta (x - \mu_2)^2\right)
$$

Solving \( \frac{d x}{dt} = g(x) \) gives the evolutionary dynamics of body size in the population. This can be analyzed to identify stable and unstable equilibria, and to predict how the trait distribution will evolve over time.

In summary, disruptive selection is a powerful evolutionary force that favors extreme trait values and can lead to increased genetic variance, niche differentiation, and speciation. Mathematical models, such as those used in adaptive dynamics, provide valuable insights into the conditions and consequences of disruptive selection in natural populations.