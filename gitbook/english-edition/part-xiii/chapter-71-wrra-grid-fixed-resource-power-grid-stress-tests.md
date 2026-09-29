# Chapter 71 WRRA-Grid: Fixed-Resource Power-Grid Stress Tests

Conclusion of this chapter: “WRRA Grid Under Scarcity” compares six control architectures across seven disturbance axes in 50,400 episodes on a 14-bus toy power grid and performs a separate 20,000-episode paired memory ablation. Given the same resources and chance, memoryless local control G0 was the minimally sufficient solution for the present environment set. Medium reserve G2 produced a large survival gain at a strong compound boundary but fell below the preregistered passing line. Failure trace M1 also failed to recover the cost of its retained information. This result is WRRA's engineering achievement: it asks not whether memory, reserves, or centralization exist, but whether they convert into actual survival gains under fixed resources.

## 71.1 Ask about the Survival Threshold before Maximum Performance

WRRA-Grid selection does not maximize one average score. Only architectures passing the survival threshold in every contracted environment remain candidates; within that set, active computation, memory, communication dependence, and standing reserves are minimized. The minimum architecture is not universally one object, but relative to environment set E and resource budget B.

A\_pass = { A : min\_{e in E}\
LCB95\[P\_survival(A | e)] >= 0.80 } (GRID.1)

A\*∈arg min\_{A∈𝒜\_pass}(C\_active, M\_state, C\_comm, R\_committed) (GRID.2)

The four costs in Equation GRID.2 are compared through a Pareto and preregistered-priority ledger rather than forced into one score despite having different units. A structure that has a high average in one environment but collapses in another is not minimally sufficient.

## 71.2 The 14-Bus Model and Fixed-Resource Equation

The toy system is an IEEE-14-like topology with fourteen buses, twenty transmission lines, five generators, three renewable-energy sources, and up to five storage sites. Each episode has 96 steps and uses lossless linearized DC power flow, island-level supply–demand balance, and stochastic overload trips.

B=G\_MW+0.30E\_storage,MWh+8C\_base=408 (GRID.3)

Increasing storage capacity or baseline control complexity reduces installed generation capacity. Additional generation is not allowed. Active computation during operation is measured separately and not deducted twice from the asset budget. The values 0.30 and 8 are equivalent units in this experiment, not estimates of market cost.

## 71.3 Environments, Survival Conditions, and a Paired Same-Chance Design

Seven axes—heat wave, renewable-output collapse, generator trip, line trip, sensor noise, cyber false data, and compound boundary—were tested at ten stress levels from 0.50 to 1.50. Running 120 episodes per architecture, environment, and stress level produced 50,400 episodes in total.

survive ⇔ min\_t s\_total(t)≥0.55 ∧ no 3-step run\[s\_total<0.78] ∧ mean\_t s\_critical(t)≥0.96 (GRID.4)

A stress level passes only if the Wilson 95% lower bound on survival is at least 0.80. Random sequences for event time, demand, renewable output, sensor error, forced line, thermal derating, and cascading trip were shared among all controllers in the same environment and run. The comparison therefore measures responses to the same chance rather than assigning different luck to each architecture.

LCB₉₅=\[p̂+z²/(2n)−z√{p̂(1−p̂)/n+z²/(4n²)}]/\[1+z²/n], z=1.96 (GRID.5)

## 71.4 Fixed-Resource Results of Six Architectures

| **Model** | **Architecture**                       | **Resources: generation / storage / active computation** | **Worst passing stress, curve area, and assessment** |
| --------- | -------------------------------------- | -------------------------------------------------------- | ---------------------------------------------------- |
| G0        | Memoryless local control               | 400.0 MW / 0 MWh / 114.04                                | 0.60 · 85.34% · minimally sufficient solution        |
| G1        | Centralized current-state optimization | 388.0 / 0 / 315.49                                       | 0.60 · 74.97% · cyber-vulnerable                     |
| G2        | Single residual + reserves             | 369.0 / 90 / 183.02                                      | 0.60 · 85.09% · boundary robustness                  |
| G3        | Signed trace                           | 360.6 / 110 / 220.84                                     | 0.50 · 84.44% · cost not recovered                   |
| G4        | Distributed reserves                   | 343.4 / 170 / 203.96                                     | 0.50 · 84.09% · excessive reserve                    |
| G5        | Permanently overprovisioned            | 276.6 / 310 / 594.02                                     | 0.00 · 82.64% · fails at the lowest stress           |

The difference in area under the full survival curve between G0 and G2 was only 0.25 percentage points, and both passed worst-axis stress 0.60. Under WRRA's second rule, G0 is therefore selected because it meets the same worst-axis floor without storage and with less active computation. This does not mean G0 is best under every condition; it is the smallest architecture surviving as much as required.

## 71.5 Reserves Worked at the Boundary, but Excess Weakened the Present

