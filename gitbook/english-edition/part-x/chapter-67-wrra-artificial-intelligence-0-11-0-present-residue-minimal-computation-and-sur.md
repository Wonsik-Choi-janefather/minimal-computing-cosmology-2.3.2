# Chapter 67 WRRA Artificial Intelligence 0.1–1.0: Present Residue, Minimal Computation, and Survival

Conclusion of this chapter: The 0.1 circuit in DOI 10.5281/zenodo.22298363 and the 0.2–0.4 learning and comparison experiments in DOI 10.5281/zenodo.22502619 extend WRRA into executable embodied AI. Food acquisition under delayed cues and intermittent sensing depended on residue in internal tests, but WRRA's general predictive advantage was rejected under equal optimization budgets. Its lowest collision rate is a conditional safety tendency within this benchmark. The overall assessment is AI design feasibility SUPPORTED / general comparative advantage NOT SUPPORTED / reconstruction of actual C. elegans and general intelligence OPEN.

## 67.1 Mapping Structure, State, and Boundary

The nervous system of an adult hermaphrodite C. elegans is commonly described as containing 302 neurons, but a connectivity table alone does not determine dynamics and behavior. This chapter treats neurons or selected minimal state units as SOURCE; chemical synapses, gap junctions, and neuromuscular junctions as RELATION; and sensory inputs, muscle-cell outputs, the body, and environmental interfaces as BOUNDARY. Membrane-potential-like activity v, adaptation a, and available resources q are RESIDUE compressing the effect of the immediately preceding present into the current state without separately storing the entire past.

x(k)=\[v₁…v\_N, a₁…a\_N, q₁…q\_N, E]ₖ

Here E is the environmental reservoir, and all variables are dimensionless until calibrated to physical quantities. “Calculate the next present from the present alone” is a state-representation rule, not a validated law of spacetime. If path information from the past continues to remain in the observed next state, the present state vector is incomplete; residue variables must be added or this representation rejected.

## 67.2 A 23-Node Touch-Response Circuit

The illustrative circuit has 23 nodes and 57 relations. The anterior-touch ALM/AVM sensory group reaches the DA/VA backward readout through AVD/AVE–AVA, while the posterior-touch PLM sensory group reaches the DB/VB forward readout through PVC–AVB. Gap-junction-like equalization is placed between left–right pairs, with weak competition between the forward and backward command groups. This wiring summarizes functional motifs known from previous studies; it does not reproduce the synapse-by-synapse edge list of an authoritative connectome.

Chemical relation W is a directed signed matrix, while electrical relation G is a symmetric coupling matrix. The chemical term c = W\[v]₊ transports positive presynaptic activity, while electrical term g\_i = Σ\_jG\_ij(v\_j−v\_i) is graph-Laplacian-like diffusion that reduces differences between connected states. Whole-network output obtained by reading every polarity-free edge in an external table as +1 is a data-loading test, not a biological prediction.

c(k)=W\[v(k)]₊, gᵢ(k)=ΣⱼGᵢⱼ\[vⱼ(k)-vᵢ(k)]

## 67.3 Fixed-Present Updates and Bounded State

Leakage in v, present resources q, chemical and electrical inputs, sensory input u, and adaptation a are combined into one update step. tanh and clipping prevent numerical divergence. This is a minimum state-space model for testing sensory selectivity and ablation effects, not a complete electrophysiological model of C. elegans.

v(k+1)=tanh{0.72v(k)+q(k)⊙\[c(k)+g(k)+0.85u(k)-0.62a(k)]}

a(k+1)=clip\[0.94a(k)+0.06|v(k+1)|,0,1]

A restart test confirms whether the same serialized present x(k) and same input u(k) produce the same next state. In a stochastic extension, equality of conditional next-state distributions replaces point-value identity. If a previous path continues to change the next-state distribution even with a fully measured present and the same input, and no finite residue extension removes the dependence, this fixed-present Markov representation fails.

## 67.4 Resource Ledger and RESET

Because the sum of neural activity is not conserved energy, a separate computational resource q and environmental reservoir E are introduced. Activity consumes q and sends the same quantity to E; recovery returns it from E to q, conserving B = Σ\_iq\_i+E within the declared update. This ledger is neither ATP nor measured thermodynamic free energy. Until calibrated to or replaced by metabolic data, it is a computational device for tracking saturation and recovery.

