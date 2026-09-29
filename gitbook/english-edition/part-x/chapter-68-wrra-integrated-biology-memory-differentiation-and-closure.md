# Chapter 68 WRRA Integrated Biology: Memory, Differentiation, and Closure

Conclusion of this chapter: The lineage from the WRRA-Cell audit in DOI 10.5281/zenodo.22304462 through Integrated Biology 3.0 in DOI 10.5281/zenodo.22448911 is connected to the two-axis completeness audit of Integrated Biology 4.1 in DOI 10.5281/zenodo.22459333. The first axis runs from DNA through RNA and protein execution, molecular allocation, minimal cells, and the first-life boundary; the second runs from epigenetic memory through differentiation, lineage, aging, cancer, spatial niches, and causal editing. The core of version 4.1 is not a declaration that every closure succeeded, but the assignment of reproducible judgments to the three remaining tests. PURE nonribosomal mass regeneration failed at 0.08; Syn3A allocation passed only within the computational model; and synthetic protocells persisted for at least three generations under external support, but autonomous closure was not established.

## 68.1 From Cosmological Intuition to a Biological Testing Contract

WRRA-Cell does not ask whether a cell rereads a list of past events each time. It asks whether, when an effect of the past is required to calculate the next present, that effect is implemented in present molecular, regulatory, metabolic, or boundary states or in a measurable sufficient statistic. This closure principle does not deny memory; it requires memory to be physically present now.

Xₖ=(xₖ,hₖ,nₖ,sₖ,bₖ,wₖ,dₖ), Xₖ₊₁=F(Xₖ,Rₖ,Bₖ,Uₖ)

x is fast program activity; h is slow present residue; n, s, b, and w are dimensionless ledgers for nutrients, substrates, biomass, and waste; and d is damage. The six programs GROWTH, STRESS, REPAIR, AUTOPHAGY, QUIESCENCE, and DEATH and their marker-gene sets form a preregistered hypothesis map, not a standard complete decomposition of actual cells. RNA expression is not identical to protein activity, metabolic flux, or cell fate.

## 68.2 Version 0.1: An Executable Toy Cell and Internal Tests

Version 0.1 executed fast state, slow residue, and the nutrient, substrate, biomass, waste, and damage ledgers across 420 discrete present updates. The maximum error in the closed dimensionless ledger M = n+s+b+w was 2.49 × 10⁻¹⁴, and restart error after copying the complete present was zero. After REPAIR ablation, the death peak increased 16.38-fold, from 0.050924 to 0.834114; in a rechallenge matched on fast state and resources, adaptive residue reduced the death peak by 15.13%.

M\_k = n\_k+s\_k+b\_k+w\_k, M\_{k+1} = M\_k \[closed dimensionless toy boundary]

These numbers are unit tests showing that the designed wiring, restart, and ledger operate as coded. REPAIR-ablation and adaptive-residue effects were built into the coupling structure and are not newly discovered biological predictions. The grade of version 0.1 is STRUCTURAL PASS; biological validation has not yet occurred.

## 68.3 Versions 0.2–0.3.1: Competing Models and a Fair Residue Test

A recurrent state merely labeled residue overlaps mathematically with existing state-space, adaptation, and memory models. To distinguish it, linear Markov M0, nonlinear Markov M1, and M2 with present residue h compete on the same holdout.

M0: xₜ₊₁=A\[xₜ,uₜ,qₜ]+b+εₜ

M1: xₜ₊₁=Aφ₂(\[xₜ,uₜ,qₜ])+b+εₜ

M2: hₜ₊₁=λhₜ+(1−λ)xₜ₊₁, xₜ₊₁=A\[xₜ,uₜ,qₜ,hₜ]+b+εₜ

Version 0.3 separates claims permitted by static data from those requiring time-series data. Static Perturb-seq can reveal mean program responses and shifts in state distributions, but cannot identify the recovery trajectory of the same cell, whether residue from a first stimulus changes a second response, residue decay rates, or long-horizon rollout. Unless there is temporal order, at least three time points per trajectory, independent repeats per protocol, perturbation-level train/test separation, and time-dependent boundary input, the temporal claim gate remains closed.

Version 0.3.1 introduced full-library normalization, treatment of near-zero variance, exclusion of directly targeted genes, dynamic boundary inputs, identical observed covariates for M0/M1/M2, validation-only tuning, and independent trajectory-level bootstrap. The earlier procedure calling test error BIC was also discarded. This is a fairness contract preventing comparison in which the residue model wins by receiving more information.

