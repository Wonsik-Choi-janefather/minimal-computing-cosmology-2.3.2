# E-11 External Application to Living Systems

## 63. WRRA execution object and provenance ledger

$$
M_WRRA=(S,L,X₀,R,O,Π)
$$

Meaning Separates supply, law, initial state, representation, observation, and provenance.\
Grade STRUCTURAL SCHEMA\
Basis 10.5281/zenodo.22289266

## 64. Minimal life instance

$$
LIFE=(Genome,Proteome,Metabolism,Membrane,Geometry,Environment,Division Predicate)
$$

Meaning The execution graph of the whole cell, not DNA alone.\
Grade STRUCTURAL DEFINITION\
Basis 10.5281/zenodo.22289266

## 65. Living-state operator and observation

$$
dx/dt=F(x;θ,e), y(t)=O[x(t)]
$$

Meaning Updates the state under an environment and parameters, then extracts observables.\
Grade GENERAL MODEL FORM\
Basis 10.5281/zenodo.22289266

## 66. Five-gate cell cycle

$$
Tcell=inf{t:GD∧GP∧GM∧GE∧GF}
$$

Meaning Replication, protein, membrane, energy, and spatial division must all close.\
Grade FAIL-CLOSED STOPPING RULE\
Basis 10.5281/zenodo.22289266

## 67. Five-component autocatalytic growth

$$
dx/dt=Ax, Av\*=λ\*v\*
$$

Meaning A positive dominant mode defines balanced growth.\
Grade EXACT IN THE LINEAR TOY MODEL\
Basis 10.5281/zenodo.22289266

## 68. Lower catalytic bound for syn3A DNA replication

$$
Trep,lower=543,380/(2×600×60)=7.546944 min
$$

Meaning An ideal lower bound omitting binding, assembly, crowding, stalling, and repair.\
Grade DERIVED LOWER BOUND\
Basis 10.5281/zenodo.22289266

## 69. Membrane-area threshold for division volume

$$
rdiv=2¹ᐟ³r₀, Adiv=2²ᐟ³A₀=797,914.8 nm²
$$

Meaning Under a spherical approximation with r₀=200 nm, membrane area must increase by 58.7401%.\
Grade EXACT GEOMETRY UNDER ASSUMPTIONS\
Basis 10.5281/zenodo.22289266

## 70. Operational condition for living closure

$$
Living closure⇔bounded openness∧renderer self-reconstruction∧intergenerational executability
$$

Meaning Requires both self-construction amid environmental exchange and intergenerational executability.\
Grade WRRA OPERATIONAL DEFINITION\
Basis 10.5281/zenodo.22289266

## 72. Operational objective function of the universal minimal-computation grammar

$$
C\*=argmin_C[Iindependent+Mstored+Uupdate+Rrepair], subject to Closure=1, Fidelity≥F\*, Robustness≥R\*
$$

Meaning A cross-domain comparative hypothesis that reduces the costs of independent input, storage, updating, and recovery while preserving closure, accuracy, and robustness.\
Grade UNIVERSAL-GRAMMAR HYPOTHESIS / OPEN\
Basis 10.5281/zenodo.22289266

## 73. Gene-execution map and no-bootstrap boundary

$$
Y=Φ(D,E,X₀,t), E=empty⇒Yprotein(t)=0
$$

Meaning Separates the DNA specification from the material executor. Grade STRUCTURAL NO-BOOTSTRAP RESULT IN ORDINARY DNA-DIRECTED TRANSLATION. Basis 10.5281/zenodo.22290829

## 73. Lower bound on peptide coding length

$$
Lcoding,min(n)=3n+3 nt
$$

Meaning The pure coding floor for n residues and one stop codon. Grade EXACT UNDER ORDINARY TRIPLET CODING. Basis 10.5281/zenodo.22290829

## 74. Length–processivity model

$$
Pfull(n|δ)=(1-δ)ⁿ, n₅₀=ln(0.5)/ln(1-δ)
$$

Meaning The probability of a full-length peptide under independent dropout per codon. Grade DERIVED / MODEL-CONDITIONAL. Basis 10.5281/zenodo.22290829

## 75. Regeneration margin of nonribosomal PURE components

$$
Rnonribosomal=0.08<1, margin=0.08-1=-0.92
$$

Meaning Functional reconstruction was achieved, but sustained self-replacement did not close. Grade EXPERIMENTAL INPUT / SUSTAINED REPLACEMENT FAIL. Basis 10.5281/zenodo.22290829

## 76. Unbiased molecular partition law

$$
X~Binomial(N,1/2), E[X]=N/2, Var(X)=N/4, CV=1/√N
$$

Meaning Even under symmetric geometry, low-copy pools have large relative noise. Grade EXACT. Basis 10.5281/zenodo.22291113

## 77. Sister-dependent offspring distribution and Rlife

$$
P₁=2(q-P₂), P₀=1-2q+P₂, Rlife=P₁+2P₂=2q
$$

Meaning A 0–1–2 offspring law preserving anticorrelated partitioning between two daughter cells. Grade EXACT UNDER DECLARED PARTITION MODEL. Basis 10.5281/zenodo.22291113

## 78. Lineage-extinction branching process

$$
f(s)=P₀+P₁s+P₂s², ζ=min{s∈[0,1]:f(s)=s}
$$

Meaning Determines the ultimate extinction probability under an assumption of iid restoration of mother cells. Grade EXACT UNDER STATED BRANCHING MODEL. Basis 10.5281/zenodo.22291113

## 79. Boundary-geometry overdispersion and cross-species covariance

$$
Var(Xᵢ)=Nᵢ/4+Nᵢ(Nᵢ-1)σp², Cov(Xᵢ,Xⱼ)=NᵢNⱼσp²
$$

Meaning Noise in a common volume ratio produces rank-one positive covariance across species. Grade EXACT UNDER COMMON-p MODEL. Basis 10.5281/zenodo.22291113

## 80. Independent lineage-closure pass condition

$$
PASS iff paired log-score>baseline ∧ P₀/P₁/P₂ calibrated ∧ covariance signature ∧ holdout survival
$$

Meaning A preregistered pass condition for no-retuning paired-daughter and generational data. Grade WRRA FALSIFICATION CONTRACT / OPEN. Basis 10.5281/zenodo.22291113

## 81. Operational condition for the first living lineage

$$
FIRST LIVING LINEAGE⇔bounded system∧heritable functional variation∧Rlife>1
$$

Meaning Requires intergenerational functional closure beyond growth or one-time division. Grade WRRA OPERATIONAL DEFINITION. Basis 10.5281/zenodo.22291862

## 82. Reproduction number under copying-error closure

$$
q=Kfᴸ, Rlife=2Kfᴸ
$$

Meaning Expected number of functional descendants in a two-daughter baseline where copying across L sites and noncopying closure K are independent. Grade EXACT UNDER DECLARED MODEL. Basis 10.5281/zenodo.22291862

## 83. Critical copying accuracy and information budget

$$
fc=(2K)⁻¹ᐟᴸ, Lmax=ln[1/(2K)]/ln f, K>1/2
$$

Meaning The inherited-length threshold allowed by renderer success and copying accuracy. Grade EXACT UNDER MODEL / NUMERIC SCENARIOS CONDITIONAL. Basis 10.5281/zenodo.22291862

## 84. Population update for first life

$$
πt₊₁(y)∝∫B(y|x)πt(x)dx
$$

Meaning Generates the next-generation distribution from a state-dependent offspring kernel without inserting an external selector. Grade GENERAL POPULATION MODEL / HISTORICAL KERNEL OPEN. Basis 10.5281/zenodo.22291862