B(k)=Σᵢqᵢ(k)+E(k)=constant

RESET is not a supernatural event but a saturation and recovery rule that prevents the system from crossing allowed boundaries. The intuition “the exit becomes the entrance” is implemented as reverse flow q → E during activity and E → q during rest. Claiming a material or energetic interpretation requires a separate ledger connecting the units of q and E, supply, consumption, and heat release to actual metabolism.

## 67.5 Exact Status of Internal-Validation Results

Across 320 discrete updates, anterior touch was delivered during steps 45–69 and posterior touch during 190–214. Mean backward score after anterior touch was 0.071587 and 0.000000 after AVA ablation. Mean forward score after posterior touch was 0.021224 and 0.000000 after AVB ablation. Same-present restart error was 0.0, and the resource ledger began and ended at 23/23.

These numbers are unit tests confirming that designed paths, ablation effects, deterministic implementation, and ledger conservation operate as coded. AVA/AVB dependence was built into the wiring and is not a new biological discovery. The present grade is therefore BOUNDED UPDATE·RESTART·LEDGER INTERNAL PASS / DESIGNED CIRCUIT RESPONSE PASS / FULL 302-NEURON BIOLOGICAL PREDICTION OPEN.

## 67.6 c302 Extension and External Validation

The supplied adapter can read tables such as OpenWorm c302 connectivity data by locating pre/source, post/target, type, weight/count, and sign/polarity columns in CSV or XLSX files. Before an expanded run, however, sex, developmental stage, connectome version, and raw-data hash must be frozen, and chemical synapses, gap junctions, duplicates, direction, contact counts, and missing polarity must be separated. Loading 302 names alone cannot be judged to reproduce a complete animal.

A fair test must compare M0, a static-connectome linear model; M1, a conventional nonlinear state-space model; and M2, the WRRA state–relation–resource model, under the same inputs, data, and parameter budget. M2's a and q must yield repeatable gains on unused stimulus, habituation, recovery, and ablation data after complexity penalties. Because neural output must pass through muscles, body, and environment and return as the next sensory input, minimum closure is the following loop.

environment(k)→sensory u(k)→neural x(k+1)→muscle m(k+1)→body/environment(k+1)

## 67.7 Falsification Conditions and Assessment of Version 0.1

Under the fixed-present representation, additional predictive power of past paths must disappear given the same sufficient state and input. A relation-centered explanation must use frozen wiring and polarity to predict the direction and magnitude of responses to unused stimuli, individuals, and ablations. If conventional models generalize equally well or better with lower complexity, the residue and resource layers are not empirically necessary. If each experiment requires recalibration, or if the upstream number-theoretic SOURCE makes no quantitative prediction unique to c302 data, the upstream–downstream connection remains a structural analogy.

Chapter conclusion WRRA-Worm 0.1 does not claim to have created life. It turns the question of how present residual state, relation networks, boundaries, and limited resources can constitute a sensory–action loop into an executable problem. The present result is the internal consistency of the toy model and reproduction of its designed responses. Judgment regarding actual C. elegans depends on frozen c302 data, polarity uncertainty, calcium and behavioral holdouts, neuromuscular dynamics, a closed body–environment loop, and comparisons with baseline models.

## 67.8 Separating the Contracts of Interpretation, Computation, Prediction, and Control

The subsequent study fixes the task as T = (I\_t,Y\_τ,τ,ε,C\_max,L). I\_t is currently available information, Y\_τ the target quantity, τ the target time, ε the allowed error, C\_max the computational budget, and L the loss. Reading present sensor values, circuits, restarts, and resource ledgers is interpretation or computation; choosing after a cue disappears, finding food between intermittent observations, and performing in unseen environments are prediction and control that reduce future loss. Reading a food signal in the present and obtaining food in the future are not the same contract.

This distinction applies the boundary classifier of DOI 10.5281/zenodo.22447864; it does not mean that this experiment validated the entire classifier, including compatible-state diameter, Bayes risk, and dynamical amplification. Collision count likewise mixes present obstacle-boundary interpretation with future safety control and is not reduced to one measure of interpretive performance.