## 68.4 Conditional Long-Horizon Predictive Gain Recovered in Synthetic Data

Conditional rollout RMSE in the revised residue-positive generating system was 0.018651 for M0, 0.020672 for M1, and 0.015505 for M2. M2 was 16.87% lower than M0 (95% paired-bootstrap CI 15.98%–17.62%) and 25.00% lower than M1 (21.71%–27.31%). In the memory-negative generating system, nonlinear Markov M1 was best at 0.013644, while M2 was 0.018923, 38.70% higher than M1. All four preregistered conditions passed.

The exact meaning of this result is that the selector recovered M2 in a world designed to generate residue and could select a strong Markov baseline in a memory-free world. This is synthetic mechanism recovery by the validation pipeline, not evidence that actual cells possess WRRA residue.

## 68.5 Version 0.4: Audit of Real Static K562 Perturb-seq

Version 0.4 applied the 34-marker map of version 0.3.1 without modification to the Harmonizome-standardized gene-by-perturbation signature matrix derived from the K562 essential-gene CRISPRi Perturb-seq study by Replogle et al. The provider's matrix contains 8,055 genes and 2,012 perturbation columns, from which 1,907 unique targets were interpreted. The input SHA-256 is 1f9e32ff09b5516807893b1515e96fe23f5e1894687b5a390b7603e9a21cb06f.

Only GROWTH and REPAIR among the six source programs had enough independent targets, so only twelve of 36 relations could be estimated. Selecting equal-size random target sets within each source 20,000 times and applying Benjamini–Hochberg correction to twelve p values produced 0/12 relations with q < 0.05. Agreement with toy signs was 4/12 = 33.3% (binomial p = 0.388); Pearson r with toy weights was 0.365 (p = 0.243), and Spearman ρ was 0.462 (p = 0.131), none significant.

The tested submatrix therefore does not support the frozen toy coupling matrix W. This result must not be reread as a success. At the same time, four source programs and every temporal axis were absent, so these data alone cannot reject WRRA as a whole or temporal residue. The frozen assessment of version 0.4 is PARTIAL NON-CONFIRMATION / INSUFFICIENT FOR GLOBAL VERDICT.

## 68.6 Audit of the Physics–Biology Boundary

M = n+s+b+w in version 0.1 conserves dimensionless tokens defined by the code, not physical mass, ATP, free energy, entropy, or the sum of program activities. An actual cell is an open nonequilibrium system that takes in nutrients and oxygen and releases heat and metabolites. Claiming a physical interpretation requires closing unit-bearing boundary fluxes of carbon, nitrogen, ATP, redox equivalents, heat, and effluents separately.

CRISPRi is an intervention, but flipping the sign of a static mean signature does not identify structural causal coefficients among programs. Incomplete knockdown, compensation, growth selection, pleiotropy, cell composition, batch, and preprocessing can all intervene. For the same reason, success or failure of the cellular application does not count as physical proof or falsification of WRRA cosmology.

## 68.7 What Could Make WRRA-Cell a Distinct Theory

If h in M2 remains a simple exponential smoother, WRRA-Cell may be a useful re-expression but is not an independent biological theory. To become a distinct theory, it must present measurable physical candidates for residue, joint predictions of relation weights and resource boundaries, preregistered RESET conditions, and parameter transport across cell lines, perturbations, and batches.

The central identification prediction is this: among cell populations matched sufficiently on observed fast transcript state and present boundary input but with different perturbation histories, rechallenge responses must differ; M2 containing a measurable present-residue candidate must improve holdout performance over strong M0/M1 under the same information and tuning budget; selective ablation of the residue candidate must erase that difference; and the effect must transfer to new cell lines and batches.

## 68.8 Failure Conditions for Version 0.5

If a strong Markov model repeatedly predicts as well as or better than M2, empirical need for the residue layer is abandoned. If history effects remain after matching the present state but cannot be compressed into finite measurable residue, the current finite-state closure is rejected. If the unit-bearing matter and energy ledgers do not balance, the resource interpretation is discarded. If the relation map must be retuned for each dataset and does not transport, the claim of a universal relation law is downgraded.

Before results are inspected, the next experiment must freeze program direction, duplicate handling, minimum target count, and exclusion rules, and secure at least ten independent targets per program for all six source programs where possible, with at least four represented. Static relation tests must be separated from washout–rechallenge temporal-residue tests and include raw or quasi-raw data, non-targeting controls, guide efficacy, batch, and lineage information.

