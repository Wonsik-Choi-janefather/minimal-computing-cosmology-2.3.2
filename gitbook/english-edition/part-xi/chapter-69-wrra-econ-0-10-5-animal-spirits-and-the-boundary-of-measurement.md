# Chapter 69 WRRA-Econ 0.1–0.5: Animal Spirits and the Boundary of Measurement

Conclusion of this chapter: DOI 10.5281/zenodo.22305789 is a frozen report that expresses confidence, fear, trust, debt, credit conditions, and institutional memory as candidate slow residue in the fixed present, then tests them in stages from a toy ledger to actual U.S. macroeconomic data. In the synthetic generating system, E2 was selected under new seeds when residue was a true cause, but universal predictive improvement was not statistically established in real data. Crisis-memory intervals showed a more favorable directional signal than calm periods, but current sentiment did not beat a 36-month-lag placebo. The final assessment is PARTIAL SIGNAL / MEASUREMENT OPEN.

## 69.1 Present Economic State and Animal Spirits

In this chapter, animal spirits do not reduce the economy to a single emotion. They form a state-space hypothesis asking whether fear, trust, optimism, debt, and risk-management practices remaining from earlier shocks can alter subsequent consumption, investment, hiring, and lending even when fast observed states such as production, employment, and credit are the same. Rather than rereading the past on a separate axis, the model assumes that a sufficient state h remaining physically and institutionally in the present acts on the next present.

Sₜ=(xₜ,hₜ,rₜ,zₜ,cₜ), Sₜ₊₁=F(Sₜ,uₜ)

x is fast observed state, h slow residue, r resources and constraints, z the net financial positions of households, firms, banks, government, and central bank, and c a crisis regime. SOURCE includes private-sector, government, and central-bank sources and demand, financial, policy, supply, and narrative shocks; RELATION includes consumption, investment, credit, wage, tax, and interest-rate couplings; BOUNDARY includes liquidity, capital, productive capacity, and crisis thresholds.

hₜ₊₁=Dhₜ+(I−D)ψ(xₜ₊₁,uₜ,cₜ), Σⱼzⱼₜ=0

A sum of financial positions equal to zero is a ledger for declared intersectoral accounting transfers. It is not identified with conservation of real resources, output, utility, currency value, or thermodynamic energy. Central-bank balance sheets and government debt likewise do not disappear outside the model; they must be assigned to specified sectors and boundary transactions.

## 69.2 Version 0.1: Structural Execution and Same-Present Restart

Version 0.1 executed a dimensionless toy economy with a boom, first financial shock, policy support, recovery, and second shock. Maximum sector-accounting error was 5.329 × 10⁻¹⁵ and same-present restart error was zero. In restarts matching fast state but differing only in residue, residue distance was 0.4549, and after the second shock the output trough was 0.5800 with residue carried versus 0.4827 when neutral, a 20.16% difference.

This effect is a designed structural test within equations that include residue as a cause. It is not data-based evidence that the actual economy possesses shock memory of the same magnitude. The grade of version 0.1 is ACCOUNTING·RESTART·REGIME STRUCTURAL PASS.

## 69.3 Versions 0.2–0.3: Competing Models and New-Seed Reproduction

Linear Markov E0, nonlinear Markov E1, and residue-augmented E2 competed on identical data, splits, and evaluation windows. In the positive generator, h causally acted on x; in the negative generator, h was recorded but did not act on x. The initial specification recursively predicted levels and accumulated long-horizon errors, so every model was changed to a common increment target. Because this revision followed inspection of test behavior, version 0.2 remains development validation only.

Δxₜ₊₁=G₀(xₜ,uₜ)+εₜ \[E0], Δxₜ₊₁=G₁(φ₂(xₜ,uₜ))+εₜ \[E1]

hₜ₊₁=Dhₜ+(I−D)ψₜ₊₁, Δxₜ₊₁=G₂(xₜ,uₜ,hₜ)+εₜ \[E2]

In version 0.2's causal-residue generator, the best Markov RMSE was 0.01551 and E2 was 0.00687, a relative effect of +55.72%. In the noncausal generator, best Markov was 0.00684 and E2 was 0.00838, an effect of −22.66%. After freezing the specification, version 0.3 applied it to five new random-seed blocks and 180 independent test trajectories, reproducing the expected direction in 5/5 causal and 5/5 negative-control blocks. Mean causal improvement was 49.88% (block range 40.10%–59.65%); mean noncausal change was −14.21%.

This result shows that the selector can identify residue in a synthetic world where it is the true generative cause and penalize E2 where residue is noncausal. Identifiability and new-seed reproduction on synthetic data constitute a VALIDATED SYNTHETIC PIPELINE, not validation of the real economy.

## 69.4 Version 0.4: External Audit on Monthly U.S. Macroeconomic Data

Fast state comprised industrial production, nonfarm employment, real retail sales, housing starts, unemployment, the policy rate, prices, and the Baa–Treasury spread. Residue proxies were the level and three-month change of Michigan Consumer Sentiment and a causal twelve-month EWMA of sentiment innovation. Targets were one-, three-, six-, and twelve-month-ahead changes in industrial production, employment, real retail sales, and unemployment. Training ended in 2006, model selection used 2007–2014, and testing began in 2015.

