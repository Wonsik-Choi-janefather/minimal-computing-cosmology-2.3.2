# Chapter 30 Finite Jacobi Realization

The starting point is a positive generalized-Laguerre spectral density above threshold s₀. For α > −1, the density is normalizable; this study uses s₀ = 1, Λ² = 1, and α = 1/2. The continuum weights are positive and integrate to one.

$$
ρ(s) = \[(s−s₀)^α e^(−(s−s₀)/Λ²)\]/\[Γ(α+1)Λ^(2α+2)\] Θ(s−s₀)
$$

_Equation (5.3)_

Using x = (s−s₀)/Λ², the measure takes the form x^αe^(−x)/Γ(α+1). The three-term recurrence of generalized Laguerre polynomials orthogonal with respect to this measure determines a real symmetric Jacobi matrix.

The diagonal entries of the N×N Jacobi matrix are s₀ + Λ²(2n+α+1), and adjacent off-diagonal entries are Λ²√((n+1)(n+1+α)). Because the matrix is real symmetric, its eigenvalues are real and unitary finite-time evolution is exactly defined.

$$
(J_N)\_(nn)=s₀+Λ²(2n+α+1), (J_N)\_(n,n+1)=Λ²√((n+1)(n+1+α))
$$

_Equation (5.4)_

Choosing the first basis vector e₀ as the visible port makes the weight of each eigenvalue s\_j, by the spectral theorem, the square w\_j of its first component. Thus w\_j is nonnegative, the weights sum to one, and one rank-one collective port reads N hidden spectral nodes.

This structure does not declare the continuum to be N independent physical particles. It is Gaussian quadrature of the target spectral measure and a finite state-space realization. N is the approximation order, not the number of particles in nature.

The greatest strength of the Jacobi construction is that positivity and self-adjointness are not obtained as post hoc checks. They follow structurally from the measure and recurrence, blocking the risk of generating complex poles or negative spectral weights by arbitrary fitting.

## **Related Research**

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)