The final grade is “0.1 toy structure STRUCTURAL PASS / 0.3.1 synthetic mechanism recovery and validation pipeline VALIDATED / 0.4 partial K562 audit of frozen W PARTIAL NON-CONFIRMATION / temporal residue in actual cells, physical resource conservation, RESET, and parameter transport OPEN.”

Chapter conclusion WRRA-Cell 0.1–0.4's most important achievement is not a declaration that cells follow WRRA, but the reduction of an upstream intuition into a computational contract capable of failure and preservation of the first result not supported by real data. The universal-logic hypothesis of minimal computation grows stronger only by passing domain-specific falsification and independent prediction, not by hiding this nonconfirmation.

## 68.9 Life Model IV: Epigenetic Memory Is Reconstruction of State, Not Persistence of a Mark

DOI 10.5281/zenodo.22429511 asks how cells with identical or nearly identical DNA construct different identities and reconstruct them after division. Genome G is treated as a relatively stable SOURCE; methylation, histones, chromatin accessibility, three-dimensional genome organization, and transcription-factor binding as execution gates; RNA, protein, metabolism, and signaling as short- or medium-term residue; and function, morphology, and lineage behavior as OBSERVABLES. Here, reconstruction of state through somatic division and germline transgenerational inheritance beyond embryonic reprogramming are separate claims.

Xₜ=(Cₜ,Mₜ,Aₜ,Hₜ,Rₜ,Pₜ,Sₜ,Qₜ), Oₜ=R(G,Xₜ,Eₜ;θ)+εₜ

C, M, A, and H denote three-dimensional chromatin, DNA methylation, accessibility, and histone state; R, P, S, and Q denote RNA, protein, signaling or metabolism, and cellular context. Because one RNA snapshot or one mark does not uniquely identify the same internal state, cell memory must be measured jointly across multiple layers and lineage.

## 68.10 Operational Definition of Memory and the Replication–Dilution–Restoration Operator

Under the strong operational definition, memory is the property that, after an inducing signal is removed, past state adds prediction of future response or functional lineage bias after controlling for genome, later environment, lineage, and present cell state, and that selective intervention on candidate residue changes the result. Mark persistence, age prediction, or cluster separation alone does not establish causal memory.

Mres(τ)=I(Xpast;Yfuture | G,Ufuture,lineage,current state)

Xₖ₊₁=Φrep(Xₖ)+Φread/write(Xₖ,Pₖ)−Λ(Xₖ)+ηₖ, mₖ₊₁=ρₘmₖ+αₘf(mₖ,pₖ)−βₘg(mₖ)+ηₖ

ρ\_m is the retention coefficient for each mark. One-half dilution is not imposed on every mark. Parental histones, DNMT1–UHRF1 restoration of hemimethylated CpG, mitotic bookmarking, and three-dimensional chromatin require distinct allocation and restoration laws. Division is therefore not simple copying of memory, but reconstruction through material allocation and reader–writer circuits.

## 68.11 Sister-Cell Covariance and Multiple Memory Clocks

Cov(Xd1,Xd2)=Cov(E\[Xd1|M],E\[Xd2|M])+E\[Cov(Xd1,Xd2|M)]

In this total-covariance decomposition, the sign of the second term is not fixed. It can be negative under binomial allocation at fixed total molecule count, but zero or positive under independent Poisson generation, a common environment, or active equalization. The sign of sister correlation must therefore be derived from the generative model and measurement design rather than intuition.

Life Model V in DOI 10.5281/zenodo.22440193 extends memory from the half-life of one mark to eigenmodes of coupled layers. It separates generation distance d from elapsed time t and forbids circular inference that reuses for memory validation the same signal used to infer lineage.

Cℓ(d)=Σᵣaℓᵣλᵣᵈ+Bℓ, Zchild=Astate Zparent+ΓX+ξ

Cross-layer memory is retained only if a nondiagonal A\_state predicts next-generation covariance in unseen lineages better than diagonal-layer and no-memory models after a complexity penalty. If one common decay rate is sufficient or off-diagonal transfer fails to transport to new lineages, the coupled-layer hypothesis is downgraded.

## 68.12 Life Model VI: Noncommutative Order in Cell-Fate Manipulation

The distinguishing prediction is that long-term fate can depend on order even when total realized exposure to gate opening G, lineage transcription-factor pulse T, and maintenance-mark writing W is matched. To avoid merely renaming a generic timing effect, the six permutations, simultaneous treatment, single treatments, catalytic-dead controls, nuclear AUC, target occupancy, washout, cell cycle, and survival must be fixed in advance.

xGTW=ΦWΦTΦGx₀, \[Li,Lj]=LiLj−LjLi, additive null ⇒ \[Li,Lj]=0

