# Chapter 16 Renderer Path Independence

Suppose two rendering paths begin at the same physical boundary and reach the same boundary. Even if their intermediate slices, gauge choices, and orders of decomposition differ, the final observable content must not. WRRA calls this renderer path equivalence or path independence.

_R\_γ₁(B\_f,B\_i) ≃\_gauge R\_γ₂(B\_f,B\_i)_ (3.11)

This principle does not require all intermediate representations to be literally identical. Differences corresponding to gauge redundancy are allowed, but gauge-invariant observables must agree. Path independence therefore separates observable content from representational redundancy.

When small deformations are applied in different orders, their difference must close again into an allowed deformation. If a local slice can be embedded in a nondegenerate spacetime geometry, the hypersurface-deformation algebra supplies the kinematics of these deformations.

In the canonical representation, these deformations appear as first-class constraints. If the constraint algebra does not close, different slicing paths create different physical states or leave an anomaly. The renderer then fails to implement the same reality consistently.

$$
{H\[N\],H\[M\]} = D\[qᵃᵇ(N∂\_bM−M∂\_bN)\]
$$

_Equation (3.12)_

It would nevertheless be an overstatement to say that path independence directly produces the Einstein equations. It demands the necessary gauge and deformation structure. Which dynamical branch is selected depends on the canonical variables used, locality, differential order, and additional degrees of freedom.

This principle makes WRRA testable. One can measure differences among boundary observables calculated along different renderer paths; an implementation fails if a constraint anomaly or source-clock leakage remains.

## **Related Open Studies**

**Renderer Path Independence and the Einstein Branch of the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22124886](https://doi.org/10.5281/zenodo.22124886)
