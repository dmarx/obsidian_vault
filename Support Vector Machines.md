see also:
- [[Discriminative Models]]
- [[Separating Hyperplane]]
- [[Decision Threshold]]
- [[Statistical Learning Theory]]

Support Vector Machines (SVMs) are a powerful class of supervised machine learning models used for classification and regression tasks. They are particularly well-known for their effectiveness in high-dimensional spaces and for cases where the number of dimensions exceeds the number of samples. SVMs are based on the concept of finding a hyperplane that best separates classes of data in a feature space.

### Mathematical Foundations

#### Hyperplane and Margin

The goal of an SVM is to find the optimal hyperplane that separates classes of data points with the maximum margin. The margin is defined as the distance between the hyperplane and the nearest data points from each class, known as support vectors. Mathematically, a hyperplane in an $n$-dimensional space is defined by the equation:
$$ w \cdot x + b = 0 $$
where:
- $w$ is a weight vector (normal to the hyperplane),
- $x$ is a feature vector,
- $b$ is a bias term.

The objective is to maximize the margin around the hyperplane, where the margin can be expressed as $\frac{2}{\|w\|}$. The problem thus reduces to minimizing $\|w\|^2$ under the constraints that the data points $x_i$ are classified correctly, formulated as:
$$ y_i (w \cdot x_i + b) \geq 1 \quad \text{for all } i $$
where $y_i \in \{-1, 1\}$ are the class labels.

#### Soft Margin and Kernel Trick

- **Soft Margin:** To allow SVM to handle non-linearly separable data and to manage outliers, the concept of a soft margin is used. This is achieved by introducing slack variables $\xi_i \geq 0$, leading to the modified constraints:
  $$ y_i (w \cdot x_i + b) \geq 1 - \xi_i $$
  The objective function also gets an additional term $C \sum \xi_i$, where $C$ is a regularization parameter that controls the trade-off between achieving a low error on the training data and maintaining a large margin.

- **[[Kernel Trick]]:** For non-linear classification, SVMs use the kernel trick to transform the input space into a higher-dimensional space where a linear separator might exist. A kernel function $K(x_i, x_j)$ computes the inner product of vectors $i$ and $j$ in this higher-dimensional space without ever computing the coordinates in that space explicitly. Common kernels include the polynomial kernel, radial basis function (RBF), and sigmoid kernel.

### Algorithmic Steps

1. **Feature Mapping:** Map data to a potentially higher-dimensional space using a kernel if non-linear separation is needed.
2. **Optimization:** Solve the optimization problem to find the hyperplane parameters $w$ and $b$ that maximize the margin and satisfy the constraints for classification.
3. **Decision Function:** Classify new data points based on the sign of $w \cdot x + b$.

### Applications and Implications

- **Classification Tasks:** SVMs are widely used for binary classification problems in various fields such as image recognition, bioinformatics (e.g., cancer classification), and text categorization.
- **Regression Tasks:** SVM regression (SVR) uses a similar principle but the goal is to fit the error within a certain threshold.
- **Anomaly Detection:** SVMs can be adapted for use in anomaly detection by finding the smallest sphere (in feature space) that contains the data.

### Conclusion

Support Vector Machines represent a robust approach to supervised learning, particularly attractive for its capacity to handle complex, high-dimensional data and its effectiveness in achieving high accuracy with a clear margin of separation. This has made SVMs a popular choice in both academia and industry for tackling a wide range of data-intensive classification and regression tasks.