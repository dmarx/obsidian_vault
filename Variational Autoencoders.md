---
tags:
  - green
---

see also:
- [[VAEs]]
- [[Denoising Autoencoders]]
- [[Encoder Decoder]]

Variational Autoencoders (VAEs) are a class of generative models that leverage the principles of variational inference to learn complex data distributions. Introduced by [[Diederik Kingma]] and [[Max Welling]] in 2013, VAEs stand at the intersection of deep learning and Bayesian inference, offering a powerful framework for modeling high-dimensional data through probabilistic latent variables. They are particularly noted for their ability to generate new data samples that are similar to the training data, making them useful in a wide range of applications including image generation, anomaly detection, and more.

### Structure of Variational Autoencoders

VAEs consist of two main components: the encoder and the decoder, structured as neural networks.

- **Encoder**: The encoder, also known as the recognition network, maps input data $x$ to a distribution over a latent space, typically a Gaussian distribution. This distribution is defined by parameters (mean $\mu$ and variance $\sigma^2$) that are functions of the input data, allowing the encoder to capture the underlying structure of the data. The encoder effectively approximates the posterior distribution $q_\phi(z|x)$ of latent variables $z$ given the data $x$.

- **Decoder**: The decoder, or generative network, aims to reconstruct the input data from the latent variables. It defines the likelihood of the data given the latent variables, $p_\theta(x|z)$, attempting to generate data that closely resembles the original input when sampled from the latent space.

### Training VAEs

The training objective of a VAE is to maximize the [[Evidence Lower Bound]] (ELBO), which serves as a proxy for maximizing the likelihood of the data under the model. The ELBO for a VAE can be written as:

$$
\text{ELBO} = \mathbb{E}_{q_\phi(z|x)}[\log p_\theta(x|z)] - \text{KL}(q_\phi(z|x) || p(z))
$$

- The first term is the expected log-likelihood of the data given the latent variables, encouraging the decoder to accurately reconstruct the data from the latent space.
- The second term is the [[KL Divergence|Kullback-Leibler divergence]] between the encoder's approximation of the [[posterior distribution]] and the [[prior distribution]] of the [[latent variables]], typically chosen to be a standard [[Gaussian distribution]]. This term acts as a [[regularizer]], ensuring that the [[latent space]] has good properties, such as [[continuity]] and [[completeness]].

### Properties and Applications

- **Generative Capability**: Once trained, VAEs can generate new data samples by sampling latent variables from the prior distribution and passing them through the decoder.

- **[[Latent Space Interpolation]]**: The structured latent space learned by VAEs allows for smooth interpolation between data points, making VAEs particularly useful for tasks like image manipulation, style transfer, and more.

- **[[Semi-supervised Learning]]**: The probabilistic framework of VAEs can be extended to semi-supervised learning scenarios, where the model can learn from both labeled and unlabeled data.

- **Anomaly Detection**: The reconstruction error from a VAE can serve as a [[Measure|metric]] for anomaly detection, where data points that the model struggles to reconstruct are considered anomalies.

### Challenges and Limitations

- **[[Posterior Collapse]]**: Sometimes, the model may ignore the latent variables (a phenomenon known as posterior collapse), especially if the decoder is too powerful.

- **Blurriness in Generated Samples**: VAEs are known to produce somewhat blurry samples compared to other generative models like GANs. This is partly due to the use of the [[reconstruction loss]], which averages over possible outputs.

- **Choice of Prior and Posterior**: The choice of the prior and approximate posterior distributions can significantly affect the performance of a VAE. Research into more flexible distributions (beyond the standard Gaussian) continues to be an active area of exploration.

Variational Autoencoders represent a significant advancement in unsupervised learning and generative modeling, combining deep neural networks with variational inference to model complex data distributions in a principled manner. Despite their challenges, VAEs continue to be a highly active area of research, with ongoing developments aimed at enhancing their generative capabilities and addressing their limitations.