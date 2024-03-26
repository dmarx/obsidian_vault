---
tags: []
---

Parseval's Theorem is a fundamental result in [[Fourier Analysis]] and signal processing that relates the total average power of a function to the sum of the squares of the coefficients in its Fourier series or [[Fourier Transform]] representation. It essentially states that the energy in a signal is preserved when transitioning between the time domain and the frequency domain. This theorem has important implications in various fields, including electrical engineering, physics, and mathematics, particularly in understanding the distribution of [[Energy]] across different frequency components of a signal.

### For [[Fourier Series]]

In the context of Fourier series for a periodic function $f(t)$ with period $T$ and [[Fourier Coefficients]] $a_n$ and $b_n$, Parseval's Theorem can be stated as follows:

$$ \frac{1}{T} \int_{0}^{T} |f(t)|^2 dt = \frac{a_0^2}{2} + \sum_{n=1}^{\infty} \left( a_n^2 + b_n^2 \right) $$

This equation shows that the total average power of the function over one period (left side) is equal to the sum of the squares of its Fourier coefficients (right side), including both the sine and cosine terms.

### For Fourier Transform

When dealing with non-periodic functions and using the Fourier Transform, Parseval's Theorem is expressed in terms of the continuous integral of the square of the function's magnitude over its entire domain, equating it to the continuous integral of the square of its Fourier transform's magnitude. For a function $f(t)$ and its Fourier Transform $F(\omega)$, the theorem is given by:

$$ \int_{-\infty}^{\infty} |f(t)|^2 dt = \frac{1}{2\pi} \int_{-\infty}^{\infty} |F(\omega)|^2 d\omega $$

This form of Parseval's Theorem implies that the total energy of the signal in the time domain is equal to the total energy in the frequency domain, normalized by $2\pi$.

### Applications and Implications

- **[[Signal Processing]]**: Parseval's Theorem is used in signal processing to analyze the energy distribution across frequencies, which is crucial in filtering, noise reduction, and system analysis.

- **Quantum Mechanics**: In quantum mechanics, Parseval's Theorem relates to the conservation of probability, as the integral of the square of the wave function's magnitude represents the total probability.

- **Communication Systems**: The theorem helps in the analysis of energy efficiency and signal integrity in communication channels, ensuring that the transmitted signal's energy is preserved.

- **Acoustics and Vibrations**: In acoustics, Parseval's Theorem is used to understand how sound energy is distributed across different frequencies, which is important for sound design, noise control, and audio analysis.

Parseval's Theorem underscores a fundamental principle of energy [[Conservation Laws|conservation]] within the context of Fourier analysis, highlighting the equivalence between time-domain and frequency-domain representations of functions and signals.