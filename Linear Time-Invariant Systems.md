---
tags:
  - needs-outlinks
---

A Linear Time-Invariant (LTI) system is a cornerstone concept in [[control theory]], [[signal processing]], and [[Systems Engineering]], characterized by two principal properties: [[linearity]] and time invariance.

### Linearity

An LTI system is linear if it satisfies the principles of superposition and homogeneity:

- **[[Superposition]]**: The response caused by two or more stimuli is the sum of the responses that would have been caused by each stimulus individually. Mathematically, if input $x_1(t)$ produces response $y_1(t)$ and input $x_2(t)$ produces response $y_2(t)$, then for any constants $a$ and $b$, the system's response to $a x_1(t) + b x_2(t)$ is $a y_1(t) + b y_2(t)$.
- **[[Homogeneity]]** (or scaling): A scaling of the input leads to a proportional scaling of the output. That is, if input $x(t)$ produces output $y(t)$, then $ax(t)$ will produce $ay(t)$ for any scalar $a$.

### [[Time Invariance]]

A system is time-invariant if its behavior and characteristics do not change over time. This means that if an input $x(t)$ produces an output $y(t)$, then any time-shifted input $x(t - t_0)$ will produce a time-shifted output $y(t - t_0)$ for any time shift $t_0$. The system's response to a particular input is the same regardless of when the input is applied.

### Mathematical Representation

The behavior of LTI systems can be described by differential or difference equations for continuous and discrete systems, respectively. In the frequency domain, LTI systems can be represented more compactly by transfer functions or system functions.

- **Continuous Systems**: Described by linear differential equations. The relationship between the input signal $x(t)$ and the output signal $y(t)$ can be analyzed using the Laplace transform, resulting in a transfer function $H(s)$.
  
$$
H(s) = \frac{Y(s)}{X(s)}
$$

where $Y(s)$ and $X(s)$ are the Laplace transforms of $y(t)$ and $x(t)$, respectively.

- **Discrete Systems**: Described by linear difference equations. The Z-transform is used to analyze these systems, leading to a system function $H(z)$.

$$
H(z) = \frac{Y(z)}{X(z)}
$$

### Impulse Response and Convolution

- **Impulse Response**: For LTI systems, the impulse response, denoted as $h(t)$ for continuous-time systems or $h[n]$ for discrete-time systems, characterizes the system's output when the input is a Dirac delta function (continuous-time) or a Kronecker delta function (discrete-time). The impulse response encapsulates all the information needed to describe the system's behavior.
  
- **Convolution**: The output of an LTI system can be computed as the convolution of the input signal with the system's impulse response. For continuous-time systems, this is given by:

$$
y(t) = \int_{-\infty}^{\infty} x(\tau)h(t - \tau)d\tau
$$

For discrete-time systems:

$$
y[n] = \sum_{k=-\infty}^{\infty} x[k]h[n - k]
$$

### Frequency Response

The frequency response of an LTI system describes how the system responds to different frequencies of a sinusoidal input. It is derived from the system's transfer function by evaluating it at $s = j\omega$ (for continuous systems) or $z = e^{j\omega T}$ (for discrete systems), where $\omega$ is the angular frequency and $T$ is the sampling period.

### Applications

LTI systems theory is widely applicable across engineering disciplines. It's foundational in designing and analyzing electrical circuits, control systems, signal processing algorithms, communication systems, and more. The concepts of impulse response, frequency response, and transfer functions provide powerful tools for understanding and designing systems that operate reliably under a wide range of conditions.