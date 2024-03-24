Flow models, also known as normalizing flows, represent a class of [[probabilistic models]] that aim to learn complex data distributions through a series of [[invertible]] and [[differentiable]] transformations. These models are a powerful tool in the landscape of generative modeling, providing a framework for explicitly modeling the probability density function of data. They stand out for their ability to exactly compute likelihoods, a feature that distinguishes them from other generative models like [[Variational Autoencoders]] (VAEs) and [[Generative Adversarial Networks]] (GANs).

### Core Principle

The core idea behind flow models is to transform a simple, known probability distribution (e.g., a [[Gaussian distribution]]) into a more complex distribution that closely matches the observed data. This transformation is accomplished through a sequence of invertible mappings, ensuring that each step is both [[reversible]] and differentiable. The term "flow" refers to the smooth transformation (or "flow") of probability densities through this sequence of [[mappings]].

### Mathematical Foundation

Mathematically, a flow model leverages the change of variables formula to relate the probability density of the complex target distribution to the simple base distribution. For an invertible transformation $f: \mathbb{R}^d \rightarrow \mathbb{R}^d$ that maps a base distribution $z \sim p_z(z)$ to a more complex distribution $x = f(z)$, the density of $x$ can be expressed as:

$$
p_x(x) = p_z(f^{-1}(x)) \left| \det \left(\frac{\partial f^{-1}}{\partial x}\right) \right|
$$

Here, $\left| \det \left(\frac{\partial f^{-1}}{\partial x}\right) \right|$ is the [[determinant]] of the [[Jacobian]] of the inverse transformation $f^{-1}$, accounting for the change in volume (or density) induced by the transformation.

### Types of Flow Models

Flow models can be categorized based on the specific type of transformations they employ:

- **Planar and Radial Flows**: Simple flows that introduce non-linearities through specific functional forms, useful for demonstrating the principles of flow models.
- **Coupling Flows**: Such as [[RealNVP]] and Glow, which divide the input into two parts and apply transformations to one part conditioned on the other. These models have been successful in generating high-quality images.
- **Autoregressive Flows**: Like [[PixelCNN]] and IAF (Inverse Autoregressive Flow), leverage autoregressive models to define complex, invertible transformations. They are powerful but can be computationally intensive due to their sequential nature.
- **Continuous Flows**: Represent transformations through differential equations, allowing for an infinite number of transformation steps. Notable examples include [[Neural Ordinary Differential Equations]] (Neural ODEs).

### Advantages

- **Exact Likelihood Evaluation**: Flow models allow for the direct computation of the likelihood of data points, facilitating model training and evaluation.
- **[[Invertibility]]**: The invertibility of transformations ensures that sampling and density estimation can be efficiently performed, a significant advantage over other generative models.
- **Flexibility**: They can model a wide range of distributions by stacking sufficient transformations, making them versatile tools for generative tasks.

### Applications

- **Data Generation**: Flow models are used to generate new data samples (e.g., images, audio) that resemble the training data.
- **[[Density Estimation]]**: They are effective in estimating the probability density of complex data, useful for anomaly detection and other statistical analysis tasks.
- **[[Variational Inference]]**: Flow models can serve as flexible variational posteriors in variational autoencoders, improving the expressiveness of VAEs.

### Conclusion

Flow models represent a powerful approach to probabilistic modeling, capable of capturing complex data distributions through a series of invertible transformations. Their ability to compute exact likelihoods and perform efficient sampling makes them valuable tools in the generative modeling toolkit, with wide-ranging applications from image generation to statistical analysis.