---
tags:
  - sod/green
  - needs-outlinks
---
see also:
- [[Signal Processing]]
	- images in frequency domain
	- sound in frequency domain
	- timeseries prediction in frequency domain

The Fourier Transform is a mathematical operation that transforms a function of time (or space) into a function of frequency, providing a frequency domain representation of the original time-domain function. This transformation is essential in various fields of science and engineering, especially where the analysis of frequency components is crucial, such as in signal processing, physics, electrical engineering, and quantum mechanics.

### Mathematical Definition

For a given function $f(t)$, where $t$ represents time, the Fourier Transform $F(\omega)$, with $\omega$ representing angular frequency, is defined as:

$$ F(\omega) = \int_{-\infty}^{\infty} f(t) e^{-i\omega t} dt $$

The [[Inverse Fourier Transform]], which reconstructs the original function $f(t)$ from its frequency domain representation $F(\omega)$, is given by:

$$ f(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} F(\omega) e^{i\omega t} d\omega $$

These equations describe how any (sufficiently well-behaved) function can be decomposed into a continuous superposition of sine and cosine waves (or, equivalently, complex exponentials) of various frequencies, amplitudes, and phases.

### Key Properties

- **[[Linearity]]**: The Fourier Transform is linear, meaning that the transform of a sum of functions is the sum of their transforms. This property is crucial for analyzing systems that can be decomposed into simpler components.
  
- **Time-Frequency Duality**: A compact (narrow) function in the time domain becomes a broad function in the frequency domain, and vice versa. This principle is known as the [[Uncertainty Principle]] in the context of signal processing and quantum mechanics.

- **[[Convolution Theorem]]**: The Fourier Transform turns convolution in the time domain into multiplication in the frequency domain, greatly simplifying the analysis of linear time-invariant systems.

- **[[Parseval's Theorem]]**: As previously discussed, this theorem relates the total [[Energy]] (or power) of a signal in the time domain to the total energy in the frequency domain, preserving energy across the transformation.

### Applications

- **[[Signal Processing]]**: Fourier Transforms are used to analyze the frequency content of signals, design filters, and study the response of systems to different frequencies.

- **Image Processing**: In image analysis, the Fourier Transform is used for filtering, image compression, and pattern recognition.

- **Quantum Mechanics**: The Fourier Transform relates the position and momentum representations of quantum states, embodying the principle of wave-particle duality.

- **Acoustics**: It's used to analyze sound waves, understanding the spectral content of audio signals, and designing acoustical systems.

- **Communication**: Fourier analysis is fundamental in modulating and demodulating signals for transmission over various media.

The Fourier Transform is a powerful tool that unveils the frequency spectrum of signals and functions, providing deep insights into their structure and behavior that are not apparent in the time or space domain. Its ubiquity in scientific and engineering disciplines underscores its fundamental importance in analyzing and understanding complex phenomena.