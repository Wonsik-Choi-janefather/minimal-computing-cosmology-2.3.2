# Chapter 34 The Recovery Cycle

Spectral simulation alone cannot test WRRA v1.2's recovery conditions. For this purpose, the total space is extended to the tensor product of a Jacobi spectral factor, a localization factor, and a syndrome qubit.

The selected recovery generator is an amplitude-damping-type Lindblad operator. It lowers syndrome excitation to the ground state through σ\_−; off-diagonal elements of the density matrix decay at rate κ/2 and population defects at rate κ.

$$
L_rec(ρ)=κ\[σ₋ρσ₊−½{σ₊σ₋,ρ}\]
$$

_Equation (5.11)_

The corrective gap in the syndrome-transverse sector is Δ\_corr,N = κ/2. This value is independent of Jacobi order N and recovery sequence. It is an exact-in-construction gap obtained because the recovery factor is separated from the spectral chain. The unitary recurrence of the Jacobi sector remains, however, so this does not mean that the full Liouvillian is mixing.

$$
Δ\_(corr,N)=κ/2 \[syndrome-transverse sector\]
$$

_Equation (5.12)_

This recovery does not reverse the normal temporal evolution of the spectral amplitude. It removes errors in the syndrome factor while preserving the intended unitary evolution of the Jacobi sector, following WRRA's principle that recovery does not restore every change to its initial condition.

Factorization is nevertheless a strong assumption. In an actual microscopic renderer, interactions may occur among the spectral, localization, and syndrome sectors, reducing the uniform gap or creating new leakage.

What passes here is therefore the existence of a recovery channel and the exact calculation of its gap. Simulation error and recovery error have not yet been controlled over long times by one coupled inequality.

## **Related Research**

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)
