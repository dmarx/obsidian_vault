### Restricted Boltzmann Machines (RBMs)

Restricted Boltzmann Machines (RBMs) are a type of stochastic neural network that can learn a probability distribution over its set of inputs. Unlike standard Boltzmann Machines, RBMs have a simplified architecture that makes them more practical for certain machine learning tasks, such as feature extraction, dimensionality reduction, and generative modeling.

#### Structure of RBMs

1. **Two-Layer Network**
   - **Visible Layer**: Contains visible units (nodes) that represent the input data. Denoted as \( \mathbf{v} \).
   - **Hidden Layer**: Contains hidden units that capture latent features. Denoted as \( \mathbf{h} \).
   - **No Intra-Layer Connections**: There are no connections between units within the same layer (no visible-visible or hidden-hidden connections).

2. **Connections**
   - **Symmetric Weights**: Connections between visible and hidden units are symmetric, represented by a weight matrix \( W \) where \( w_{ij} \) is the weight between visible unit \( v_i \) and hidden unit \( h_j \).
   - **Bias Terms**: Each unit has a bias term, denoted by \( b_i \) for visible units and \( c_j \) for hidden units.

#### Energy Function and Probability Distribution

The energy function of an RBM defines the joint configuration of the visible and hidden units. The network aims to minimize this energy.

1. **Energy Function**
   - **Equation**:
     $$
     E(\mathbf{v}, \mathbf{h}) = -\sum_{i} b_i v_i - \sum_{j} c_j h_j - \sum_{i,j} v_i w_{ij} h_j
     $$
     where:
     - \( \mathbf{v} \) is the state vector of visible units.
     - \( \mathbf{h} \) is the state vector of hidden units.
     - \( b_i \) and \( c_j \) are the biases of visible and hidden units, respectively.
     - \( w_{ij} \) is the weight between visible unit \( i \) and hidden unit \( j \).

2. **Probability Distribution**
   - **Joint Probability**: The joint probability of a visible and hidden configuration is given by the Boltzmann distribution:
     $$
     P(\mathbf{v}, \mathbf{h}) = \frac{e^{-E(\mathbf{v}, \mathbf{h})}}{Z}
     $$
     where \( Z \) is the partition function, summing over all possible configurations of visible and hidden units.
   - **Marginal Probability**: The marginal probability of a visible configuration is:
     $$
     P(\mathbf{v}) = \sum_{\mathbf{h}} P(\mathbf{v}, \mathbf{h})
     $$

3. **Conditional Probabilities**
   - **Visible to Hidden**:
     $$
     P(h_j = 1 | \mathbf{v}) = \sigma\left(c_j + \sum_{i} v_i w_{ij}\right)
     $$
   - **Hidden to Visible**:
     $$
     P(v_i = 1 | \mathbf{h}) = \sigma\left(b_i + \sum_{j} h_j w_{ij}\right)
     $$
   where \( \sigma(x) \) is the sigmoid activation function \( \sigma(x) = \frac{1}{1 + e^{-x}} \).

#### Training RBMs

Training an RBM involves adjusting the weights and biases to maximize the likelihood of the training data. This is typically done using an approximation method known as Contrastive Divergence (CD).

1. **Contrastive Divergence (CD)**
   - **Objective**: Approximate the gradient of the log-likelihood to update the weights.
   - **Steps**:
     1. **Positive Phase**: Compute the expectation of the product of visible and hidden units' states using the training data.
     2. **Negative Phase**: Reconstruct the visible units by sampling from the hidden units, then compute the expectation of the product of visible and hidden units' states using the reconstructed data.
     3. **Weight Update**:
        $$
        \Delta w_{ij} = \eta \left( \langle v_i h_j \rangle_{\text{data}} - \langle v_i h_j \rangle_{\text{recon}} \right)
        $$
        where:
        - \( \eta \) is the learning rate.
        - \( \langle v_i h_j \rangle_{\text{data}} \) is the expectation under the data distribution.
        - \( \langle v_i h_j \rangle_{\text{recon}} \) is the expectation under the model distribution (reconstructed data).

2. **Bias Updates**
   - **Visible Bias**:
     $$
     \Delta b_i = \eta ( \langle v_i \rangle_{\text{data}} - \langle v_i \rangle_{\text{recon}} )
     $$
   - **Hidden Bias**:
     $$
     \Delta c_j = \eta ( \langle h_j \rangle_{\text{data}} - \langle h_j \rangle_{\text{recon}} )
     $$

#### Applications of RBMs

1. **Feature Learning**
   - **Unsupervised Learning**: RBMs can learn to represent the input data in terms of latent features, which can be used for classification, clustering, and other tasks.

2. **Dimensionality Reduction**
   - **Data Compression**: By learning a compact representation of the data, RBMs can reduce the dimensionality of the input while preserving important features.

3. **Collaborative Filtering**
   - **Recommender Systems**: RBMs can be used to model user preferences and recommend items by learning from the patterns of user interactions.

4. **Generative Modeling**
   - **Data Generation**: After training, RBMs can generate new data samples that resemble the training data by sampling from the learned distribution.

5. **Pre-training for Deep Networks**
   - **Layer-Wise Training**: RBMs can be used to pre-train layers of deep neural networks, improving convergence and performance in deep learning tasks.

#### Advantages and Limitations

1. **Advantages**
   - **Efficient Training**: The use of contrastive divergence makes RBMs relatively efficient to train compared to other probabilistic models.
   - **Versatility**: RBMs can be applied to a wide range of tasks, including unsupervised learning, feature extraction, and generative modeling.

2. **Limitations**
   - **Scalability**: RBMs can be challenging to scale to very large datasets and deep architectures without significant computational resources.
   - **Approximation**: The contrastive divergence algorithm is an approximation and may not always converge to the optimal solution.
   - **Interpretability**: The features learned by RBMs can be difficult to interpret, particularly in high-dimensional data.

### Conclusion

Restricted Boltzmann Machines (RBMs) are powerful tools for unsupervised learning and probabilistic modeling. They are particularly useful for feature learning, dimensionality reduction, and generative modeling. Understanding the structure, training mechanisms, and applications of RBMs provides valuable insights into their capabilities and limitations. For further exploration, consider examining related topics such as [[Boltzmann Machines]], [[Deep Belief Networks]], and [[Generative Models]].