The hypothesis that GTW is superior to other orders is separated from a general order effect. If another order wins, the GTW-optimal hypothesis is rejected while noncommutativity itself may remain. If order coefficients lie within a preregistered equivalence interval after realized AUC and occupancy are matched, or if the difference disappears across multiple divisions after washout, the claim of long-term cell-fate memory is withdrawn.

## 68.13 Life Models VII–IX: Induction, Selection, Reversible Editing, and Extracellular Memory

For aging, clonal hematopoiesis, and cancer recurrence, state induction within a lineage must be separated from selection of an existing clone. Bulk before–after differences do not identify the two mechanisms. Life Model VII's central candidate is that short cellular memory can become long population memory through selective proliferation and lineage transmission; it must beat a genotype-and-current-environment-only baseline on external data.

ppost(y)=Z⁻¹∫KU(y|x)sU(x)ppre(x)dx

Life Model VIII holds genome and present environment fixed and write → erase → rewrites candidate memory state Z, testing whether function, rechallenge response, and lineage persistence return together. A one-way expression change cannot exclude off-target effects, toxicity, selection, or general stress. Life Model IX separates ownership by cell, niche, and their interaction through a 2×2 crossover of young versus aged, or untreated versus stimulated, cells and niches.

Z₀→write Z₁→erase Z₀′→rewrite Z₁′, ΔY=ΔYcell+ΔYniche+ΔYcell×niche

## 68.14 Life Model X: Joint Closure from Information to a Living Lineage

The integrative paper retains the previous conclusion that DNA alone does not execute life. Minimal life requires boundary B, replicable source S, decoding relation R, catalytic polymers P, energy and material flow E, and whole-cycle closure C to close together sufficiently to execute again in the next generation. To avoid hiding work performed by the environment, autonomous closure fraction Λ\_auto = N\_internal/N\_required is recorded separately.

Lmin={B,S,R,P,E,C}, 0≤Λauto≤1, I(Xparent;Xoffspring)>0, Rlife=2Kfᴸ>1

This condition does not reconstruct the molecule, location, or path that was historically first. A molecule copied once or a vesicle divided once is not automatically life. The minimum unit of assessment is whether memory, execution, repair, boundary reproduction, and selection create a functional lineage across at least several generations.

## 68.15 Integrated Evidence Ladder and Falsification Contract

What is presently closed under stated assumptions consists of the coding lower bound, finite-allocation equations, total-covariance identity, and executable experimental designs. Minimal-cell toy calculations and the C. elegans circuit are internal computational passes, while the K562 audit is a partial nonconfirmation. General epigenetic and contextual dependence is supported by the literature, but WRRA-specific multilayer transfer matrices, GTW order superiority, induced-state/selection mixtures, reversible rescue, niche interactions, and repeated-generation closure of Λ\_auto remain OPEN.

The common rejection rule gives priority to simple baselines. If a common-clock, independent-layer, additive-AUC, selection-only, independent-cell, or noncausal-mark model predicts the holdout equally well or better under the same information and complexity budget, the WRRA extension is reduced. In clinical or genetic-engineering applications, a fail-closed policy forbids release if any one of Function ∧ Identity ∧ Genome stability ∧ No tumorigenicity ∧ Controllability fails.

## 68.16 Position through Integrated Biology 2.1

What the two new papers strengthen is not the declaration that “cells obey WRRA laws,” but an audit structure separating DNA information from material executors, present state from effects of the past, individuals from lineages, cells from niches, and one-time output from intergenerational closure. This broadens the possibility that minimal computation is a general methodology for analyzing complex systems, but is not independent physical evidence for cosmology. The biological theory's grade rises only if distinguishing predictions are reproduced in independent lineage data and intervention experiments.

## 68.17 The Four-Track Validation Contract of Integrated Biology 3.0

DOI 10.5281/zenodo.22448911 does not combine four tracks into one evidence grade. Tracks 1 and 2 independently recalculate downloadable public data; Track 3 is a structural simulation within declared equations; and Track 4 consists of synthetic predictions and a wet-lab preregistration not yet run. A fail-closed principle prevents synthetic trajectories from being labeled measurements and reported results of original authors from being labeled the present study's own recalculations.

The extended state is X(t) = (g,a,q,m,r,p,e,b,w), separating genome, accessibility, regulatory-factor occupancy, slow epigenetic residue, RNA, protein and phenotype, resources, boundary, and cell–niche relations. This is not a standard complete decomposition of biological entities, but an audit coordinate for tracking which layers were observed and perturbed.

