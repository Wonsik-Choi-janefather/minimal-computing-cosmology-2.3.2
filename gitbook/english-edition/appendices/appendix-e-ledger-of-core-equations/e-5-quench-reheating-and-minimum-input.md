# E-5 Quench, Reheating, and Minimum Input

## 17. Continuous transfer in an effectively stiff background

$$\rho_{s} = \rho_{*}A^{- 6}\exp\left\lbrack - \frac{\kappa}{3}\left( A^{3} - 1 \right) \right\rbrack$$

**Meaning** An exact sequence in which a post-opening kinetic-dominated stiff component attenuates through expansion and decay.\
**Scope** H=H\*A⁻³, constant transfer rate Γ, κ=Γ/H\*.\
**Grade** EXACT in the stated stiff-transfer model\
**Basis** 10.5281/zenodo.22182366

## 18. Radiation accumulation in a stiff background

$$\rho_{r} = \rho_{*}A^{- 4}\kappa\int_{1}^{A}x\exp\left\lbrack - \frac{\kappa}{3}\left( x^{3} - 1 \right) \right\rbrack dx$$

**Meaning** The expansion-inclusive cumulative energy transferred from the decaying stiff component into the radiation sector.\
**Scope** The same background and transfer rate as Eq. 17.\
**Grade** EXACT\
**Basis** 10.5281/zenodo.22182366

## 19. Slow-transfer approximation at stiff–radiation equality

$$A_{eq} = 0.9335516614\,\kappa^{- 1/3},\quad\frac{T_{eq}}{T_{*}} = 1.0009587908\,\kappa^{1/2}$$

**Meaning** For κ≪1, gives the scale factor and temperature at which radiation catches up with the stiff component.\
**Scope** The slow-transfer limit under stiff domination and constant transfer.\
**Grade** ASYMPTOTIC EXACT\
**Basis** 10.5281/zenodo.22182366

## 20. Coupled scalar–radiation system

$$\ddot{\sigma} + (3H + \Gamma)\dot{\sigma} + V\prime(\sigma) = 0,\quad{\dot{\rho}}_{r} + 4H\rho_{r} = \Gamma{\dot{\sigma}}^{2},\quad 3{\bar{M}}_{P}^{2}H^{2} = \frac{{\dot{\sigma}}^{2}}{2} + V(\sigma) + \rho_{r}$$

**Meaning** Scalar dissipation and radiation production are coupled by Γσ̇², not Γρσ. This exact system is the starting point for distinguishing the stiff interval from the quadratic-oscillation interval.\
**Scope** A homogeneous canonical scalar, constant Γ, and flat FLRW.\
**Grade** EXACT in the restricted model\
**Basis** 10.5281/zenodo.22182366

## 21. Matter-like scalar solution after quadratic oscillation

$$\rho_{\sigma} = \rho_{o}A^{- 3}\exp\left\lbrack - \frac{2\kappa_{o}}{3}\left( A^{3/2} - 1 \right) \right\rbrack$$

**Meaning** Near a quadratic minimum, where the mean equation of state is wσ=0, scalar energy on the assumed scalar-dominated background decays as A⁻³ times an exponential decay factor.\
**Scope** H=H\_oA⁻³ᐟ², κ\_o=Γ/H\_o, and ρσ(A=1)=ρ\_o. The radiation contribution to the Friedmann equation is omitted from the background equation.\
**Grade** EXACT SOLUTION ON THE ASSUMED SCALAR-DOMINATED BACKGROUND\
**Basis** 10.5281/zenodo.22182366

## 22. Radiation accumulation in the matter-like interval

$$\rho_{r} = \rho_{o}A^{- 4}\kappa_{o}\int_{1}^{A}x^{3/2}\exp\left\lbrack - \frac{2\kappa_{o}}{3}\left( x^{3/2} - 1 \right) \right\rbrack dx$$

**Meaning** An integral solution in which energy lost by the oscillating scalar accumulates as radiation on the assumed scalar-dominated background.\
**Scope** The same mean matter-like background as Eq. 21. Radiation backreaction near equality is not included.\
**Grade** EXACT ON THE ASSUMED BACKGROUND; NOT A FULL TWO-COMPONENT CLOSURE\
**Basis** 10.5281/zenodo.22182366

## 23. Slow-transfer approximation at matter–radiation equality

$$y_{m} = 1.6094969705952367,\quad A_{eq} = 1.3733886134\,\kappa_{o}^{- 2/3},$$

$$\frac{T_{eq}}{T_{o}} = 0.60277557043\,\kappa_{o}^{1/2}$$

**Meaning** For κ\_o≪1, an asymptotic estimate of the scale and temperature at which radiation catches up with the scalar after quadratic oscillation. Near equality, coupled integration including the radiation Friedmann term is required.\
**Scope** averaged wσ=0, slow-transfer, scalar-dominated background approximation.\
**Grade** ASYMPTOTIC EQUALITY ESTIMATE; NOT A FULL TWO-COMPONENT NUMERICAL CLOSURE\
**Basis** 10.5281/zenodo.22182366

## 24. Preliminary BBN benchmark and minimum κ\_o

