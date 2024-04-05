Principal Component Analysis (PCA) is a statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components. This transformation is defined in such a way that the first principal component has the largest possible variance (that is, accounts for as much of the variability in the data as possible), and each succeeding component in turn has the highest variance possible under the constraint that it is orthogonal to the preceding components. The resulting vectors are an uncorrelated orthogonal basis set. PCA is sensitive to the relative scaling of the original variables.

### Key Concepts and Steps

1. **Standardization**: Often, the initial step in PCA is to standardize the data so that each feature contributes equally to the analysis. This involves subtracting the mean and dividing by the standard deviation for each value of each variable.

2. **Covariance Matrix Computation**: The next step is to compute the covariance matrix of the data. The covariance matrix expresses the correlation between the different variables in the dataset.

3. **[[Spectral Decomposition|Eigenvalue Decomposition]]**: PCA involves decomposing the covariance matrix into its eigenvalues and eigenvectors. The eigenvectors of the covariance matrix represent the directions (or principal components) of the data that maximize the variance of the data, while the eigenvalues represent the magnitude of these directions.

4. **Selection of Principal Components**: The principal components are ranked according to their eigenvalues, with the first principal component corresponding to the direction of greatest variance, the second principal component corresponding to the direction of the second greatest variance, and so on. The number of principal components kept for further analysis is often chosen based on the cumulative explained variance, which should ideally be as high as possible (commonly set to a threshold like 95%).

5. **Transformation to New Space**: Finally, the original data is projected onto the principal components (the eigenvectors of the covariance matrix) to transform it into the new space. This results in a set of orthogonal vectors over which the original data is now expressed.

### Applications

- **[[Dimensionality Reduction]]**: PCA is widely used for dimensionality reduction in data preprocessing for machine learning models when the number of input features (variables) is too high. It helps to avoid the curse of dimensionality and reduce computational cost.

- **Visualization**: PCA is used for visualizing high-dimensional data by reducing it to 2D or 3D.

- **[[Noise Reduction]]**: By keeping only the most significant principal components and ignoring the ones with lower variance, which are likely to correspond to noise, PCA can help in filtering noise from the data.

- **[[Feature Extraction]] and Engineering**: PCA can be used to derive new features that are a linear combination of the original features but with better properties, such as being uncorrelated and capturing the essence of the data.

Despite its wide range of applications, PCA has limitations, such as assuming linearity, being sensitive to the scale of the data, and not necessarily capturing the intrinsic structure of the data if the relationships are nonlinear. Advanced techniques like kernel PCA or autoencoders may be used to overcome some of these limitations, especially for complex or non-linear datasets.

>fundamentally, PCA is just a rotation

Yes, at its core, Principal Component Analysis (PCA) can be understood as a rotation and transformation of the coordinate system of the data. This rotation is performed in such a way that the new axes (the principal components) align with the directions of maximum variance in the data, with the first principal component pointing in the direction of the greatest variance, the second principal component orthogonal to the first and pointing in the direction of the next highest variance, and so on.

### Geometric Interpretation

1. **[[Rotation]]**: The process of PCA involves rotating the original axes (features) of the data space to new axes that better capture the variance in the data. This rotation does not alter the relative positioning of the data points themselves; rather, it changes the reference frame in which the data is described.

2. **Transformation**: After the rotation, the data is projected onto the new axes (the principal components), which transforms the original data into a new space. This new coordinate system has the property that the coordinates (principal component scores) are uncorrelated, and the dimensions are ordered by the amount of variance they capture from the original data.

### Mathematical Perspective

Mathematically, this rotation is achieved by computing the eigenvectors of the covariance matrix of the data. These eigenvectors form an orthogonal basis set for the new coordinate system. Multiplying the original data by the matrix of eigenvectors (where each column is an eigenvector) rotates the data into this new space.

### Key Properties

- **[[Orthogonality]]**: The principal components are orthogonal to each other, meaning that in the new coordinate system formed by PCA, the axes are perpendicular. This orthogonality also ensures that the principal components are linearly uncorrelated.

- **[[Variance]]**: The principal components are ordered by the amount of original variance they capture, with the first principal component capturing the most variance, and each subsequent component capturing less. The total variance in the data is preserved in the transformation.

- **[[Dimensionality Reduction]]**: By selecting a subset of the principal components (typically those capturing most of the variance), PCA allows for effective dimensionality reduction. This subset provides a lower-dimensional representation of the data that still captures most of its variability.

### Applications and Implications

- **Data Visualization**: PCA is often used to reduce high-dimensional data to two or three dimensions for visualization purposes. The rotation and transformation make it possible to view the data from the perspective of its main sources of variance.

- **[[Feature Selection]] and Extraction**: In machine learning and statistics, PCA aids in feature selection and extraction, providing a smaller set of features (principal components) that can be used for further analysis, thereby simplifying models and reducing overfitting.

The geometric interpretation of PCA as a rotation and transformation of the [[data space]] helps to intuitively understand how PCA works and why it is a powerful tool for data analysis, allowing us to view and interpret data in terms of its most significant patterns and structures.