# Chapter 70 WRRA-Met 0.1–0.5: Prospective Testing of Tropical-Cyclone Track Residue

Conclusion of this chapter: DOI 10.5281/zenodo.22306663 is a frozen study using JMA western North Pacific best-track data to test whether current residue—the compressed effect of past trajectories—provides independent information for tropical-cyclone track prediction. The causal residue was recovered in synthetic systems, but the weak linear signal in real data was not unique relative to raw finite history and disappeared against a strong nonlinear current-state baseline. The final assessment is TRACK-ONLY RESIDUE NOT ESTABLISHED / ENVIRONMENTAL STATE REQUIRED.

## 70.1 Interpretation and Prediction Are Not the Same Task

When interpreting already formed DNA or material structure, the information to be analyzed exists in the present object. A tropical cyclone's next position, however, depends on steering flow, pressure fields, vertical wind shear, moisture, sea-surface temperature, ocean heat content, cold wakes, and land interactions that it has yet to encounter. The ability to read the meaning of present structure and the ability to predict a next present that is not yet closed cannot be judged by the same performance criterion.

Ynow=G(Xnow,Rnow), Xnext=F(Xnow,Rnow,Enow,ξnow)

X\_now is accessible present state, R\_now compressed residue remaining in the present, E\_now environmental state, and ξ\_now input unresolved by the model and observation. The present test intentionally excludes E\_now. Failure therefore means not that memory in general is absent, but that track history alone does not close the next state.

## 70.2 Data, State, and Causal Residue

The in-progress year 2026 was excluded from evaluation in the 1951–2026 JMA RSMC Tokyo best-track archive. A total of 154,144 samples for 6-, 12-, 24-, 48-, and 72-hour forecasts were constructed from 1,900 segments across 1,823 tropical cyclones, each sampled at exact six-hour intervals and having length at least fourteen. Data were split forward in time—training through 2014, validation from 2015 to 2019, and final testing from 2020 to 2025—with no cyclone segment crossing a split.

Present state I\_t included latitude, cyclic longitude, longitudinal and latitudinal velocity and acceleration, central pressure, maximum wind speed, intensity change, and seasonal terms. Residue of motion, acceleration, pressure, and wind-speed changes q\_t was updated by an exponential moving average without future values.

Rₜ⁽τ⁾=(1−ατ)Rₜ₋₁⁽τ⁾+ατqₜ, ατ=1−exp(−1/τ), τ∈{2,4,8}

The base τ values correspond to 12, 24, and 48 hours. This definition creates a finite state updated in the present without preserving a list of past times as separate coordinates. Being a computable compressed quantity alone does not, however, make it an independent physical state variable.

## 70.3 Comparison Models and Failure-First Validation

The study compared persistence P; linear current-state model M1; H1 with raw 6-, 12-, 24-, and 48-hour history; and W2 with EWMA residue. W2-S with residue shuffled within year and W2-L with 72-hour-lagged residue served as placebos, while nonlinear Extra Trees N1 current state, N2 raw history, and N3 residue were tested on the same targets and splits.

The tests became progressively stronger: 0.1 synthetic identifiability, 0.2 fixed future period, 0.3 forward reproduction across four eras, 0.4 nonlinear baseline, and 0.5 decay-time sensitivity. Uncertainty was calculated by 2,000 cluster-bootstrap resamples at the cyclone-segment level rather than treating time-point rows as independent samples.

## 70.4 The Synthetic System Passed the Detector

In fifteen cells of a synthetic system where residue was the true generative cause, 15/15 were positive, with mean improvement 10.744% (range 6.966–16.766%). In a generating system where residue was noncausal, the mean was effectively zero at −0.021% (range −0.127–0.044%), with only 4/15 positive. Negative real-data results therefore cannot be explained by an inability of the detector itself to find residue.

## 70.5 A Weak Linear Signal in Real Data

In the fixed 2020–2025 test, linear W2 slightly outperformed M1 only at 12, 24, and 48 hours and was worse at 6 and 72 hours. The 95% intervals for cyclone-segment-weighted improvement included zero at all five horizons. Raw-history H1 significantly outperformed W2 at 6 and 12 hours, while direct comparisons between W2 and shuffled residue were nonsignificant throughout.

Across four forward eras—2000–2005, 2006–2011, 2012–2017, and 2018–2025—W2 beat M1 in 18/20 cells, with median improvement 0.460%. It beat H1 in only 11/20. This is compatible with a recurring weak linear history signal, but does not support a unique advantage from residue compression.

## 70.6 The Decisive Boundary Created by a Nonlinear Baseline

Nonlinear current-state N1 produced approximately 1.98–5.66% lower error than linear M1 across horizons. Adding residue in N3 beat N1 at 0/5 horizons; cyclone-segment-weighted improvements were all negative, and the entire 95% interval lay below zero at 6, 24, and 48 hours. N3 also beat raw-history N2 at 0/5 horizons.

The most conservative interpretation is therefore that the small W2 gain in restricted linear models proxied nonlinear structure of the current state missed by the linear equation, rather than a new independent residue state. Across four decay families—6/12/24, 12/24/48, 18/36/72, and 24/48/96 hours—0/20 results were significantly positive.

## 70.7 Ownership of Failure and the Open Future

A tropical-cyclone center track is not a closed system. If slow traces of actual dynamics exist, their owner is more likely the coupled atmosphere–ocean environmental field than a compressed centerline record. This is not a fact established by the present result, but an OPEN HYPOTHESIS for WRRA-Met 0.6.

H(X\_future|X\_now^observed) > 0 ⇏ ontological indeterminism

Failure to recover one future path from a restricted observed present shows nonuniqueness of prediction, but is not metaphysical proof that the universe is intrinsically indeterministic. Sufficient missing initial conditions and environmental fields may increase predictability. WRRA must distinguish the existence of laws, informational completeness of the observed present, and predictability of future states.

## 70.8 Conditions for Resuming WRRA-Met 0.6

Resumption requires time-aligning multilayer winds, geopotential height, sea-level pressure, moisture, SST, and OHC from ERA5 or equivalent data and preregistering local, remote, and multiple-τ residue using only environmental fields available through the present. Nonlinear models with identical inputs, raw time series, the present environmental field, and available operational guidance must serve as strong baselines; time lags, cross-storm permutation, spatial rotation, and irrelevant remote fields must serve as placebos.

The study must use cyclone-level forward splits, probabilistic distributions and calibration, and one-shot external validation on an independent basin or subsequent season. The grade is raised only when cluster CI > 0 at several preregistered leads and the model simultaneously beats raw history and nonlinear baselines. Until then, track-only hyperparameter tuning is suspended.

The final grade is “0.1 identification of synthetic causal residue EMPIRICAL PASS / real-data linear history signal SUPPORTED BUT NOT ESTABLISHED / uniqueness of residue relative to raw history NOT ESTABLISHED / residue relative to nonlinear current state REJECTED HERE / improvement of tropical-cyclone track prediction NOT ESTABLISHED / environmental-field residue and ontological indeterminism OPEN.”

Chapter conclusion The achievement of WRRA-Met 0.1–0.5 does not lie in creating a new tropical-cyclone forecaster. It separates information that can interpret the present from information required for a future transition, downgrades a claim when a weak gain disappears against a stronger baseline, and moves the research boundary from a failed variable to the next candidate owner of information. As a complex-systems analysis tool, WRRA should be not a model that prophesies the future, but a methodology auditing ownership of information actually remaining in the present and conditions under which the next state closes.

**Part XIII WRRA Extended to Engineering Complex Systems: Power Grids and Resource Scarcity**