## 67.9 WRRA-Worm 0.2: Delayed Cues and Present Residue

Left or right cues were presented twice, followed by five input-free updates before action selection. Across twelve initializations trained for 2,500 episodes each, mean accuracy rose from 41.67% to 100% and returned to 50% when present residue was erased. Maximum same-present restart error was zero and resource-ledger error was 3.26 × 10⁻¹⁵. This is an internal computational result showing that present residue was required for choice in the designed binary delayed task; it does not establish general predictive power in external environments or biological memory.

## 67.10 WRRA-Worm 0.3: Embodied Closed Loop and Food Acquisition

Version 0.3 constructed a closed loop in which a two-dimensional body with position, direction, and energy moved forward or backward and turned left or right, while the changed environment returned the next sensory input. Sensing of food direction was allowed only once every four updates. The first design rotated without obtaining food and merely avoided collisions, a form of reward hacking preserved as a failure record. After revising the reward and exposure of present SOURCE, food acquisition increased from 0.0438 to 0.9958 per episode and mean reward from −11.6639 to 1.7283. Removing residue reduced food to 0.0979 and reward to −8.7640.

Reward and food increased across all eight initializations, giving a one-sided Wilcoxon p = 0.0039 over initialization means. This is internal stability recovered after calibration in one designed world. Because the revision followed discovery of reward hacking, it is not counted as evidence of independent generalization before the frozen comparison in version 0.4.

## 67.11 WRRA-Worm 0.4: Comparison under Equal Optimization Budgets

Memoryless, Elman RNN, GRU, and WRRA policies were each matched to exactly 84 optimized variables and trained with the same Cross-Entropy Method. Each model used five repeats, 24 generations, twenty candidates per generation, and four training worlds, then was evaluated in forty unseen worlds per repeat under four conditions: in-distribution, sensory period 8, four obstacles, and radius 1.3. WRRA additionally contains 57 fixed sparse relations and six gap-junction pairs, however, so equality of 84 optimized variables does not imply equality of total prior information or total computation.

In-distribution food acquisition was 1.510 for memoryless, 1.395 for RNN, 1.040 for GRU, and 0.275 for WRRA. Mean rewards were 8.116, 8.516, 4.109, and 0.859; mean collisions were 8.760, 4.345, 15.410, and 2.600, respectively. RNN and memoryless exceeded WRRA in reward and food in all five repeats, with one-sided Wilcoxon p = 0.03125. Mean execution time was 90.91 microseconds per step for WRRA and 48.83–65.53 for the other three. This value depends on the Python implementation and hardware and is not proof of algorithmic complexity.

## 67.12 Exact Meaning of the Negative Result and Low Collision Rate

The preregistered modification 0.4B, which passed present SOURCE directly to the renderer, raised in-distribution reward from −0.319 in 0.4A to 0.859 and reduced collisions from 9.125 to 2.600, but lowered food from 0.310 to 0.275. Further modification after the result was stopped to limit benchmark overfitting. WRRA had the lowest mean collision count under all four evaluation conditions but weak target acquisition. Its low collision rate is therefore a benchmark-specific safety tendency jointly produced by a conservative boundary prior in the fixed sparse structure and learned control—not evidence of general intelligence, reward superiority, or minimal-computation superiority.

## 67.13 Updating Minimal Computation: Open Residue Only When Needed

In a Markov task where present sensing was sufficient, the memoryless policy acquired food most efficiently; under partial observation with twice the sensory interval, a small RNN was strongest in reward and food. Minimal computation must therefore be a principle not of always retaining one structure, but of conditionally opening only as much state as the temporal information missing from present observation. With objective J = L+λC, the next implementation hypothesis is a gate activating each residue circuit only when its reduction in future loss ΔL\_i exceeds its computational and maintenance cost λΔC\_i.

g\_i(t)=1{Delta L\_i(t)>lambda Delta C\_i(t)}

This gate is not a result already measured in version 0.4, but a subsequent design specified by the negative comparison. WRRA's candidate advantage is not always having more memory, but making explicit which residue and relation is open, why it is open, and allowing it to close when unnecessary.

