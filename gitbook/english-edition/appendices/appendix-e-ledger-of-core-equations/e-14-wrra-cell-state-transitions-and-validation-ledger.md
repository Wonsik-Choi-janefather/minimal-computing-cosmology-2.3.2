# E-14 WRRA-Cell State Transitions and Validation Ledger

## 102. Present cellular state and update

$$
Xₖ=(xₖ,hₖ,nₖ,sₖ,bₖ,wₖ,dₖ), Xₖ₊₁=F(Xₖ,Rₖ,Bₖ,Uₖ)
$$

Meaning Combines fast activity, slow residue, resources, and damage as a candidate sufficient state of the present.\
Grade MODEL STATE DEFINITION\
Basis 10.5281/zenodo.22304462

## 103. Closed dimensionless matter ledger

$$
Mₖ=nₖ+sₖ+bₖ+wₖ, Mₖ₊₁=Mₖ
$$

Meaning Conservation in the token ledger defined by the toy code. It is not identical to conservation of mass, ATP, or free energy in a real cell.\
Grade EXACT UNDER IMPLEMENTED CLOSED TOY BOUNDARY\
Basis 10.5281/zenodo.22304462

## 104. Linear Markov baseline M0

$$
xₜ₊₁=A[xₜ,uₜ,qₜ]+b+εₜ
$$

Meaning A linear baseline using only the currently observed state and input, without residue.\
Grade COMPARATOR DEFINITION\
Basis 10.5281/zenodo.22304462

## 105. Nonlinear Markov baseline M1

$$
xₜ₊₁=Aφ₂([xₜ,uₜ,qₜ])+b+εₜ
$$

Meaning Tests whether present nonlinearity absorbs an apparent residue effect.\
Grade COMPARATOR DEFINITION\
Basis 10.5281/zenodo.22304462

## 106. Residue-augmented model M2

$$
hₜ₊₁=λhₜ+(1−λ)xₜ₊₁, xₜ₊₁=A[xₜ,uₜ,qₜ,hₜ]+b+εₜ
$$

Meaning Recursively carries a finite-dimensional slow present state.\
Grade MODEL DEFINITION; whether it constitutes a distinct biological theory is OPEN\
Basis 10.5281/zenodo.22304462

## 107. Library-size normalization and direct-target exclusion

$$
eᵢg=log[1+10⁴cᵢg/Lᵢ], xᵢP=σ{|G_P∖{tᵢ}|⁻¹Σg∈G_P∖{tᵢ} zᵢg}
$$

Meaning Normalizes by the full library and prevents a direct target from dominating its own program score.\
Grade LEAKAGE-CONTROLLED TRANSFORM\
Basis 10.5281/zenodo.22304462

## 108. Estimation of static program relations

$$
Ŵd←s=−|T_s|⁻¹Σg∈T_s Sdg
$$

Meaning Estimates destination response from the mean static signature of source-program targets. CRISPRi sign reversal is an operational convention, not a theorem of structural causality.\
Grade STATIC PARTIAL ESTIMATOR\
Basis 10.5281/zenodo.22304462

## 109. K562 partial-audit judgment

$$
q<0.05: 0/12, sign agreement=4/12, r=0.365, ρ=0.462
$$

Meaning The tested GROWTH/REPAIR source submatrix did not support the frozen toy W.\
Grade PARTIAL NON-CONFIRMATION; GLOBAL VERDICT INSUFFICIENT\
Basis 10.5281/zenodo.22304462

## 110. Discriminating prediction for residue

$$
matched xₜ,uₜ + different history ⇒ different rechallenge; RMSEholdout(M2)<min[RMSEholdout(M0),RMSEholdout(M1)]
$$

Meaning With the currently observed state matched, a history-dependent difference must remain, and a measurable residue candidate must predict new data better than a strong Markov baseline.\
Grade PROPOSED FALSIFICATION TEST / OPEN\
Basis 10.5281/zenodo.22304462