## 68.18 Track 1: Cross-Animal Holdout of DNA Methylation and Protein State

In the raw EPI-Clone GEO matrix, cells from LARRY mice 3 and 4 were matched to antibody-derived-tag records, producing 8,850 cells, 663 assay columns, and twenty shared protein markers. In cross-holdouts that selected CpGs in one animal and tested only in the other, the mean balanced accuracy was 0.487 for 120 state-associated CpGs and 0.502 for all eligible CpGs. It was 0.225 for state-excluded CpGs, while the six-state majority baseline was 0.167.

This result supports a reproducible association across animals between DNA methylation and independently measured protein state. It did not directly test WRRA-specific heritable clonal residue, however, because the downloaded raw data lacked a cell-level LARRY truth table and the publication's refined cell-type and pseudotime information. The six states were also unsupervised protein clusters, not prospectively defined biological labels. The assessment is CROSS-LAYER STATE SUPPORT / CLONAL MEMORY OPEN.

## 68.19 Track 2: Spatial Tumor Plasticity and Selective Niche Information

Of 678,067 rows in the KPSpatial-derived table, 673,263 complete observations were averaged into 150 sample×tumor groups across 39 samples to reduce spatial pseudoreplication. Block permutation within samples 5,000 times and BH correction over eleven neighborhood modules left seven modules passing FDR < 0.05. In sample-group holdout, S1 using six epithelial programs achieved mean R² = 0.201 and MAE = 0.0549, improving on the global-mean baseline R² = −0.130 and MAE = 0.0648.

Adding every stromal and immune module in S2 worsened performance to R² = −0.023 and MAE = 0.0605. The strong claim “adding more relation layers is always better” is therefore unsupported by this audit. Correlations in observational data cannot distinguish niche → state causation, tumor-state → niche reconstruction, and common causes; a cell×niche crossover intervention remains the decisive test. The assessment is SELECTIVE RELATIONAL SUPPORT / NICHE CAUSALITY OPEN.

## 68.20 Tracks 3–4: Structural Predictions and Wet-Lab Preregistration

When the six G/T/W permutations, each with identical six-hour treatments and two-hour intervals, were calculated in the declared gate–occupancy–mark model, G → T → W gave a final mark of 0.5021, while second-ranked T → G → W gave 0.1630. Across 1,000 synthetic parameter sets independently varying nine kinetic scales and half-life multipliers by factors of 0.7–1.3, G → T → W ranked first in every case. This is internal robustness of order dependence in those equations, not a biological fact measured in cells.

In a synthetic write–erase–rewrite system, the mark fell to 0.0008 after erasure and returned to 0.5090 after rewrite, giving a model rescue fraction of 1.008. An actual pass requires the lower bound of the 95% confidence interval for functional R\_rescue to exceed 0.50 across independent biological replicates and jointly satisfy W > WE, WER > WE, restoration of the target mark, balance of survival and proliferation, and off-target limits. If the effect does not persist across at least three divisions after editor removal, it is classified as transient execution rather than heritable memory.

## 68.21 Position through Integrated Biology 3.0

Version 3.0 raises only two evidence grades. The association between DNA and protein differentiation state is supported by cross-animal public-data reanalysis, and selected epithelial spatial programs improve prediction of tumor plasticity in sample holdouts. Indiscriminate addition of every niche layer failed, while WRRA-specific clonal residue, actual biological superiority of GTW, causal rescue through write–erase–rewrite, and multigenerational autonomous closure remain OPEN pending independent experiments.

Chapter conclusion WRRA Integrated Biology 3.0 does not prove life with one equation. It separates which layer interprets present state, which term predicts the future of a new sample or lineage, which result is only a structural simulation, and what awaits an actual intervention. Preserving these distinctions allows minimal computation to become a candidate general methodology for comparing information ownership and failure conditions in complex systems rather than rhetoric importing biology as evidence for cosmology.

## 68.22 Integrated Biology 4.1: The Exact Meaning of Two-Axis Completeness

In DOI 10.5281/zenodo.22459333, “completeness” does not mean that every mechanism of life passed. It is completeness of research structure: operational variables, thresholds, current judgments, and falsification conditions have been assigned to each requested question along the two axes DNA → first life and epigenetic memory → cell fate. The evidence order remains direct measurement; original-author report; reanalysis or explicit inference; mechanistic simulation; and unrun preregistration.

## 68.23 PURE: The Mass Ledger of Generation-by-Generation Self-Regeneration

