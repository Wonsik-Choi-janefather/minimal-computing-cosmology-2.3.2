# Chapter 65 WRRA Life Model III: Lineage Closure

Conclusion of this chapter: The problem of one cell transmitting its executability to two daughter cells and descendants is closed as a model of finite molecule counts, stochastic allocation, boundary geometry, and a branching process. The mathematical lineage layer is executable, but independent biological prediction remains OPEN because there is no molecular-level paired-daughter holdout.

## 65.1 From One Mother Cell to a Living Lineage

In DOI 10.5281/zenodo.22291113, SOURCE is the genome and inherited molecular inventory; LAW, the rules of reaction, transport, replication, and allocation; STATE, time-resolved molecule counts and spatial arrangement; RENDERER, membrane geometry, division plane, position, and stochastic events; and OBSERVABLES, growth, division, daughter-cell composition, and lineage survival. Copy numbers for the six JCVI-syn3A molecular pools used here mix sources and measurement methods; they are therefore an explicit sensitivity scenario, not one simultaneously measured natural mother cell.

## 65.2 The Exact Allocation Law of a Single Division

If a mother cell has N molecules and each divides independently and without bias, the number X in the first daughter follows a finite binomial distribution.

X\~Binomial(N,1/2), E\[X]=N/2, Var(X)=N/4, CV(X)=1/√N

If the daughter-cell minimum for each pool i is m\_i = ceil(φN\_i/2), the probability that both daughters pass is the sum of binomial probabilities from x = m\_i to N\_i−m\_i. Thus even when volume is exactly symmetric, count noise in essential low-copy-number pools is large.

## 65.3 Sibling-Dependent Offspring Distribution and Reproduction Number

Let q be the probability that one daughter passes all thresholds and P₂ the probability that both do. The exact distribution over zero, one, or two offspring, without treating sisters as independent, is as follows.

P₁=2(q-P₂), P₀=1-2q+P₂, Rlife=P₁+2P₂=2q

Let f(s) = P₀+P₁s+P₂s² be the generating function of the branching process. Under the iid assumption that the same mother-cell distribution is restored each generation, ultimate extinction probability ζ is the smallest solution of f(ζ) = ζ. If R\_life ≤ 1, ζ = 1; if R\_life > 1, ζ = P₀/P₂. For finite generations, ζ\_g = f(ζ\_{g−1}) with ζ₀ = 0.

## 65.4 The Integer Threshold Cliff Owned by HupA

In the declared six-pool scenario, at φ = 6/7 each daughter requires twelve of the 28 copies of HupA and R\_life = 1.133. Increasing φ slightly above 6/7 raises the requirement to thirteen, lowering q and R\_life to 0.978 and making the lineage subcritical. Within this input panel, HupA owns the discontinuous transition.

At φ = 0.80, R\_life = 1.400 and ultimate lineage survival is 86.8%. At φ = 0.8572, R\_life = 0.978, 100-generation survival is 1.18%, and ultimate survival is zero. These are not measured biological constants but a CONDITIONAL SCENARIO showing threshold sensitivity and an integer copy-number cliff.

## 65.5 Active Equalization and the Copy-Number Reliability Frontier

In an audit family where each pool follows feasible equal allocation with probability a and unbiased binomial allocation with probability 1−a, the minimum equalization fraction restoring R\_life = 1 at φ = 0.90 is 26.85%. At φ = 1.00, 76.24% is required. This calculates the strength of renderer control required, not a particular molecular mechanism.

Holding the daughter-cell minimum for HupA at twelve copies, mother-cell counts of 35, 39, and 45 give 95%, 99%, and 99.9% joint passage of both daughters, respectively. Reserves relative to the 28-copy input are +7, +11, and +17. Because translation cost and actual survival thresholds are absent, this is a Pareto frontier between copy cost and inheritance reliability, not an optimum selected by nature.

## 65.6 Boundary-Geometry Covariance and the Paired-Daughter Holdout

If the first daughter's volume fraction p fluctuates with Var(p) = σ\_p², a common geometric RENDERER increases molecule-count variance and creates positive cross-species covariance.

Var(Xᵢ)=Nᵢ/4+Nᵢ(Nᵢ-1)σp², Cov(Xᵢ,Xⱼ)=NᵢNⱼσp² (i≠j)

An approximate rank-one positive common mode proportional to NNᵀ is thus a signal of division-plane and volume noise; species-specific block overdispersion is a candidate for localization or packets; and dispersion index κ < 1 is a candidate for active equalization. The symmetric daughters and 105 min in the public 4D whole-cell model were constrained or calibrated by experimental information and are not reused as independent WRRA holdouts.

The frozen experiment links one mother-cell ID to paired daughters A and B and records the mother molecule count, daughter molecule counts, volume fraction, division plane, subsequent growth or division of each daughter, and the measurement-error model together. An independent PREDICTION PASS requires that the no-refit paired-daughter log score, P₀/P₁/P₂, κ(N) and cross-species covariance, and generational survival curve exceed preregistered criteria.

The final grade is “WRRA-to-life mapping STRUCTURAL PASS / finite binomial allocation and sibling-dependent offspring law EXACT / iid-restoration extinction EXACT UNDER STATED MODEL / HupA cliff EXACT FOR DECLARED PANEL / equalization and reliability frontier CONDITIONAL / common-p covariance EXACT UNDER MODEL / public 4D reconstruction PASS, NOT INDEPENDENT / paired-daughter prediction OPEN.”

Chapter conclusion WRRA Life Model III makes the mathematical layer of lineage closure executable. Integer cliffs at low molecule counts, active equalization, and boundary-geometry covariance supply concrete prediction forms. Biological lineage closure nevertheless remains open until tested on actual molecular-level paired-daughter data.