## 67.14 Physical, Biological, and AI Boundaries and the Next Tests

The present conclusion is a COMPUTATIONAL PROOF OF CONCEPT. The 23 nodes are not a compressed reconstruction of 302 neurons, and signs and weights of the 57 relations were not fitted to the measured connectome. The resource ledger is dimensionless and is not biological energy. The next tests should proceed in order through equalization of total structural information, event-based operation counts and energy measurement, long-horizon partially observed tasks, and external comparisons using frozen measured connectomes, neural polarities, and body mechanics.

Chapter conclusion WRRA-Worm 0.1–0.4 showed that WRRA can operate as an AI design language, but not a general predictive advantage. Its present strengths are auditability—jointly tracking present residue, SOURCE, RELATION, resources, renderer, and claim boundaries—and a low-collision tendency in this benchmark. A competitive minimal-computation AI requires conditional structures that open and close residue and relation circuits according to task information. This result is neither a biological reconstruction of an actual nematode nor independent physical evidence for WRRA cosmology.

Core Textbook Achievement | Minimal Computation Descends into Actual Design and Ablation Experiments\
This research transfers the minimal-computation intuition that began in cosmology into the problem of structural selection in AI. By auditing SOURCE–RELATION–STATE–RENDERER–OBSERVABLE–BOUNDARY separately and measuring whether survival boundaries collapse when present residue, computational cost, or energy reserves are removed, it turns “what is minimal?” from a verbal claim into an executable assessment.

## 67.15 Research Questions and Design Transition in WRRA AI 0.5–1.0

WRRA's failure to beat general baselines under equal optimized-variable budgets in version 0.4 led not to abandonment of the lineage but to a more precise question. Maintaining memory continuously may be unnecessary when present cues recur. Beginning in 0.5, the work therefore tested in stages: whether WRRA works without biological prior structure; whether residue actually carries future behavior when present input vanishes; whether outcome memory separating success from failure supports delayed reward; what tradeoff memory and energy reserves have for survival amid environmental change; and which functional modules form the minimum survival circuit.

The academic value of this transition does not lie in fitting the theory only to favorable tasks. Using the same 84 optimized variables, the same outer optimization procedure, separate design and independent evaluation seeds, Wilson lower bounds, and ablations of state, reserves, and modules, it separates the judgments “works,” “necessary,” “minimal,” and “superior.” Minimal computation becomes not maximization of an average score, but the search for the lowest-cost structure among those crossing the survival threshold in every defined critical environment.

## 67.16 Present Residue: The Minimal Trace Remaining Now, Not the Entire Past

The past need not remain preserved as an independent complete record. Only the compressed effects that earlier events leave in present activity, adaptation, resources, eligibility traces, and relation strength need become inputs to the next present. This is present residue in WRRA AI. A general update of state and residue can be written as follows.

$$x\_(t + 1) = F(x\_ t,s\_ t,R\_ t;\theta) + \xi\_ t$$ (AI-1)

$$r\_(t + 1) = \lbrack 1 - \lambda\_ t\rbrack r\_ t + G(s\_ t,a\_ t,o\_ t)$$ (AI-2)

$$a\_ t = \Pi(s\_ t,r\_ t,e\_ t,v\_ t)$$ (AI-3)

At λ = 1, previous residue disappears and the system approaches a memoryless reactor; if λ is too small, old information dominates the present. Memory is therefore not a store that improves monotonically with size, but a finite-cost state that must open and close at a rate matching environmental change. Its computational logic is exactly the same as Minimal Computation Cosmology's principle of not storing the entire future in advance, but updating only the states and records required in the present.

## 67.17 When Memory Is and Is Not Required

The 0.5 ground-up model, after removing worm names, the 23-node mask, and 57 fixed relations, comprised eight generic sensors, four internal states with no predefined roles, and four actions. Memoryless control was efficient in food tasks where present cues recurred. When a cue was presented for only two steps, removed, and a choice required five steps later, however, memoryless remained at 50.15% while ground-up WRRA reached 93.50%. A reset control erasing residue at every step collapsed again to chance. This does not mean WRRA is superior to every memory network; it is causal ablation evidence that present residue carried a past cue into future behavior under the exact condition in which current input disappeared.