A 2026 PURE reconstruction study synthesized all 36 nonribosomal proteins within one PURE reaction and reconstructed a functional second-generation translation system. Starting from 350 μg of nonribosomal proteins, however, only 28 μg was recovered after purification and concentration, so the measured mass-regeneration ratio is R\_mass,nr = 28/350 = 0.08. This falls below the threshold R\_mass,nr ≥ 1 required for nondegeneration under repeated equivalent transfer.

Assuming constant efficiency 0.08 gives M\_nr(n)/M\_nr(0) = (0.08)ⁿ and a ratio of 5.12 × 10⁻⁴ after three transfers. This is a mass-balance extrapolation, not an observed three-generation functional trajectory. Nonribosomal synthesis and one-time functional reconstruction are PASS; nonribosomal mass replacement in this implementation is FAIL. Because ribosomes, rRNA, tRNA, DNA replication, energy, and boundary were not regenerated jointly within one lineage, full PURE autonomous closure is not extrapolated as failure but remains OPEN.

## 68.24 Syn3A: Molecular Allocation from One Mother to Two Daughters

To avoid confusing survival-threshold fraction φ with allocation error, define the allocation error for molecular species x as D\_x = |p\_x−v|. Here p\_x = N\_x,1/(N\_x,1+N\_x,2) is the molecule-count fraction between two daughters and v = V₁/(V₁+V₂) the volume fraction. D\_x = 0 is volume-proportional allocation. For equal-sized daughters and unbiased binomial allocation, RMS(D\_x) = 1/(2√N\_x) and E\[D\_x] ≈ 1/√(2πN\_x).

Across fifty complete cell cycles in the Syn3A four-dimensional whole-cell model, the mean mother cell at 105 min contained 881 ribosomes, 176 RNA polymerases, and 192 degradosomes. Reported daughter distributions of ribosomes, degradosomes, PtsG, and GapDH were near-binomial within the model and had no significant directional bias. Expected RMS allocation errors from mother-cell counts are 1.68% for ribosomes and 3.61% for degradosomes. These are analytical expectations under the binomial null, not measurements from individual daughter cells.

The Syn3A assessment is therefore COMPUTATIONAL PASS / DIRECT EXPERIMENT OPEN. Actual closure requires time-resolved tracking of one mother and two daughters, cell-specific volume correction, molecule-species counts, preregistered acceptance bands for D\_x, and simultaneous measurement of whether every essential pool crosses threshold φ. If directional bias in a particular molecular species is reproduced after controlling geometry, cell cycle, DNA exclusion, and detection efficiency, the unbiased-allocation hypothesis is rejected.

## 68.25 Synthetic Protocells: Separating Three-Generation Persistence from Autonomy

A 2026 synthetic-cell preprint reported a five-cycle experiment combining genome replication, feeder-liposome growth, division, and selection using a defined PURE translation system and a 90-kbp genome split among seven plasmids. The narrow threshold G\_persist ≥ 3 therefore passes on this evidence. Operation for approximately five to ten generations in the official description is a supplementary statement, not an independently recalculated value.

Approximately 30% of fifth-generation daughter cells retained all seven plasmids. Under assumptions of ideal binary fission and similar survival and sampling, a proxy for geometric growth of complete-genome descendants is R\_genome,eff = \[2⁵×0.30]^(1/5) ≈ 1.57. This is a conditional inference calculated from the reported endpoint, not a measured value of the paper's authors, and is not R\_life. The actual system depends on feeder vesicles, membrane capture, preformed ribosomes, and external molecular support and does not regenerate ribosomes. The assessment is therefore “persistence for at least three generations passed; autonomous closure not established.”

## 68.26 Final Closure Map of the Two Axes

Closed on Axis I are DNA and protein execution, one-time functional reconstruction of PURE, computational near-binomial allocation in Syn3A, and at least three generations of externally supported protocell persistence. Not closed are sustained replacement with R\_mass,nr ≥ 1, simultaneous molecular measurements of an actual mother and two daughters, and an R\_life > 1 lineage jointly updating genome, translation, energy, and boundary without external material replacement. On Axis II, cross-animal DNA–protein state associations and selective spatial programs receive limited support. WRRA-specific clonal residue and functional rescue by write–erase–rewrite across multiple divisions remain OPEN.

Chapter conclusion Integrated Biology 4.1 does not conclude that “DNA alone created life.” By separating lineage persistence under external support from internal resource regeneration, it narrows the first-life boundary. The decisive remaining Axis I experiment asks whether one compartmentalized lineage updates genome, translation, energy, and boundary without material replacement and maintains R\_life > 1 for at least three generations. Axis II still requires reversible memory editing along the same tracked lineage that jointly shows functional rescue and persistence for at least three divisions. This biological completeness is completeness of an audit contract, not independent physical proof of WRRA cosmology.

