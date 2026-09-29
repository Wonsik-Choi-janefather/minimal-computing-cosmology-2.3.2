# Chapter 25 Designing Independent Predictions

> **WRRA methodological position.** Independent prediction is not a prerequisite for theory status or originality. This chapter defines an optional, stricter validation protocol. Calibration with verified constants and observations is legitimate; WRRA originality is assessed through its own structures, transformations, connections, and explanations. After a calibrated model is frozen, an unmeasured quantity produced through a WRRA-specific transformation counts as a WRRA prediction.

Independent prediction cannot be declared after a calculation is finished. The calibration set C, validation set V, and final test set T must first be separated, and values in T must remain unused until the model and analysis rules are frozen. This is a minimum discipline shared by machine-learning evaluation and blind analysis in physics.

$$
D = C ⊔ V ⊔ T
$$

_Equation (4.9)_

The prediction map is then fixed. It specifies which LAW and SOURCE inputs pass through which renderer to read which observable, together with the renormalization scale, unit conversions, and allowed error. If many intermediate branches can be selected, the branch itself is a free parameter.

A small ratio is more appropriate than a grand target for WRRA's first blind test. Candidates include a mass ratio, coupling-constant ratio, residue ratio, or pole spacing in a restricted energy window for which an already calibrated absolute unit cancels.

A prediction need not be a point value. An interval prediction separating theoretical and numerical errors is also legitimate. Widening the interval or changing the observable after observation, however, is not a prospective prediction. Failed predictions must remain preserved together with their version DOI.

$$
O_pred = μ_model ± (σ_theory ⊕ σ_numeric)
$$

_Equation (4.10)_

If different runtimes reproduce the same low-energy observable algebra, shared predictions can be separated from implementation-specific ones. A result common to every runtime tests the WRRA architecture, while a result appearing in only one runtime tests that microscopic implementation.

Once this procedure is established, the research objective also changes. Rather than fitting more constants simultaneously, the next advance is to calculate one sealed value from few inputs and assign the cause of failure to the correct layer.

## From a Failed Common Dipole to a Frozen Neutron Current

The neutron magnetic-form-factor study is a case in which this procedure was applied to actual observational data. A common dipole model fixed by the proton magnetic radius passed a static-radius comparison but failed on ten finite-momentum-transfer points published in 2024, with χ² ≈ 61.7. What closed here was not the entire common static geometry, but the claim that “the same uncorrected dipole executes the finite-momentum neutron current as well.”

The missing layer was localized to current dressing, and the following transition factor was tested.

T(Q²)=1+a·Q²/(Q²+λ\_π)+b·Q²/(Q²+λ\_m), λ\_π=4m\_π² (4.18)

After fitting two parameters to the first five points, the proximity of λ\_m ≈ 0.14885 GeV² to (m\_ρ/2)² = 0.150257 GeV² was recognized post hoc. The ρ-half scale is therefore post hoc compression, not an independent prediction. Fixing both scales and determining a from the neutron-radius constraint leaves only one continuously calibrated quantity, b = 0.487160.

The frozen model achieved χ² = 2.751 (0.550 per point) on the untouched upper five points, and all ten points fell within the combined quoted 1σ uncertainty in leave-one-out refitting (max|z| = 0.953). This is stronger than a simple visual fit over the full range, but it remains a retrospective ordered holdout within the same dataset. It cannot be promoted to an externally independent prediction until λ\_π, λ\_m, a, and b are applied without change to another experiment or to a newly preregistered Q² interval.

Frozen card: λ\_π = 0.077919575 GeV², λ\_m = 0.150257017 GeV², b = 0.4871600738, a = −0.2600650101. For the next dataset, the residual vector, covariance, χ², and every difference in observable definitions will be disclosed, with no retuning.

Claim grades: the uncorrected common dipole is REJECTED; the one-amplitude runtime is INTERNAL ORDERED-HOLDOUT PASS; the ρ-half interpretation is POST-HOC COMPRESSION; and transfer to another experiment and derivation of the neutron current from fixed LAW and renderer remain OPEN.

## **Related Open Studies**

**A Tuned Model of Our Universe Based on the Dimensional Filter** [10.5281/zenodo.22051682](https://doi.org/10.5281/zenodo.22051682)
