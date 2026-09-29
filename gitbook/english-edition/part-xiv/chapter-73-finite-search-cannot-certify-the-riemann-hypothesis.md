# Chapter 73 Finite Search Cannot Certify the Riemann Hypothesis

Conclusion of this chapter: DOI 10.5281/zenodo.22346428 does not claim that the Riemann Hypothesis itself is unprovable. Its exact conclusion is narrower and stronger. The fact that no counterexample was found at finite height, in finite samples and finite-order derivatives, at finite precision, and under a fixed cutoff cannot certify that no counterexample exists in the full infinite critical strip. One counterexample can be a finite witness, but absence across an infinite region cannot close through search alone without a separate global invariant.

## 73.1 The Problem and Exact Scope of a Finite Search Environment

For a nontrivial zero ρ, RH is the global proposition ξ(ρ) = 0 ⇒ Re(ρ) = 1/2. If existence of an off-critical-line zero in each height window I\_k = \[T\_k,T\_k+H] is recorded as b\_k, RH becomes the infinite conjunction b\_k = 0 for every k.

bₖ=1{∃ρ: ξ(ρ)=0, Re(ρ)≠1/2, Im(ρ)∈Iₖ}; RH ⇔ bₖ=0 for all k

Here finite search means a procedure that ① directly inspects only a finite height or compact region; ② queries only finite-order function values and derivatives at finitely many points; ③ represents values at finite precision or by finite enclosures; and ④ declares global absence of counterexamples solely because none was found in the inspected range. Analytic proofs compressing an infinite domain into finite logic through the functional equation, Euler product, positivity, or spectral invariants are excluded from this definition.

FINITE SEARCH = finite window + finite queries + finite resolution + no independent global invariant

After any finite K, ℕ\1,…,K} still has the same countably infinite cardinality as ℕ. This does not mean K+1 is infinite; it means that increasing a finite prefix never removes the infinity of the unexamined tail.

## 73.2 Completeness of Finite Sieves and Failure of a Fixed Cutoff

Let Π\_p remove multiples of prime p, Q\_p = I−Π\_p, and S\_cut(z) = product\_{p≤z}(I−Π\_p). For z < n ≤ z², passing S\_cut(z) is equivalent to n being prime. A composite n has a prime factor no greater than √n ≤ z and is removed, while a prime n > z is divisible by no p ≤ z.

z\<n<=z^2: S\_cut(z;n) survives iff n is prime

For every finite z, however, choose distinct primes p,q > z; then m = pq is composite but passes the fixed S\_≤z. This does not mean primality testing for an individual input n is impossible. Choosing z ≥ √n for each n decides it in finite time. What fails is the claim that one fixed cutoff can permanently close all natural numbers.

For every finite z, there exist primes p,q>z such that m=pq is composite and S\_cut(z;m) survives.

## 73.3 A Zero-Insertion Theorem Preserving Finite Jets

Suppose a general entire function f has been observed exactly through order r\_j at each of finitely many points z\_j. Select one unobserved point w and construct P and g as follows.

P(z)=product\_j (z−z\_j)^(r\_j+1), g(z)=f(z)−f(w)P(z)/P(w)

Because P vanishes to order at least r\_j+1 at every z\_j, g^(k)(z\_j) = f^(k)(z\_j) for 0 ≤ k ≤ r\_j, while g(w) = 0. A finite exact jet transcript therefore cannot certify global zero-freeness in an unobserved region.

This theorem is an information-theoretic no-go for the class of general entire functions. It does not mean that the constructed g preserves ξ's Euler product, exact growth rate, arithmetic coefficients, and functional equation. It therefore does not exclude a global structural theorem specific to ξ.

## 73.4 Finite Precision and the Boundary of Critical-Line Identity

Writing a zero as ρ = 1/2+δ+iγ, numerical assessment of RH asks whether δ is exactly zero. If quantizer Q\_ε at resolution ε maps |δ| ≤ ε to the same output, it does not distinguish δ = 0 from 0 < |δ| < ε.

Qε(δ)=0 if |δ|≤ε, 1 if |δ|>ε; Qε(0)=Qε(δ) for 0<|δ|<ε

ε can be reduced indefinitely, but every finite stage leaves a smaller nonzero δ. This is a deterministic limitation of finite-precision representation, not an assumption that physical space is quantized. The observation “numerically very close to 1/2” is not a substitute for exact identity.

## 73.5 Local Detectors and Jensen Closure

A 2×2 mixed-corner difference telescopes along cell boundaries but can give zero for symmetrically placed interior zeros. A 3×3 nine-point Laplacian amplifies an isolated-zero signal faster than a harmonic background and can serve as a recursive detector on compact regions, but no fixed finite stencil escapes the finite-sample limitation of Section 72.3.

When ξ(c) ≠ 0 and the boundary circle contains no zero, define the Jensen circular-mean defect as follows.

Jₕ(c)=(1/2π)∫₀²π log|ξ(c+h e^(iθ))|²dθ−log|ξ(c)|² = 2Σ|ρ−c|\<h mρ log(h/|ρ−c|)≥0

If the open disk contains no zero, J\_h(c) = 0; if it contains a zero, J\_h(c) is positive. If the nearest center satisfies |ρ−c| ≤ h/√2, then J\_h(c) ≥ log 2 at a sufficiently small admissible scale. Restricting the disk by Re(c)−h > 1/2 or Re(c)+h < 1/2 produces an off-line detector excluding critical-line zeros. It is complete on each finite disk, but does not finish all infinite heights in finitely many steps.

