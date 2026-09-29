# Chapter 33 Real-Time Tracking

The amplitude A(t) of the continuous spectrum decreases through phase mixing. A finite Jacobi system, however, is a finite sum of discrete eigenvalues and cannot reproduce irreversible decay forever. Recurrences and revivals appear after sufficiently long times.

The calculation defined T\_1% as the time before the relative error between continuous and finite amplitudes exceeded 1%. For N = 2, 4, 8, 16, and 32, the values were 0.43857, 0.96863, 1.69659, 2.67806, and 4.02408, respectively.

$$
T\_(1%) = sup{T : relative error ≤ 0.01 on \[0,T\]}
$$

_Equation (5.9)_

An empirical fit to these data is T\_1% ≈ 0.84√N − 0.72. Increasing the order fourfold tends to approximately double the reliable time. This equation, too, summarizes the five benchmark orders rather than constituting an asymptotic theorem.

_T\_(1%) ≈ 0.84√N − 0.72 \[empirical]_ (5.10)

The long-time mean survival plateau decreased through 0.700, 0.450, 0.3236, 0.2318, and 0.1650. As N increases, the mean magnitude of visible return decreases, but it does not become permanent continuum damping at finite N.

This result clarifies the boundary between simulation and realization. A finite closed system can imitate a continuous response extremely accurately within a specified time window, but it does not own irreversibility over infinite time or the thermodynamic arrow.

Adopting N as a physical cutoff therefore requires a tracking window longer than the observational period, the experimental invisibility of revivals, or coupling to an actual environment. Otherwise, the model remains a finite-window simulator.

## **Related Research**

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)