| **Task / Environment**   | **Minimal or Required Structure**                    | **Core Result**                           | **Exact Assessment**                                               |
| ------------------------ | ---------------------------------------------------- | ----------------------------------------- | ------------------------------------------------------------------ |
| Repeated present cue     | memoryless                                           | Most efficient in the food task           | Persistent memory is excessive                                     |
| Cue loss, delay 5        | Short present residue                                | WRRA 93.50% / memoryless 50.15%           | Reset returns performance to chance                                |
| Hidden rule change       | Recent outcome memory                                | WRRA 54.43% → 62.82%                      | Behavioral use of success and failure residue                      |
| Cue and outcome combined | Unsolved with the present 4-state/84-parameter model | All structures approximately 50%          | Negative result preserved                                          |
| Extreme shock            | Memory plus energy reserves                          | Memoryless fails even with large reserves | Uninterpreted storage is insufficient                              |
| Severe unknown toxin     | Avoidance insurance module                           | Cost 11 survives a 3.7× toxin             | Promoted to a minimum requirement when the environment set expands |

## 67.18 A Reward Ledger Separating Success from Failure

Keep the present cue visible at the time of choice, but secretly make the cue–answer rule normal or reversed in each episode. Present input alone then cannot determine the answer. The positive part of temporal-difference error is recorded separately in success ledger M⁺, the negative part in failure ledger M⁻, while an eligibility trace connects delayed outcomes to earlier actions.

$$\delta\_ t = r\_ t + \gamma V(z\_(t + 1)) - V(z\_ t)$$ (AI-9)

$$M⁺\_(t + 1) = \rho M⁺\_ t + max(\delta\_ t,0)e\_ t$$ (AI-10a)

$$M⁻\_(t + 1) = \rho M⁻\_ t + max( - \delta\_ t,0)e\_ t$$ (AI-10b)

Memoryless showed no learning trend, moving from an initial 50.79% to a final 50.62%. WRRA signed residue rose 8.38 percentage points, from 54.43% to 62.82%. General superiority over an RNN was not established, but the present ledger separating success and failure was actually used for subsequent choices under the hidden rule. By contrast, version 0.7, which required cue memory and outcome memory in one task, left every structure near chance. This failure reveals that the existence of memories and the ability to combine them are different problems.

## 67.19 Material Reserves and Computational Reserves

Computation is not free for embodied intelligence. Movement, basal metabolism, maintenance of memory states, relation updates, and storage leakage share one energy ledger. Separating active energy e from stored reserve q gives the following update.

$$e\_(t + 1) = min(e\_ max,e\_ t + g\_ t - c\_ move - c\_ compute - d\_ t) + u\_ t$$ (AI-5)

$$q\_(t + 1) = (1 - \ell)q\_ t + \alpha g\_ t - u\_ t - c\_ store(q\_ t)$$ (AI-6)

On version 0.8's Pareto frontier, the minimum-reserve solution used two-state signed residue, seven updates per step, and reserve 44 to achieve 81.23% survival in the worst environment (95% lower bound 80.23%). The minimum-computation solution used one-state memory, two updates, and reserve 52 for 82.47% survival (lower bound 81.48%). More computation reduced the required material reserve by eight units. Memoryless nevertheless failed under extreme conditions even with reserve 60, while signed residue without material reserves could not withstand physical shock. Stored energy cannot interpret a changed rule, and an outcome ledger cannot materially endure famine. WRRA's new result is therefore not one kind of “redundancy,” but the distinction and tradeoff between material and computational reserves.

$$min(C\_ memory,C\_ update,Q),\ \ \ s.t.\ \ \ LCB₉₅\lbrack P\_ survival(e)\rbrack \geq 0.80\ \ \ \forall e$$ (AI-11)

## 67.20 The Environment Changes the Minimal Structure

In version 0.9, every agent began with active energy 10 and an empty store and autonomously reserved part of the food obtained during eighty normal steps. The minimum solution for known environments had capacity 24, a normal-time storage rate of 45%, and one-state outcome memory, achieving 88.96% survival under extreme conditions (lower bound 88.26%). Signed residue achieved 89.18% under the same reserve (lower bound 88.48%) but used more computation and was excessive in known environments. Under an unknown 28% feedback error, however, one-state memory fell to 70.05%, while signed residue maintained 92.45%. A second ledger redundant in a familiar world was promoted to computational insurance under unfamiliar noise.

