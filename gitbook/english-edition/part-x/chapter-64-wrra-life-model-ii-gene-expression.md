# Chapter 64 WRRA Life Model II: Gene Expression

Conclusion of this chapter: DNA can specify a protein but cannot synthesize it by itself. Genetic sequence is SOURCE; the genetic code and reaction rules are LAW; molecular concentrations are STATE; polymerases, ribosomes, tRNAs, aminoacyl-tRNA synthetases, and the energy-regeneration system are the material RENDERER; and full-length peptide yield, speed, and error are OBSERVABLES. WRRA's core lies in not confusing information with its executor.

## 64.1 Ownership of Sequence and Executor

DOI 10.5281/zenodo.22290829 treats minimal gene execution between the whole-cell structure of Life Model I and the generational calculation of Life Model III. Writing execution output as Y = Φ(D,E,X₀,t), D is the DNA specification, E the executor inventory, and X₀ the initial chemical state. In ordinary DNA-directed protein synthesis, the absence of E means there is no catalytic path and therefore no protein output.

Y=Φ(D,E,X₀,t), E=empty ⇒ Yprotein(t)=0

Even if DNA encodes polymerases, translation factors, and ribosomal proteins, the first decoder and generator must already exist. This no-bootstrap result is not a theorem that autonomous life is impossible, but an ownership audit showing that a DNA-only proposal hides material initial conditions.

## 64.2 Exact Coding Floor and the Undefinable Shortest Cassette

A peptide of n residues including the initiating amino acid requires n sense codons and one stop codon; under the ordinary triplet code, the pure-coding lower bound is exact.

Lcoding,min(n)=3n+3 nucleotides

A physical expression cassette, however, requires a promoter, leader, ribosome-binding site, terminator, ions, and recognition rules. In L\_cassette = 3n+3+R, R depends on the executor and assay, so a “universally shortest expression DNA” without a fixed executor is null/OPEN rather than zero.

## 64.3 Length-Dependent Limit of Translation Processivity

Substituting the 2021 PURE-system interval of processivity loss per codon, δ = 1.3 × 10⁻³–13.2 × 10⁻³, into an independent-dropout model makes the probability of full-length production decrease exponentially with length.

Pfull(n|δ)=(1-δ)ⁿ, n₅₀=ln(0.5)/ln(1-δ)

The 50% full-length scale in this calculation is 532.8 residues at the low-loss boundary and 52.2 residues at the high-loss boundary. This is not a universal law of translation but a model-conditional ceiling obtained by transforming the stated empirical interval. It can be tested in holdouts that vary ORF length in the same executor without retuning δ.

## 64.4 The Present Boundary of Seeded Execution and Self-Regeneration

The 2001 PURE system experimentally closed DNA-to-protein execution in a seeded renderer supplied with purified ribosomes, tRNAs, aminoacyl-tRNA synthetases, translation factors, and energy chemistry. Cell-free expression inside a vesicle adds a boundary, but does not establish autonomy when the executor and metabolism are supplied externally.

A 2026 report synthesized PURE's 36 nonribosomal proteins using PURE and reconstructed a functional second-generation PURE system. The regeneration efficiency per reaction was only 8%, however, below the minimum ledger value of one required for sustained replacement.

Rnonribosomal=0.08<1 ⇒ sustained replacement FAIL

## 64.5 Assessment and Frozen Predictions

The exact coding floor is EXACT UNDER ORDINARY TRIPLET CODING; protein production by DNA alone is EXCLUDED IN ORDINARY CHEMISTRY; seeded purified expression and functional reconstruction of the 36 nonribosomal proteins are EXPERIMENTAL PASS; the length–processivity relation is DERIVED/MODEL-CONDITIONAL; sustained self-regeneration at 8% is FAIL; and seed-free generation of ribosomes and decoders and closure of membrane and generations remain OPEN.

Preregistration candidates are: ① yield, start point, and full-length fraction under executor swaps using the same DNA; ② log-linear completion rate on an uncalibrated length panel; ③ second-generation activity versus parent-generation activity for classes of essential executors; and ④ co-inheritance and descendant persistence with and without a regenerated membrane. If δ or thresholds are fitted on the same data, the result remains CALIBRATION.

Chapter conclusion A gene is a program, not its executor. WRRA Life Model II closes seeded DNA-to-protein execution, but autonomous minimal life jointly reconstructing decoder, energy, membrane, division, and lineage remains open.