## **68.27 WRRA-Motor H2: From Explaining Life to Designing Molecular Machinery**

DOI 10.5281/zenodo.22660185 asks, “What minimum functional architecture is required for a protein that repeatedly advances along a polar track while consuming chemical free energy?” Rather than copying the appearance of natural kinesin, the research first establishes a strict walking contract through WRRA Core, exhaustively surveys possible functional architectures, compares them post hoc with natural motors, and finally connects a protein and DNA renderer. This order tracks what is DERIVED, what is INHERITED, and what was newly DESIGNED.

## **68.28 The WRRA Domain Profile and Strict Contract for the Walking Problem**

**Table 68-1. Information Ownership in WRRA-Motor**

| **WRRA Owner**     | **Implementation in a Molecular Motor**                                            |
| ------------------ | ---------------------------------------------------------------------------------- |
| SOURCE             | External chemical free energy, typically ATP                                       |
| RELATION/LAW       | Binding and unbinding, thermal diffusion, local detailed balance, polar track      |
| STATE/RESIDUE      | Binding of the two heads, nucleotide occupancy, elastic and structural deformation |
| BOUNDARY           | Cytoplasm, temperature, thermal noise, load, microtubule lattice                   |
| COMMON CARRIER     | Protein conformational change converting energy state into mechanical displacement |
| UPDATE             | Present-state transition coupled to ATP input                                      |
| RENDERER/PHENOTYPE | Folding, binding geometry, and gate → net plus-end displacement                    |
| OBSERVABLE         | Velocity, detachment rate, run length, ATP cost, and stall force                   |

The strict contract V\_strict(M) = 1 simultaneously requires positive expected displacement per cycle; at least one contact remaining on the track during contact exchange; finite energy and complexity; and determination of the next binding or unbinding order from present state alone. A one-contact Brownian ratchet permitting biased rebinding after complete detachment is separated into the weaker V\_relaxed. Two-contact minimality is therefore a theorem under the declared strict contract, not an unconditional proposition about all of nature.

## **68.29 Exhaustive Survey of 64 Functional Architectures and a Conditional Minimality Theorem**

All 64 architectures combining one to four contacts with four binary conditions—energy drive, polar coupling, present record, and coordination—were evaluated. A single point contact cannot move from i to i+1 without an interval of zero contact, whereas two contacts allow one to move while the other remains anchored.

S₀(i,i+1) → S₁(∅,i+1) → S₂(i+1,i+2) → S₀(i+1,i+2)

M\*=(2 contacts, drive, polarity, present record, coordination)

Among two-, three-, and four-contact architectures passing the strict contract, M\* is the unique Pareto minimum of cost vector C(M) = (number of contacts, number of controls, number of drives). This structural conclusion was obtained by independently enumerating the functional contract for walking, not by entering known kinesin into an equation and recovering it. In a post hoc comparison, two motor heads, ATP, microtubule polarity, nucleotide occupancy and strain, and neck-linker gating corresponded to the five requirements.

## **68.30 The Physical Ledger of Directionality, Load, and Redundancy**

Under local detailed balance, the forward-to-reverse ratio is determined by cycle affinity A. ATP itself has no direction; mean displacement arises only when chemical input Δμ couples to a polar track and asymmetric structure.

k₊/k₋=exp(A), A=(Δμ−Wload)/(kBT)

p₊=1/\[1+exp(−A)], ⟨Δx⟩=d·tanh(A/2), Fmax,ideal=Δμ/d

If the probability of losing each contact in the exchange window is simplified to q, N-cycle survival for an n-contact architecture is P\_survive(N;n,q) = (1−qⁿ)ᴺ. Two contacts are minimal at low risk, but as q increases, the existence cost of a third or fourth contact greatly reduces the risk of complete detachment. This result again shows at molecular scale that minimality and redundancy are not opposites, but costs exchanged according to boundary conditions.

## **68.31 Protein Renderer 0.3 and the H2 Candidate**

Functional conditions do not immediately yield a unique amino-acid sequence. A hybrid renderer therefore retains the validated human KIF5B 1–353 aa segment as the motor and track-binding core and generates only a 32-aa coiled-coil-like gate targeting dimerization and present-state coupling. Using fixed seed 260908, 512 gates were generated and filtered, the top five preserved, and top candidate H2-b2f820d18e obtained.

