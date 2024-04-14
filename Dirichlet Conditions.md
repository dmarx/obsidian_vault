---
tags:
  - sod/gold
---

The Dirichlet conditions are a set of criteria that, if satisfied by a function, ensure that its [[Fourier Series]] converges at most points. Named after the German mathematician [[Peter Gustav Lejeune Dirichlet]], these conditions are used to determine whether a periodic function can be represented as a Fourier series in a manner that converges to the function itself at points of continuity and to the average of the left-hand and right-hand limits at points of discontinuity. The Dirichlet conditions for a function $f(t)$ over a period $T$ are as follows:

1. **[[Periodicity]]**: The function $f(t)$ must be periodic, meaning there exists a positive value $T$ such that $f(t + T) = f(t)$ for all $t$.

2. **[[Integrability]]**: The function $f(t)$ must be absolutely integrable over a period. This means the integral of the absolute value of $f(t)$ over one period must be finite:
   $$ \int_{t_0}^{t_0+T} |f(t)| dt < \infty $$
   for some starting point $t_0$. This condition ensures that the function doesn't "blow up" or diverge over its period.

3. **Finite Number of [[Discontinuities]]**: Within any one period, $f(t)$ must have a finite number of discontinuities. This allows for the function to be approximated accurately by the sine and cosine terms of the Fourier series, even though it may not converge exactly at the points of discontinuity.

4. **Finite Number of Extrema**: The function must have a finite number of maxima and minima within any period. This condition prevents functions that oscillate infinitely often within a finite interval, which would be impossible to accurately represent with a finite sum of sine and cosine functions.

5. **Bounded Variation**: In any interval, the total variation of $f(t)$ should be bounded. This technical condition, which is often implied if the other conditions are met, ensures that the function does not oscillate too wildly within a period.

When these conditions are met, the Fourier series of $f(t)$ converges to $f(t)$ at every point where $f(t)$ is continuous. At points where $f(t)$ is discontinuous, the Fourier series converges to the midpoint of the jump (i.e., the average of the left-hand and right-hand limits of $f(t)$ at the point of discontinuity).

These conditions, while not necessary for convergence, provide a useful guideline for when a Fourier series will represent a periodic function well. Modern mathematics has identified functions and circumstances where Fourier series can converge without strictly meeting all the Dirichlet conditions, but these conditions remain a foundational guideline in the study and application of Fourier analysis.