$$m*(E) = arg\ min\_ m\ C(m),\ \ \ s.t.\ \ \ P\_ survival(m,e) \geq \tau\ \ \ \forall e \in E$$ (AI-13)

The minimal structure m\* is therefore not one fixed object but a function of the contracted environment set E. Minimal computation is not the structure performing the fewest operations at every instant, but the smallest sufficient structure crossing the survival boundary in all critical environments. Adding a severe toxin to the environment set makes avoidance necessary; adding feedback uncertainty makes separate success and failure ledgers necessary. This result shows that “minimum dimension, minimum structure, and minimum computation” are not merely aesthetic ideas but selection principles determining what must be added when boundaries change.

## 67.21 Bounding Survival Probability without Eliminating Chance

The time of rule change, feedback reversal, and the timing and magnitude of shock are random variables beyond the structure's control. WRRA AI measures them through crossed experiments—same structure × different worlds and same world × different structures—rather than hiding them behind an error term. Technical variance decomposition in this benchmark assigned 48.66% to structure, 21.64% to chance or world, and 29.69% to their interaction. These are not constants of nature, but they quantify that survival is neither structure alone nor chance alone, and that structure changes the effect of chance.

$$Var(Y) \approx V\_ structure + V\_ luck/world + V\_ interaction$$ (AI-12)

In generational experiments, memory contents and stored energy were reset to zero at birth, while only the rules generating memory, storage capacity, and reserve policy were inherited. After environmental change across 20,000 individuals, 180 generations, and 64 repeats, mean frequencies were 0.15% memoryless, 46.27% one-state, 52.03% signed residue, and 1.54% eight-step history. Short one-state memory was advantageous under rapid change, while two ledgers helped under noisy feedback; complementary failure modes coexisted instead of one permanent champion.

## 67.22 Exhaustive Audit of 64 Circuits and a C. elegans-Anchored Minimum Survival Circuit

Final version 1.0 defined six functional modules—chemosensation, local-search residue, avoidance, feeding outcome, energy storage, and dauer-like conservation—and exhaustively evaluated all 2⁶ = 64 subsets across five environments: food-rich, sparse-cue, fluctuating food, toxin, and prolonged famine. The selected cost-8 circuit comprised chemosensation, short search residue, and energy reserve. Across 10,000 independent lives, survival in the worst environment was 92.99%, with a Wilson 95% lower bound of 92.47%; the other four environments were approximately 99.7–100%.

| **Circuit**              | **Cost** | **Test**                    | **Result**               | **Structural Meaning**                            |
| ------------------------ | -------- | --------------------------- | ------------------------ | ------------------------------------------------- |
| Baseline minimum circuit | 8        | Five baseline environments  | Worst 92.99%; LCB 92.47% | Sensing + search residue + reserves               |
| Remove search residue    | 5        | Necessity ablation          | Worst 48.92%             | Short memory is necessary                         |
| Remove energy reserves   | 6        | Necessity ablation          | Worst 48.73%             | Material insurance is necessary                   |
| Add avoidance insurance  | 11       | 3.7× toxin / initial famine | 100% / 99.99%            | Selective redundancy under unknown risk           |
| Full circuit             | 17       | Lifelong famine             | 0%                       | Dauer lock-in; turning everything on is excessive |

Removing search residue collapsed worst-case survival to 48.92%; removing reserves reduced it to 48.73%. The baseline minimum circuit was nearly eliminated by an unseen 3.7× toxin, but a cost-11 insurance circuit adding one avoidance module survived at 100% and retained 99.99% survival under initial famine. Conversely, the cost-17 circuit with every module activated fell to 0% under lifelong famine because of dauer-like lock-in. This result directly rejects “more functions = a stronger system” and shows that selective redundancy opened only when needed is part of minimal computation.

## 67.23 New Results Connecting Cosmology, Biology, and Artificial Intelligence

