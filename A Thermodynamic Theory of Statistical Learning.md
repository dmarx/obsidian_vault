---
tags:
  - book-idea
  - sod/gold
  - sod/synthesis
  - oc/theory
  - OC/collaboration
  - OC/half-baked
---
see also:
* [[Information Thermodynamics]]
## Background
- see ["Entropy production along a stochastic trajectory and an integral fluctuation theorem" - Udo Seifert](https://arxiv.org/abs/cond-mat/0503686)
- [Claude - Deep Thoughts / Entropy Production and Fluctuation Theorems in Thermodynamics](https://claude.ai/chat/83bd4f78-2186-4e16-b047-ca7eaa1f30c2)
- [Claude - Deep Thoughts / Modeling NN Training Dynamics with Dissipation Fluctuation Theory](https://claude.ai/chat/4f1d0f67-27e1-4805-849e-e30cc4168ba6)
* reference for analysis of SGD as a diffusion process
* reference for parameter distance increase after convergence
* reference for critical batch size
* [Stochastic Simulation of Chemical Kinetics](https://www.dna.caltech.edu/courses/cs191/paperscs191/gillespie1.pdf)


## Claude Responses

* [[A Thermodynamic Framework for SGD Dynamics]]
* [[Seiffert Applied to SGD]]
* [[Error Bounds and Convergence Rates in SGD]]
* [[Fundamental Tradeoffs in Training]]

* [[Optimal Training Through the Lens of Thermodynamics]]
* [[Information Processing Rate and Training Dynamics]]

* [[Work and Power]]
* [[Maximum Power Training Limits]]
* [[Power-Time Tradeoff]]
* [[Stability-Limited Training Speed]]
* [[Critical Batch Size]]
* [[Supercritical Batch Size]]
* [[B_power vs B_info]]

* [[Fisher Information and Training Power]]
* [[Thermodynamic interpretation of Natural Gradient]]

* [[Conservation Laws in DNN Training]]
* [[Thermodynamics of Chinchilla]]
* [[Kramer's Theory Applied to DNN Training]]
* [[Learning Rate as a Thermal Parameter]]

* [[Fluctuation Dissipation framework for SGD]]
* [[Information Conductivity]]
* [[Information Thermodynamics via Gibbs Free Energy]]
* [[Gradient Magnitude, Machine Precision, and Bit-Level Information Flow]]
### Misc References

* [Measuring the Effects of Data Parallelism on Neural Network Training](https://www.jmlr.org/papers/volume20/18-789/18-789.pdf) - Empirical observation of the existence of a critical batch size
	* Papers referencing this: https://scholar.google.com/scholar?oi=bibs&hl=en&cites=12544556029233445066,3487261182134896571,15934798779379948142&as_sdt=5
* [Stochastic Thermodynamics of Learning](https://arxiv.org/pdf/1611.09428)
* [Stochastic time-evolution, information geometry and the Cram´er-Rao bound](https://arxiv.org/pdf/1810.06832) thermodynamic interpretation of fisher information


## Key Observations
* The existence of a critical batch size is a property of saturating the information carrying capacity of the parameter update operator (i.e .the gradient of the loss)
	* This predicts that models engineered to have gradients requiring many bits to express can potentially tolerate higher data parallelism before reaching the critical batch size
	* Could explain why local SGD has demonstrated improved time to convergence and tolerance for larger batch size than mini batch sgd - [DON’T USE LARGE MINI-BATCHES, USE LOCAL SGD](https://arxiv.org/pdf/1808.07217)
		* More evidence for benefit of local SGD: [Local SGD Converges Fast and Communicates Little](https://arxiv.org/pdf/1805.09767)
		* More: [ProxSkip: Yes! Local Gradient Steps Provably Lead to Communication Acceleration! Finally!](https://proceedings.mlr.press/v162/mishchenko22b/mishchenko22b.pdf)
		* more corroboration: [On the Linear Speedup Analysis of Communication Efficient Momentum SGD for Distributed Non-Convex Optimization](https://proceedings.mlr.press/v97/yu19d.html)
		* Lean on local SGD more in early training - [Adaptive Communication Strategies to Achieve the Best Error-Runtime Trade-off in Local-Update SGD](https://proceedings.mlsys.org/paper_files/paper/2019/hash/4a0151b47bd93c5de2a0b57831981a0d-Abstract.html)
		* Analysis of local "iterate bias" as an SDE drift term in local SGD - [Sharp Bounds for Federated Averaging (Local SGD) and Continuous Perspective](https://proceedings.mlr.press/v151/glasgow22a.html)
	* If we can establish measures of batch information capacity and update operation information capacity, we can understand the bottlenecks at play here analytically
		* **Hypothesis**: The maximum information gain of a given data batch should be proportional to the "heat" input needed to overfit to that batch
		* We can then relate this to the expected heat of an update to make inferences about efficiency of data utilization and useful batch size limitations
	* I.e. this explains the [gradient noise](https://arxiv.org/pdf/1812.06162) paper thermodynamically

* Continued divergence of the parameters from initialization despite convergence of the loss is consistent with modeling SGD as governed by langevin dynamics
	* This is consistent with the observations of [Directional convergence and alignment in deep learning](https://proceedings.neurips.cc/paper_files/paper/2020/hash/c76e4b2fa54f8506719a5c0dc14c2eb9-Abstract.html)
* Modeling local SGD by adding a "local drift" term to the SDE, we can escape some of the constraint imposed on us by the information bottleneck by distributing the per-update information across "federated" ranks, regaining information capacity for global updates
	* **Hypothesis**: we can further assist convergence by regularizing drift. A simple drift regularizer would be to use a moving average in the federated update operation. this would however have an impact on the update energy.
	* The eigenspace of the update jacobian can be used to quantify information transfer in the update. The diagonal and off-diagonal eigenspaces are subject to different dynamics - [Deep Learning Theory Review: An Optimal Control and Dynamical Systems Perspective](https://arxiv.org/pdf/1908.10920)
* Transferring information requires doing work. 


# Setting Up Notation
## Dimensional Analysis of Scaling Laws
Empirically (Chinchilla, Gopher), optimal compute budget $C$ has been observed to scale roughly proportional to the size of the model (number of parameters) $N$ and dataset (number of tokens) $D$, i.e. $C \propto N \cdot D$ or $C = k \cdot N \cdot D$. Using floating point operations (FLOPs) as our measure of compute, this implies the scaling factor $k$ is expressed in units of $\text{FLOP/token/parameter}$, which is analogous to a kind of computational density.
According to [[Landauer's principal]], There is a theoretical limit to the minimal energy required to irreversibly change one bit of information.
A FLOP can be interpreted as a potential opportunity to change the value of a parameter, and therefore FLOPs provide a natural upper bound on the information transmitted from the data to the model during training, and Landauer's principal gives us a lower bound on the energy required to accomplish this information transmission ([[Von Neumann - Landauer principal]]?)

yadda yadda... incorporating time into the discussion...
$k/s$ is analogous to a reaction rate term.

## Information Absorption Efficiency
Consider some model with parameters $\theta$, such that $\theta_0$ denotes the parameters at initialization, $\theta_t$ denotes the parameters at step $t$ of training, and $\theta_\infty$ denotes the parameters at convergence. Consider the mutual information between the parameters and the training data, $I(\theta, D)$. For notational simplicity, let's call this $I_D(\theta)$, to be read as the information contained in the parameters, with respect to the dataset. The theoretical maximum information gain from training is then $I_D(\theta_\infty) -  I_D(\theta_0)$. as $t \to \infty$, for convergent training we expect $I_D(\theta_\infty) -  I_D(\theta_t) \to 0$. Marginalizing over the data, we can restate this observation in terms of the information entropy of the parameters: $H(\theta_\infty) -  H(\theta_t) \to 0$. 

Let $\frac{d}{dt} I_D(\theta_t)$ denote the instantaneous rate of information uptake by the model at some training step $t$, and let $\frac{d}{dt}C$ denote the computational efficiency. 
Let $\eta_I(\theta_t)$ denote the information absorption efficiency of the parameters at training step $t$, per unit compute. Then $\eta_I(\theta_t,C) = \frac{dI_D(\theta_t)}{dC}$.
This relationship can be restated in the form of a proportionality constant $\eta(C)$ which relates the efficiency with which the system converts computational work into information absorption: $\frac{dI_D(\theta_t)}{dC} = \eta_I(\theta_t,C) = \eta(C) \cdot [I_D(\theta_\infty) -  I_D(\theta_t)]$.
Alternatively:  $\frac{dH(\theta_t)}{dC} = \eta(C) \cdot [H(\theta_\infty) -  H(\theta_t)]$.
Training convergence -- i.e. effective information saturation -- occurs at some critical $C$, $C_{crit}$, above which $\frac{dH(\theta_t)}{dC} \lt \epsilon$ for some positive $\epsilon \approx 0$.
Via dimensional analysis, we see that $\eta(C)$ is in units of $\frac{1}{\text{FLOPs}}$.

## Impacts of Gradient Accumulation on Information Efficiency
Treating the fitting procedure as a communication channel that transmits information from the data into the parameters, the channel capacity is a function of the (loss) gradient utilized for a given parameter update step. if an update step results in no parameters updated, then the data processed in that step did not transmit any new information into the model parameters. Concretely, we can interpret the number of bits that change during a parameter update as a measure of the information gained during the parameter update, and consequently, the magnitude of the gradient therefore serves as a measure of the information transmitted in that data processing step.
Consider a batch of $M$ samples $x_0, x_1, \dots x_m$. Let $\nabla f(x_i)$ denote the gradient with respect to a given sample, and let the magnitude (L2 norm) be given by $|\nabla f(x_i)|$.
Given some fixed learning rate, we want to know how the information transmitted per token (i.e. the per-sample normalized magnitude of the gradient) is affected by our choice of batch size. For the moment, let's assume noise-less data, i.e. our goal in this regime should be to transmit all of the information available in any given token. We'll extend this analysis to noisy data next.
With a batch size of 1, we have normal SGD. Each sample has its own gradient computed independently, and the per-sample normalized gradient magnitude is just the average magnitude of the gradients: $\frac{1}{m} \sum_{i=o}^m |\nabla f(x_i)| = E[|f(x_i)|]$.
With a batch size of $m$, we pool the respective per-sample gradients before we have a chance to observe the magnitude, yielding a single gradient with magnitude $|\frac{1}{m} \sum_{i=o}^m \nabla f(x_i)| = |E[f(x_i)]|$.
By Jensen's inequality -- $g(E[X]) \le E[g(X)]$ -- it is necessarily the case that $|E[f(x_i)]| = E[|f(x_i)|]$.
Further, we can quantify the gap here by invoking the central limit theorem (TODO), which reveals the magnitude of a batch gradient is expected to scale on the order of $\frac{1}{\sqrt{m}}$, which then is interpretable as our per-sample efficiency in the batch training regime.
Now, back to the real world, where the data is noisy.
Let $\bar{x_i} = x_i + \epsilon$ denote a noisy sample for some noise $\epsilon \sim N(\mu, \sigma)$, such that the "noiseless" sample is still denoted $x_i$ as above. For some noisy observation, we observe a gradient $\nabla f(\bar{x_i}) = \nabla f(x_i + \epsilon) = \dots$

## Communication Theory of Model Training
We can treat a parameter update as a message transmitted from the data to the parameters. The communication channel here is the gradient. The channel gain is the learning rate, and the channel capacity has a strict upper bound: the number of bits required to express the model parameters, i.e. the maximum information that could be communicated in a single update would result in flipping every bit in the model's learnable parameters. The gradient dimension therefore operates as a kind of information bottleneck, thresholding the information that could feasibly be transmitted. Above some threshold batch size (strictly smaller than the number of parameters), this channel capacity becomes saturated.
In practice, gradients become increasingly sparse as training progresses (i.e. magnitude increasingly concentrated in fewer components, i.e. fewer parameter bits change per update as training progresses). The channel still experiences a kind of saturation of useful information, which interacts with the gradient precision.

## Analogy to Chemical Kinetics
* Changing a bit is analogous to a "reaction"
* Bit precision imposes a lower bound on the "activation energy" of changing a parameter
* The "activity" of the system is the rate of change of parameters, which is in turn propotional to the gradient magnitude (although it can also be measured more directly by observing the bit-change activity of a training step).
* The learning rate operates like a temperature: reactions progress at higher temperature, and carefully controlling the temperature throughout the reaction generally increases the yield of "structure" produced (model generalizability ~ crystallization quality).
* We can accelerate the reaction by increasing the temperature, but then we risk reducing the yield.
* We can increase the yield (model quality) by annealing the temperature (update magnitude) slowly, but if we anneal too slowly we are just wasting energy.

References:
* Shannon 1948, A Mathematical Theory of Information
* Landauer, 1961, Irreversibility and Heat Generation in the Computing Process

## Reaction Kinetics of Deep Learning

We can model the learning procedure as a diffusion of information from a region of high concentration (the dataset) into a region of low concentration (the randomly initiatlized parameters) whose "volume" is a function of model capacity.
This analogy permits modeling of extremely nuanced dynamics, such as a low quality dataset catalyzing the activity of a more challenging dataset. But later. First, fundamentals.
Let $\nabla I = I_D(\theta_{\infty}) - I_D(\theta_t)$ denote the "information gradient".
[[Fick's laws of diffusion|Fick's first law]] gives the information flux as $J=D\nabla I$, where $D$ is a "diffusivity coefficient" that is proportional to the activity of the system. We can reasonably anticipate $D$ will take the form $D=\rho \eta^k$ or $D=\rho \text{exp}(-\eta^k)$, where $\rho$ is a transmitivity property of the medium akin to viscosity (probably corresponds to FLOPs/parameter activity, possibly interacting with how model topology affects gradient flow), $\eta$ is learning, and $k$ is some scaling power.
