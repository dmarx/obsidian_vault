---
tags:
  - stub
  - green
---
see also:
- [[Hessian]]
- [[Fisher Information]]

Given two matrices \(A\) of size \(m \times n\) and \(B\) of size \(p \times q\), the Kronecker product \(A \otimes B\) is a block matrix of size \((mp) \times (nq)\), constructed as follows:

$$
A \otimes B = \begin{pmatrix}
a_{11}B & \cdots & a_{1n}B \\
\vdots & \ddots & \vdots \\
a_{m1}B & \cdots & a_{mn}B
\end{pmatrix}
$$

Each element \(a_{ij}\) of matrix \(A\) is multiplied by the entire matrix \(B\), leading to a larger matrix where the original structures of \(A\) and \(B\) are preserved and intertwined.