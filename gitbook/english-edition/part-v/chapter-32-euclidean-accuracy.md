# Chapter 32 Euclidean Accuracy

The finite model's first test was performed on the Euclidean window Q² ∈ \[0,10]. Increasing the Jacobi order through N = 2, 4, 8, 16, and 32, the maximum relative error between the exact Stieltjes transform and finite resolvent was compared.

$$
δ_N = max\_(Q²∈\[0,10\]) \|G\_(N,E)−G_E\|/\|G_E\|
$$

_Equation (5.7)_

The errors were, respectively, 4.089 × 10^(−2), 4.746 × 10^(−3), 1.858 × 10^(−4), 1.623 × 10^(−6), and 1.763 × 10^(−9). At N = 32, the error falls to a few parts per billion within the specified window.

The observed fit log δ\_N ≈ −0.55N − 3.31 summarizes rapid convergence in this finite sample. It is not, however, a proven asymptotic theorem but an empirical fit for N = 2 through 32. The same slope is not guaranteed for different windows or values of α.

_log δ\_N ≈ −0.55N − 3.31 \[empirical]_ (5.8)

Numerical consistency between nodes and recurrence was also confirmed. Depending on order, differences between eigenvalues and quadrature nodes ranged from approximately 2.2 × 10^(−16) to 5.7 × 10^(−14), consistent with the stability of the double-precision calculation used.

Euclidean convergence is rapid because the Stieltjes kernel is smooth off the positive real axis and favorable for quadrature. This success must not be transferred directly into accuracy of long-time Lorentzian dynamics.

The exact assessment of this chapter is therefore fixed-window PASS. For the specified spectral density and Euclidean window, the finite Jacobi resolvent converges rapidly; completion at all scales and throughout the complex domain remains open.

## **Related Research**

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)