Because higher-order polynomial models extrapolated unstably, particularly during the pandemic shock, the core comparison was restricted to linear E0 and linear E2, which used the same information plus only three sentiment coordinates. Overall test gains were +0.25%, +0.78%, +1.74%, and +3.58% at one, three, six, and twelve months, but the respective 95% CIs \[−0.82,+1.08], \[−3.00,+1.83], \[−6.21,+3.23], and \[−9.39,+6.33] all included zero.

Before March 2020, E2 performed slightly worse at all four horizons, from −0.18% to −0.48%; afterward, it improved at every horizon, from +0.26% to +5.66%. Consistent point estimates cannot replace uncertainty, so universal improvement on real data is NOT ESTABLISHED.

## 69.5 Version 0.5: A Partial Signal in the Crisis-Memory Regime

Official recession months and the following 24 months were designated the crisis-memory regime, and monthly expanding-window forecasts were produced from 2000 onward. Ridge regularization was selected annually using only the preceding eligible 36 months. E0 and E2 are linear, use identical splits and complexity, and differ only by E2's three added sentiment-residue coordinates.

Across 100 crisis-memory months, E2 improvements at one, three, six, and twelve months were +0.006%, +0.751%, +1.119%, and +4.664%. In the calm regime, all four horizons worsened: −0.635%, −0.739%, −2.789%, and −7.057%. Eight of twelve episode×horizon cells favored E2, but there were only three independent recession episodes—2001, 2007–2009, and 2020—and only the three-month horizon excluded zero under episode-cluster bootstrap.

Using recession months alone made three of four horizons positive; including the subsequent 6, 12, 18, or 24 months made all four positive, but extending through 36 months left only one. This is compatible with finite crisis memory, but because it is a sensitivity analysis varying windows within the same sample, it is not interpreted as independent confirmation or a universal 24-month constant.

## 69.6 The 36-Month-Lag Placebo and Final Downgrade

The same expanding-window procedure was applied to stale E2, moving the three current-sentiment coordinates 36 months into the past. Current E2 beat lagged E2 in only four of sixteen cells, all at the twelve-month horizon. At one, three, and six months, old sentiment performed better. The gain in crisis intervals therefore cannot be uniquely attributed to current sentiment residue.

Lagged sentiment may measure actual 36-month economic memory, but it may instead fortuitously proxy an omitted structural variable, event, or sample composition. The present data cannot distinguish the two explanations. The study is therefore frozen not as a “discovery of 36-month memory,” but with the crisis–calm directional contrast as PARTIAL SIGNAL and the measurement and temporal alignment of residue as OPEN.

## 69.7 Data Quality and Claim Boundary

The central limitation is construct mismatch. WRRA residue may be structural memory distributed across debt, credit supply, risk-management practices, lags in hiring and investment, asset losses, and institutional trust, but the primary proxy was one consumer survey. There are few independent crises, the 2020 event dominates error, and presently revised FRED series differ from the real-time vintages seen by forecasters then. Three-, six-, and twelve-month target errors also overlap, reducing the effective independent sample.

This chapter therefore does not claim that WRRA predicted the economy, proved animal spirits, or discovered 36-month memory. The economic application is not physical evidence for Minimal Computation Cosmology and is a separate domain from the biological applications. What it strengthens is a procedure for analyzing complex systems: decomposing states, relations, boundaries, ledgers, and slow candidates, then freezing failures through strong baselines, negative controls, fresh-seed replication, and temporal placebos.

## 69.8 Conditions for Resuming WRRA-Econ 0.6

The next residue candidate must be separated into multiple dimensions, H\_t = (H\_sentiment,H\_debt,H\_credit,H\_employment,H\_institution), with distinct decay times preregistered. Rather than further fitting the same U.S. sample, the work requires a non-U.S. country or multicountry panel, real-time data vintages and actual release lags, household and corporate debt, lending standards, credit spreads, canceled investment, employment persistence, and institutional trust.

Observed variables, complexity, splits, and tuning budgets must remain identical across E0/E1/E2, which must pass lagged placebos and negative controls together. The grade is not raised until episode-level consistency, cluster uncertainty, and calm-regime negative controls close simultaneously in out-of-event validation on new events.

The re-entry gate is NEW DATA + PREREGISTERED MULTIDIMENSIONAL RESIDUE + TEMPORAL PLACEBO + OUT-OF-EVENT VALIDATION. WRRA-Econ 0.1–0.5 remains frozen until all four conditions are ready.

The final grade is “0.1 accounting, restart, and regime STRUCTURAL PASS / 0.3 synthetic-residue identification on new seeds REPLICATED / 0.4 universal real-data prediction NOT ESTABLISHED / 0.5 crisis–calm directional contrast PARTIAL SIGNAL / temporal specificity of current sentiment and measurement of structural residue MEASUREMENT OPEN.”

Chapter conclusion WRRA-Econ 0.1–0.5 is not a theory proving shock memory in the economy, but a freeze report preserving what was computable and where the data blocked identification. The failure of current sentiment to beat a temporal placebo is precisely the starting point of the next study. If WRRA is a complex-systems analysis tool, its value is clearer in exposing such measurement boundaries and freezing re-entry conditions than in a successful fit alone.

Part XII WRRA Extended to Natural Complex Systems: Meteorology and the Boundary of Prediction