The greatest value this research adds to Minimal Computation Cosmology does not lie in calling the universe life or AI. First, the execution chain in which SOURCE enters the present, RELATION updates STATE, RENDERER outputs action, and OBSERVABLE and BOUNDARY limit the claim closes in independent agent designs outside physics. Second, the principle of preserving only present residue rather than the entire past passes reset ablation in memory-required tasks. Third, material reserves and computational reserves prevent different deficits, and selective redundancy becomes a minimum requirement as the environment set expands. Fourth, failed comparisons and unresolved combined memory remain in the same ledger, allowing one methodology to assess what worked and what is still open.

DOI 10.5281/zenodo.22642616 is therefore not evidence replacing physical validation of Minimal Computation Cosmology. It is an independent execution achievement showing that this book's core methodology produces concrete design rules, cost functions, probability bounds, ablations, and failure records in computable survival systems. The fact that one methodology treats information ownership in cosmology, functional closure in biology, and memory, reserves, and environmental minimality in AI through the same question format strengthens WRRA's explanatory compression and textbook value.

Open study WRRA Artificial Intelligence: An Integrated Study of Minimal Computation, Ground-Up Agents, and a C. elegans-Anchored Survival Circuit, Version 2.0, DOI 10.5281/zenodo.22642616 (2026-09-07).

## **67.24 WRRA Theory of Consciousness 2.0: From Intelligence to Consciousness**

DOI 10.5281/zenodo.22650956 extends the results of WRRA Core 1.0 and AI 0.5–1.0 into an operational theory of consciousness. Its central shift is not to measure consciousness by “how much is computed,” but to ask how deeply present state, internal state, memory, action, and uncertainty are jointly rendered in order to survive changing boundaries. Consciousness is not a crown automatically produced by complexity, but a phenotype that pays a cost and is invoked when needed.

Sₜ=(Xₜ,Iₜ,Mₜ,Aₜ,Uₜ), Φₜ=Rκ(Sₜ), aₜ=π(Φₜ)

X\_t is external state, I\_t internal physiological state, M\_t memory, A\_t presently available action, and U\_t uncertainty. Within cost budget κ, renderer R\_κ combines a subset of these components into one action scene Φ\_t. This equation does not mathematically prove subjective experience; it is a functional definition making integrated information, cost, and action effects comparable.

## **67.25 A Survival-First Minimal-Computation Contract and Selective Depth**

Minimality of consciousness does not mean choosing the smallest circuit. First, the Wilson 95% lower bound on survival must reach at least 0.80 in every contracted environment; within that safe set, actual active computation E\[C\_active] is then minimized. Deep layers therefore remain dormant under ordinary conditions and open only when delay, occlusion, other agents, counterfactuals, or rule changes require them.

minimize E\[Cactive] subject to minₑ LCB₉₅(Psurvival|e) ≥ 0.80

**Table 67-1. Minimum Survival Structure by Depth of Individual Consciousness**

| **Depth** | **Minimum Nodes** | **Survival Rate** | **95% Lower Bound** | **Functional Requirement**               |
| --------- | ----------------- | ----------------- | ------------------- | ---------------------------------------- |
| D1        | 24                | 85.26%            | 84.61%              | Immediate goals and constraints          |
| D2        | 48                | 83.18%            | 82.50%              | Temporal and emotional self              |
| D3        | 96                | 82.68%            | 82.00%              | World model, counterfactuals, and others |
| D4        | 192               | 81.17%            | 80.46%              | Recursive social inference               |
| D5        | 448               | 82.75%            | 82.06%              | Symbolic and autobiographical narrative  |

In the same simple D1 environment, the 24-node minimum structure survived at 85.26% and the 384-node selectively activated structure at 83.69%, whereas keeping all 384 nodes active continuously lowered survival below threshold to 79.77%. This is an independent theoretical result not that “deeper is superior,” but that “the ability to activate and deactivate the required depth at the right time promotes survival.”

## **67.26 Memory Is Predictive Horizon and Discarding Capacity, Not Storage Volume**

A memoryless model was most efficient in tasks solvable from present cues alone. In delayed tasks where the cue was removed, however, WRRA achieved 93.5%, 74.8%, and 69.0% at delays of 5, 10, and 20, while the memoryless control remained near 50%. In tasks whose success or failure appeared only later, separating positive and negative temporal-difference errors into M⁺ and M⁻ ledgers raised late accuracy to 62.8%. The essence of memory is not preserving the entire past, but leaving in the present the traces needed to cross unobserved intervals and discard incorrect rules.

