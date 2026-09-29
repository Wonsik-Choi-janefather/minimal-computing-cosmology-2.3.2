# E-13 External Sensorimotor Application: WRRA-Worm

## 95. Fixed-present neural state

$$
x(k)=[v₁…v_N, a₁…a_N, q₁…q_N, E]ₖ
$$

Meaning Calculates the next state using only current activity, adaptation, resources, and the environmental reservoir.\
Grade MODEL STATE DEFINITION\
Basis 10.5281/zenodo.22298363

## 96. Chemical and electrical relation terms

$$
c(k)=W[v(k)]₊, gᵢ(k)=ΣⱼGᵢⱼ[vⱼ(k)-vᵢ(k)]
$$

Meaning Separates directed signed chemical synapses from symmetric gap-junction diffusion.\
Grade STANDARD-FORM TOY DYNAMICS\
Basis 10.5281/zenodo.22298363

## 97. Fixed-present activity update

$$
v(k+1)=tanh{0.72v(k)+q(k)⊙[c(k)+g(k)+0.85u(k)-0.62a(k)]}
$$

Meaning Combines leak, current resources, relations, input, and adaptation into a bounded next state.\
Grade DECLARED TOY UPDATE\
Basis 10.5281/zenodo.22298363

## 98. Adaptation-state update

$$
a(k+1)=clip[0.94a(k)+0.06|v(k+1)|,0,1]
$$

Meaning Leaves residue of current activity in a finite adaptation variable.\
Grade DECLARED TOY UPDATE\
Basis 10.5281/zenodo.22298363

## 99. Conservation of computational resources

$$
B(k)=Σᵢqᵢ(k)+E(k)=constant
$$

Meaning Conserves movement of computational resources between activity and recovery. It is not a direct identification with ATP or physical energy.\
Grade EXACT UNDER IMPLEMENTED LEDGER\
Basis 10.5281/zenodo.22298363

## 100. Same-present restart condition

$$
x₁(k)=x₂(k), u₁(k)=u₂(k) ⇒ F[x₁(k),u₁(k)]=F[x₂(k),u₂(k)]
$$

Meaning Tests whether the same serialized present and input produce the same next state.\
Grade EXACT FOR DETERMINISTIC IMPLEMENTATION\
Basis 10.5281/zenodo.22298363

## 101. Closed body–environment loop

$$
environment(k)→sensory u(k)→neural x(k+1)→muscle m(k+1)→body/environment(k+1)
$$

Meaning To judge neural readout as actual behavior requires feedback through muscles, the body, and the environment.\
Grade REQUIRED VALIDATION ARCHITECTURE / OPEN\
Basis 10.5281/zenodo.22298363