R₀.₃: F → Thybrid → {gᵢ}ᵢ₌₁⁵¹² → filter → H2\* → DNA(H2\*)

KIF5B(1–353) ∥ VQNIEQKIANLKEEGAAALQQVEQKIQNLKAE

**Table 68-2. H2 Design Results and Ownership Ledger**

| **Output**           | **Quantitative Result**                     | **Ownership and Grade** |
| -------------------- | ------------------------------------------- | ----------------------- |
| Motor / binding core | KIF5B 1–353 aa; 91.69% of the whole         | INHERITED               |
| WRRA gate            | Residues 354–385; 32 aa; 8.31% of the whole | DESIGNED                |
| H2 protein           | 385-aa parallel-homodimer hypothesis        | HYBRID / PREDICTED      |
| DNA CDS              | 1,158 nt including stop; GC 57.69%          | PREDICTED               |
| Gate search          | 512 passed; top five preserved              | REPRODUCIBLE SEARCH     |
| Fully de novo N1     | No sequence output                          | FAIL-CLOSED             |

The H2 gate satisfied every declared hydrophobic a,d position and oppositely charged e,g position in the heptad and obtained charge density 0.2813, maximum nine-residue hydrophobicity 0.5556, normalized composition entropy 0.7014, and constraint-satisfaction score 5.0806. These values are pass records for sequence grammar, not probabilities of function. The important achievement lies not in exaggerating numbers into physical validation, but in closing function contract, topology, sequence, DNA, and controls into one lineage.

## **68.32 A Conditional Theorem of Present-State Machinery and Cumulative Displacement**

The past required for walking remains not in a separate history file but in present binding states B\_A and B\_B, neck-linker directions and tensions N\_A and N\_B, nucleotide state E, and gate state G. X\_t = (B\_A,B\_B,N\_A,N\_B,E,G), updated as X\_{t+1} = T(X\_t,ATP).

S₀(x) → S₁(x) → S₂(x+8 nm) → S₀(x+8 nm)

xₙ=x₀+8n nm

Under a transition contract in which every normal cycle moves S₀(x) to S₀(x+8 nm) and backward transitions are forbidden, induction gives cumulative displacement 8n nm after n cycles. This is a formal result that directional accumulation emerges if the WRRA state-transition rule is implemented. Whether the H2 sequence actually implements that rule belongs to separate renderer, structural, dynamical, and experimental layers.

## **68.33 A New Boundary of Design Science: Inheritance, Design, Prediction, and Openness**

The originality of this research does not lie in creating every residue anew. The already functional 353-aa core is frozen as INHERITED, while only the 32 aa responsible for the present-state coordination function required by WRRA is narrowed as DESIGNED. Controls are a gateless B0, H1 with an existing GCN4 appendage, a length-matched generic coiled-coil C1, and a composition-preserved scrambled gate C2. A WRRA-specific contribution can be assessed if H2 differs from these controls in repeated walking, tension transfer, and detachment rate.

With no renderer capable of validating a fully de novo ATPase and microtubule-binding surface, no N1 sequence was generated. This fail-closed judgment is not concealment of weakness but a methodological achievement distinguishing strings that can be generated from designs that can be scientifically owned. WRRA's minimal computation minimizes not only unnecessary structure, but unsupported proliferation of claims.

## **68.34 What WRRA-Motor Adds to Minimal Computation Cosmology**

First, WRRA advances beyond post hoc interpretation of known phenomena into a design framework that generates candidate architectures from an explicit contract. Second, the fixed-present principle becomes not an abstract philosophy of time but a concrete design condition: molecular machinery determines the next order from present material states of binding, energy, and tension. Third, the common carrier is materialized as protein conformational change converting ATP energy state into spatial displacement. Fourth, the tradeoff between minimality and redundancy is recovered, following cosmology, AI, and life, as the direct structural problem of contact number. Fifth, a ledger preserving information ownership is built all the way from function to DNA.

**Chapter conclusion WRRA-Motor H2 in DOI 10.5281/zenodo.22660185 presents a more structural achievement than the short declaration “a new protein was created.” It connects a strict walking contract, exhaustive survey of 64 architectures, a conditional minimality theorem, thermodynamic directionality, a hybrid renderer, a 385-aa candidate, a 1,158-nt CDS, controls, and fail-closed boundaries into one reproducible design lineage. This is the first constructive case showing that the principle of minimal computation can move from explanation of the universe into design of living matter.**

Part XI WRRA Extended to Social Complex Systems: Economics and Institutional Memory