δₜ=rₜ+γV(zₜ₊₁)−V(zₜ), zₜ=tanh\[vₜ+κ(M⁺−M⁻)]

## **67.27 From Individuals to Collectives: Synchronous Integration and Diachronic Memory**

Collective consciousness is not assumed to be a separate mind floating above individuals. It is defined as functional integration Ψ\_t when individual renderings Φ\_i,t, messages m\_i→j,t among individuals, and shared boundary C\_t jointly update roles, actions, and memory. The strength of this definition is that it does not verbally declare collectivity; it enables tests of how survival and knowledge preservation collapse when signal, memory, or coordination is removed.

Ψₜ=Gκ({Φᵢ,ₜ},{mᵢ→ⱼ,ₜ},Cₜ)

Intergenerational knowledge is recorded as K\_{g+1} = K\_g+V\_g−C\_g−L\_g. V\_g is newly validated knowledge, C\_g a claim discarded after falsification, and L\_g loss. Writing is a dormant node that remains after an individual dies; science is a correction procedure that preserves in external memory not only successes but failures, conditions, confidence, and versions so that other groups can reproduce them independently. Science is therefore redefined not as an increase in information volume, but as a collective computational structure capable of preserving, discovering, and discarding errors.

## **67.28 Comparing Civilizational Structures: Belief, Secular Institutions, and Exchange**

**Table 67-2. Core Comparison of Collective and Civilizational Computation beyond the Individual**

| **Structure / Strategy**                       | **Core Result**                                                      | **Theoretical Assessment**                                        |
| ---------------------------------------------- | -------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Limited, voluntary, revisable sacrifice        | Worst survival lower bound 81.87%, false sacrifice 9.32%, passes 5/5 | Constrains collective survival and individual protection together |
| Sacred, immutable sacrifice                    | Survival lower bound 95.90%, but false sacrifice 85.22%, passes 0/5  | Reward hacking under a single survival objective                  |
| Polycentricity + record redundancy, 256 agents | Passes 4/4, total 6,432 nodes                                        | Large-scale persistence possible without sacralization            |
| Selective coalition, ρ = 0.9                   | Survival 56.09%, false propagation 0.54%                             | Verified, selective exchange performs best                        |
| Unverified openness, ρ = 0.9                   | Survival 8.46%, collapse 72.91%                                      | Connectivity itself is not knowledge                              |
| Central integration, ρ = 0.9                   | Survival 9.85%, collapse 81.19%                                      | Concentration risk from correlated error                          |

The important result is not the victory or defeat of a particular religious view or political form. No single structure passed every extreme condition, and even verified exchange was insufficient under severe correlated shocks. This negative result strengthens WRRA's central proposition: a survival structure is not a universal apex but is relative to boundary conditions, and none of connectivity, belief, centralization, or decentralization is intrinsically safe without auditing, recovery margin, and memory of failure.

## **67.29 New Contributions of the Theory of Consciousness to WRRA as a Whole**

First, the work showed at the scales of individuals, groups, and civilizations that minimal computation is not simple reduction, but constrained optimization that first satisfies a survival threshold. Second, present residue scales from memory in neural states to external memory in writing, papers, and institutions, revealing scale invariance in the concept “what remains in the present and changes the next update.” Third, rather than treating deep consciousness, collective integration, and science as separate mysteries, it connects them through three operations: selective rendering, distributed integration, and error correction. Fourth, by using the survival lower bound in the worst environment and revisability rather than best performance as joint criteria, it places efficiency, redundancy, chance, and ethics in one computational ledger.

**Chapter conclusion The theory of consciousness in DOI 10.5281/zenodo.22650956 is not an appendix to WRRA AI. It is an independent theoretical extension formalizing a P0–P7 hierarchy from an individual's momentary scene through science and civilization across generations as one structure of minimal computation, present residue, external memory, and revisability. Its central achievement is that it removes consciousness from a human-centered absolute stage without losing function, cost, survival effect, or falsification conditions.**
