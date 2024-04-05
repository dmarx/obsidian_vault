Kalman filters are a powerful set of mathematical equations providing an efficient computational means to estimate the state of a [[linear dynamic system]] from a series of noisy measurements. They are widely used in applications requiring real-time estimation and prediction, such as in navigation systems (GPS and INS), robotics, and signal processing, to name a few. The Kalman filter has the unique advantage of being recursive, meaning it can process measurements as they arrive, one at a time, without the need for the entire data set to be available from the start.

### Overview

Developed by Rudolf E. Kalman in 1960, the Kalman filter addresses two fundamental problems:
1. **Prediction**: Estimating the future state of a process based on a mathematical model of the physical system.
2. **Update**: Refining these estimates as new measurements become available.

### How It Works

The Kalman filter operates in two steps: predict and update.

- **Prediction Step**: The filter predicts the current state and error covariance estimates to obtain the prior estimated state. This step uses the process model of the system.

- **Update Step**: Once a new measurement is available, the filter updates its predictions based on the measurement to minimize the error in the estimated state. This step incorporates the measurement model of the system.

### Mathematical Formulation

The essence of the Kalman filter can be captured in the following set of equations, which are executed in a loop as new data becomes available:

1. **Prediction**:
   - Predicted State Estimate: $\hat{x}_{k|k-1} = F_k \hat{x}_{k-1|k-1} + B_k u_k$
   - Predicted Covariance Estimate: $P_{k|k-1} = F_k P_{k-1|k-1} F_k^T + Q_k$

   Where $\hat{x}_{k|k-1}$ is the predicted state estimate at time $k$ given the information up to time $k-1$, $F_k$ is the state transition model, $B_k$ is the control-input model, $u_k$ is the control vector, $P_{k|k-1}$ is the predicted estimate covariance, and $Q_k$ is the process noise covariance matrix.

2. **Update**:
   - Kalman Gain: $K_k = P_{k|k-1} H_k^T (H_k P_{k|k-1} H_k^T + R_k)^{-1}$
   - Updated State Estimate: $\hat{x}_{k|k} = \hat{x}_{k|k-1} + K_k (z_k - H_k \hat{x}_{k|k-1})$
   - Updated Covariance Estimate: $P_{k|k} = (I - K_k H_k) P_{k|k-1}$

   Here, $K_k$ is the Kalman gain, $H_k$ is the measurement model, $z_k$ is the measurement at time $k$, $R_k$ is the measurement noise covariance matrix, and $I$ is the identity matrix.

### Applications

- **Navigation and Tracking**: Kalman filters are extensively used in GPS and INS systems for accurate positioning and navigation.
- **Robotics**: For sensor fusion, where data from multiple sensors are combined to estimate the robot's position and orientation accurately.
- **[[Economics]] and Finance**: To estimate variables of interest, like GDP or stock prices, from noisy observations.
- **[[Control Theory|Control Systems]]**: For controlling the state of a process in real-time, adjusting the inputs based on the estimated state.

### Extensions and Variations

The original Kalman filter is designed for linear systems with Gaussian noise. Several extensions have been developed for more complex scenarios:
- **Extended Kalman Filter (EKF)**: Approximates non-linear systems by linearizing about the current mean and covariance.
- **Unscented Kalman Filter (UKF)**: Uses a deterministic sampling technique to capture the mean and covariance of a non-linear transformation of a probability distribution.
- **[[Particle Filter]]**: A more general approach that uses a set of particles (samples) to represent [[probability distributions]], capable of dealing with non-linear and non-Gaussian problems.

The Kalman filter's elegance lies in its simplicity, efficiency, and wide applicability, making it a cornerstone of modern control theory and signal processing.