## 73.6 The Global Zero-Mass Integral Is a Definition, Not Yet an Algorithm

Let u(s) = log|ξ(s)|². In the distributional sense, Δu(s) = 4πΣ\_ρm\_ρδ\_ρ. For the right half of the critical strip Ω\_+ = {1/2 < Re(s) < 1} and an admissible weight w that is positive at every height and decays sufficiently rapidly for the weighted sum over zero density to converge, define the following global quantity.

E+(w)=(1/4π)∫Ω+ w(Im s)Δlog|ξ(s)|²dA(s)=ΣRe(ρ)>1/2 mρw(Im ρ)

If an admissible w is strictly positive at every height and the weighted sum and integral converge, RH ⇔ E\_+(w) = 0. This equation is a complete definition containing every infinite height, but no independent finite procedure has yet been given to calculate its exact value as zero. Writing infinite information in one line with an integral sign is not the same as compressing infinite information into a finite computation.

## 73.7 The N×M Prime–Zero Relation Ledger

Writing the relation between ρ\_j = 1/2+δ\_j+iγ\_j and natural number n as A\_jn = n^(−ρ\_j), every row on the critical line has radial factor one, whereas an off-line row contracts or expands as n^(−δ\_j).

Aⱼn=n^(−1/2)e^(−δⱼlog n)e^(−iγⱼlog n), Rⱼn=|Aⱼn|/n^(−1/2)=n^(−δⱼ)

A direct-comparison ledger for M zeros and N arithmetic modes has size M×N. This must not be claimed as a lower bound on the computational complexity of every algorithm. Multiplicativity A\_j,mn = A\_jmA\_jn and analytic transforms can compress composite columns. The exact conclusion is that a fixed finite-dimensional sample ledger cannot, by search alone, terminate the possibility of infinitely many newly appearing zero rows.

## 73.8 Main Theorem: Non-Certifiability within the Defined Search Class

Main Theorem 72.1 — PROVED WITHIN THE DEFINED CLASS. A search procedure using only finite height, finitely many exact jets or finite-precision enclosures, and the absence of counterexamples in the observed range cannot logically and completely certify the truth of RH.

The proof has three clear steps. First, if the procedure terminates in finite time, the region above some T remains unexamined. Second, if the set of queried points and derivative orders is finite, g from Section 72.3 has both the same transcript and a zero outside the observed range. Third, finite precision is weaker than exact jets and adds the critical-line-identity limitation of Section 72.4. A global conclusion therefore requires a global invariant law independent of the search data, at which point the procedure leaves the defined search-only class.

This theorem does not state that RH is independent of ZFC and does not exclude a finite analytic proof using ξ's full structure. A finite sentence can compress an infinite object, as Euclid's proof of the infinitude of primes shows. What is frozen is the route of completing a global proof by indefinitely enlarging a finite list of absent counterexamples.

## 73.9 The Boundary from Analysis to Prediction

Calculating a finite K windows and obtaining b₁ = … = b\_K = 0 is analysis of the examined present. The moment one declares b\_k = 0 for every unopened k > K, the statement becomes prediction rather than proof.

finite analysis: b₁=…=bK=0; unopened-tail prediction: bₖ=0 for every k>K

The route back to proof is not to visit every window, but to show that finite state S\_k and transition T preserve a safe set A: S₀ ∈ A, T(A) ⊆ A, and S\_k ∈ A ⇒ b\_k = 0. The WJNS studies of finite-window transport, boundary carry, and no-burial sought such a transition invariant, but safe-set invariance has not yet been proven for the arithmetic kernel of the actual ξ.

## 73.10 Computational Labor and the Minimal-Computation Principle

By the Riemann–von Mangoldt law, the number of nontrivial zeros up to height T grows at leading order as T log T.

M(T)≈(T/2π)log(T/2π)−T/2π; Cdirect(T)∝N(T)M(T); Cgrid(T,h)∝T/h²

Directly comparing each zero with N(T) modes costs N(T)M(T) ledger operations, while a planar grid of spacing h requires approximately T/h² cells. If h(T) → 0 as T grows, direct-search labor grows still faster. This is not a universal complexity lower bound on every possible algorithm, but a scale audit of the direct-search, grid, and relation-ledger models defined in this chapter.

The methodological interpretation of Minimal Computation Cosmology is that reality must be realized through finite generators and conserved transition invariants rather than by exhausting an infinite ledger item by item. Brute-force routes expanding as T log T, N(T)M(T), and T/h(T)² with scale are therefore inconsistent with the minimal-computation principle. The principle “nature should be simple,” however, does not by itself prove the independence or impossibility of RH.

## 73.11 Final Frozen Assessment

FROZEN THEOREM. However large a finite environment becomes, the absence of a detected zero within it cannot certify the absence of off-critical-line zeros throughout the infinite domain. Increasing size moves the boundary; it does not remove it.

The frozen route is a search-only attack seeking to complete RH through a higher cutoff, finer grid, larger stencil, or longer numerical verification. The remaining route is an independent global invariant that compresses infinite height into a finite law through ξ's functional equation, Euler product, positivity, or spectral structure.

Chapter conclusion The exact final sentence is not “RH is unprovable,” but “the truth of RH is not proven by completion of finite search alone.” Unless a separate analytic theorem compresses the infinite-zero problem into a finite structural law, search only enlarges the analyzed past and does not eliminate prediction concerning an unexamined infinite tail.
