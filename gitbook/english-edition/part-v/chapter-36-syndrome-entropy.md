# Chapter 36 Syndrome Entropy

Logical possibility of recovery does not make it free. If a syndrome bit is excited with probability p, the Shannon entropy processed in one cycle is −p ln p − (1−p)ln(1−p).

$$
ΔS_rec=−p ln p−(1−p)ln(1−p)
$$

_Equation (5.15)_

For the benchmark's p = 0.01, ΔS\_rec,N = 0.0560015 nat/step. This value is finite and independent of N. The bounded ledger results from fixing the syndrome factor as one qubit.

Applying the Landauer bound gives a minimum heat cost Q\_min = 0.0560015 k\_BT per step. This is not the heat output of an actual device or universe, but an ideal lower bound for irreversible erasure of the selected syndrome record.

$$
Q_min=k_BT ΔS_rec=0.0560015 k_BT at p=0.01
$$

_Equation (5.16)_

Calculating actual cost requires cycle time, bath temperature, coupling efficiency, error-production rate, and backreaction. Because these values are absent, a cosmological heat budget has not yet been obtained.

Bounded entropy and bounded total long-time cost are also different statements. If cost per cycle is positive, cumulative cost over infinitely many cycles continues to grow unless a resource supply and discharge path exist.

What the benchmark closes is therefore the syndrome-entropy ledger for one cycle. How long the universe performs this recovery and which reservoir it uses are questions for the next stage.

## **Related Research**

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)