$$\kappa_{o,\min} = \left\lbrack \frac{T_{req}}{0.60277557043\, T_{o}} \right\rbrack^{2},\quad T_{req} = 5\, MeV$$

**Meaning** A fixed benchmark that takes T\_req=5 MeV as a formal required temperature and calculates a lower bound on κ\_o. The previously presented number is the arithmetic value obtained by fixing g\*=106.75 over the entire interval; it is not a precision physical BBN boundary at 5 MeV.\
**Scope** Restricted matter-like completion, T\_req=5 MeV, and fixed-g\*=106.75 benchmark. Actual BBN requires g\*(5 MeV)≈10.75, changes in entropy degrees of freedom, and integration of the coupled system.\
**Grade** PRELIMINARY CONDITIONAL BBN BENCHMARK\
**Basis** 10.5281/zenodo.22182366

## 25. Two stiff-to-matter intervals and decay rate

$$m_{\sigma} = \sqrt{2\lambda}\,{\bar{M}}_{P},\quad H_{o} \simeq m_{\sigma},\quad\frac{\Gamma}{m_{\sigma}} = 2C_{SM}\lambda \ll 1$$

**Meaning** If mσ/H\*≪1, the system passes through a kinetic/stiff interval N\_stiff≃(1/3)ln(H\*/mσ) before entering the oscillatory interval at H\_o≈mσ. If mσ/H\*≥1, it enters matter-like oscillation immediately.\
**Scope** V=λ(σ²−M̄\_P²)²/4 and restricted Standard Model coupling. For Γ/mσ≪1, the matter-like approximation governs the BBN benchmark.\
**Grade** CONDITIONAL TWO-REGIME APPROXIMATION; FULL COUPLED INTEGRATION OPEN\
**Basis** 10.5281/zenodo.22182366

## 26. Lower bound on λ in the fixed-g\* benchmark

$$q_{m} = \sqrt{\frac{\pi^{2}g_{*}}{90}}\frac{T_{req}^{2}}{(0.60277557043)^{2}{\bar{M}}_{P}^{2}} = 3.97048310136 \times 10^{- 41},$$

$$\lambda_{\min} = \frac{1}{2}\left( \frac{q_{m}}{C_{SM}} \right)^{2/3}$$

**Meaning** Calculates lower bounds on λ and mσ/M̄\_P for each C\_SM in a benchmark fixing g\*=106.75 and T\_req=5 MeV. The numbers in the existing table remain arithmetically valid under this assumption.\
**Scope** L\_int=−\[(σ−M̄\_P)/M̄\_P]T^μ\_μ, Γ=C\_SM mσ³/M̄\_P², fixed g\*=106.75. The actual 5 MeV boundary requires g\*≈10.75, entropy changes, and full integration of the coupled system.\
**Grade** PRELIMINARY CONDITIONAL NUMERICAL BENCHMARK; NOT A PHYSICAL BBN CLOSURE\
**Basis** 10.5281/zenodo.22182366\
Fixed benchmark values For C\_SM=1, 1/(8π), 10⁻³, and 10⁻⁶: λ\_min=5.81923067×10⁻²⁸, 4.99296834×10⁻²⁷, 5.81923067×10⁻²⁶, and 5.81923067×10⁻²⁴; mσ/M̄\_P=3.41151892×10⁻¹⁴, 9.99296586×10⁻¹⁴, 3.41151892×10⁻¹³, and 3.41151892×10⁻¹².

## 27. Stabilizing potential

$$V(\sigma) = \frac{\lambda}{4}\left( \sigma^{2} - {\bar{M}}_{P}^{2} \right)^{2}$$

**Meaning** A dimensionless scale-breaking potential for the opening field. λ is a dimensionless coefficient belonging to bulk LAW, not a SOURCE impulse.\
**Scope** A restricted model fixing a canonical homogeneous compensator, double-well stabilization, and Planck anchoring.\
**Grade** ONE-COEFFICIENT SUFFICIENCY, not universal uniqueness\
**Basis** 10.5281/zenodo.22182366

## 28. LAW–SOURCE ownership separation

$$\lambda \in LAW,\quad\eta \in SOURCE$$

**Meaning** λ forms the solution space of realizable universes, while η begins one history within it. Minimum input does not mean “zero coefficients in the laws.”\
**Scope** Ownership ledger for the restricted completion class.\
**Grade** CENTRAL INTERPRETIVE CLOSURE\
**Basis** 10.5281/zenodo.22182131; 10.5281/zenodo.22182366

## 29. Undetermined degrees of freedom in n-channel branching

$$b_{i} \geq 0,\quad\sum_{i = 1}^{n}b_{i} = 1\quad \Rightarrow \quad\dim\left( \text{branching simplex} \right) = n - 1$$

**Meaning** One total transfer rate does not determine how energy is divided among n independent channels. Branching fractions must be supplied by LAW’s interaction structure, not hidden and substituted within SOURCE.\
**Scope** n mutually independent final channels and normalized branching fractions.\
**Grade** EXACT NON-IDENTIFIABILITY\
**Basis** 10.5281/zenodo.22182366