At compound stress 0.70, G0 survived at 11.7% and G2 at 49.2%, a 37.5-percentage-point advantage for G2. The local value of medium reserves is clear, but G2's 49.2% remained below the preregistered 80% threshold and did not move the passing boundary by one level. In G4 and G5, storage and control displaced too much generation capacity and caused earlier failure. The value of reserves lies neither at zero nor infinity, but within a range that prevents boundary collapse without destroying present supply.

## 71.6 A Separate Memory-Required Task and the Implemented Trace

Most of the seven general disturbances are visible in current state, so G0's victory cannot establish the general uselessness of memory. A separate recurrent-shock task was therefore created in which a first shock depletes storage, a short normal recovery period follows, and a larger second shock arrives. M0 and M1 have identical sensing, storage, ramping, and communication; only M1 uses a negative trace of the first failure to increase recovery-period charging.

q\_t=s\_t^critical−0.06 min(o\_t,2)−0.02·1(trip\_t>0) (GRID.6)

m\_t⁺=0.91m\_{t−1}⁺+max(q\_t−q\_{t−1},0) (GRID.7)

m\_t⁻=0.91m\_{t−1}⁻+max(q\_{t−1}−q\_t,0) (GRID.8)

A positive trace is recorded but not connected to action selection; only a negative trace raises predictive margin and charging intensity. M1 is therefore an asymmetric failure-avoidance prototype, not complete bidirectional reinforcement learning. The two models shared the same 1,000 random sequences at each stress and were compared over 20,000 episodes.

## 71.7 Negative Result of Paired Memory Ablation

| **stress** | **M0 memoryless** | **M1 failure trace** | **M1−M0, paired bootstrap 95% CI** |
| ---------- | ----------------- | -------------------- | ---------------------------------- |
| 0.60       | 100.0%            | 100.0%               | 0.0%p                              |
| 0.70       | 83.6%             | 81.5%                | −2.1%p \[−3.3, −0.9]               |
| 0.75       | 72.4%             | 72.7%                | +0.3%p \[−0.7, +1.3]               |
| 0.85       | 28.5%             | 24.6%                | −3.9%p \[−5.3, −2.6]               |
| 1.00       | 0.0%              | 0.0%                 | 0.0%p                              |

The maximum stress satisfying an 80% Wilson lower bound was 0.70 for M0 and 0.60 for M1. Paired exact McNemar p values were 0.00075 at stress 0.70 and 7.6 × 10⁻⁹ at 0.85. M1 reduced unserved energy in some episodes but failed to convert retained information into sufficiently accurate anticipatory action; reduced generation capacity and increased computational cost exceeded the benefit.

The exact conclusion is not that “memory is useless.” Even in a task designed to require memory, this single decaying failure trace and charging rule failed to justify their own cost. The existence of memory and the existence of a useful memory policy are distinct propositions.

## 71.8 Academic Value Added to Power-Grid Research by WRRA

First, storage, memory, and centralization receive no free resources; the generation capacity they displace is included in the same budget. Second, the survival lower bound in the worst environment is assessed before average performance. Third, the paired same-random-sequence design separates effects of chance from effects of architecture. Fourth, preservation of both the local positive result for reserves and the negative result for memory rejects the two simplifications “greater complexity is stronger” and “greater simplicity is stronger.”

This engineering application's independent achievement is bringing minimal computation down from a philosophical slogan into a cost-inclusive structural-selection experiment. An intuition that a module is necessary is accepted only when the survival loss it reduces recovers its resource, computational, and communication costs. WRRA's cross-domain research question is whether the same principle recurs in embodied intelligence, consciousness, cells, and cosmology without conflating their different physical quantities.

## 71.9 Claim Boundary and Re-Entry Conditions

The present grade is EXPLORATORY COMPUTATIONAL SCIENCE / TOY-WORLD STRUCTURAL RESULT. DC flow omits frequency, voltage, reactive power, inertia, protection, repair, and recovery; resource coefficients are experimental assumptions; and the controllers are not industrial optimization algorithms. The result must not be read as having established optimal control for operating power grids.

Re-entry tests require: ① a sensitivity map over B and resource coefficients; ② a fine grid over compound stress 0.60–0.75; ③ preregistration of the action reinforced by a positive trace, failure-cause labels, learning rate, and forgetting rate; ④ parallel same-generation-capacity and cost-inclusive comparisons; ⑤ AC dynamics, frequency collapse, protection, repair, and recovery; and ⑥ unseen disturbance sequences and distribution shifts. These tests seek the boundary at which the present conclusion breaks, rather than adjusting WRRA to win after inspecting results.

Chapter conclusion WRRA-Grid does not designate either the most complex or simplest architecture as the winner in advance. G0, which sufficiently reads present information, was minimal in this environment; G2 showed the practical value of reserves at a compound boundary; and over-reserving and an immature memory policy failed because of their costs. Explaining these three results simultaneously in one ledger is the power-grid application's central achievement.

Part XIV WRRA Is an Interpreter: Informational Closure and the Boundary of Prediction
