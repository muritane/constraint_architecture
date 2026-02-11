# Execution Primitives

## Measurable Ontology for Bounded Physical Systems

---

## Status

This document defines the **minimal physical and informational constraints** required for reasoning about execution in real systems.

It contains:

* No goals
* No norms
* No agency claims
* No responsibility claims
* No optimization criteria
* No governance rules

It specifies only what must be physically and informationally true for execution to exist in bounded systems.

Higher layers derive their typing rules and constraints from these primitives.

If any primitive here is invalidated by physical law, the entire stack must be reconsidered.

---

# 0. Scope

This ontology applies if and only if:

1. State transitions occur in physical time.
2. Resources are finite and measurable.
3. State evolution is not freely reversible.
4. Effects propagate across structured systems.
5. Observation channels are capacity-limited.

Purely symbolic, timeless, or consequence-free systems are out of scope.

---

# Core Execution Primitives (E1–E8)

Each primitive is stated in physically measurable terms.

---

# E1 — Finite Resource Vectors

For every execution locus ( L ), there exists a finite resource vector:

[
R_L = (r_1, r_2, ..., r_n)
]

where each component has measurable physical units, such as:

* Time (seconds, s)
* Energy (joules, J)
* Power (watts, W)
* Mass (kg)
* Memory (bytes)
* Computation rate (FLOPs/s)
* Bandwidth (bits/s)
* Currency (unit-defined)
* Thermal capacity (J/K)

For all execution trajectories over horizon ( H ):

[
r_i(t) < \infty
]

No executor has infinite slack in any resource dimension.

---

# E2 — Information Capacity Limits (Partial Observability)

Let:

* ( C ) = channel capacity (bits/s)
* ( N ) = noise power
* ( H(X) ) = entropy of system state

Then:

[
\text{Information acquired per unit time} \le C
]

All state estimation is bounded by:

* Finite sampling rate (Hz)
* Finite bandwidth (bits/s)
* Signal-to-noise ratio (SNR)
* Latency (seconds)

No executor can access complete state information of a nontrivial environment.

Observability is capacity-limited and noise-corrupted.

---

# E3 — Physical Irreversibility

For any nontrivial state transition:

[
\Delta S \ge 0
]

where ( S ) is entropy.

Irreversible processes dissipate energy:

[
E_{diss} > 0
]

Information erasure incurs minimum thermodynamic cost:

[
E_{min} = kT \ln 2 \quad \text{per bit}
]

(Landauer bound)

Perfect rollback requires additional energy expenditure and cannot restore prior microstate symmetry.

Execution reduces reachable microstate set unless compensated by work.

---

# E4 — Lossy Representation and Actuation

Execution requires compression.

## E4a — Representational Compression

Let:

* ( \Omega ) = full state space
* ( \hat{\Omega} ) = represented state space

Then:

[
|\hat{\Omega}| \le |\Omega|
]

Representation reduces distinguishable states.

Compression can be characterized via:

* Kolmogorov complexity
* Rate-distortion tradeoff
* Information loss (bits)

Lossless full representation of nontrivial systems is infeasible under finite resources.

---

## E4b — Actuation Collapse

Let:

* ( A ) = available action space
* ( a_t \in A ) = executed action at time t

Execution selects a single trajectory branch:

[
\text{Reachable}_{t+1} \subseteq \text{Reachable}_t
]

Branching alternatives collapse irreversibly.

Actuation reduces reachable future volume.

---

# E5 — Drift / Non-Stationarity

Let system parameters be ( \theta(t) ).

Drift is defined as:

[
\frac{d\theta}{dt} \neq 0
]

Drift magnitude over horizon ( H ):

[
D(H) = \int_0^H \left| \frac{d\theta}{dt} \right| dt
]

No nontrivial real-world system has globally stationary causal structure.

All invariants are regime-bound and horizon-bound.

---

# E6 — Horizon Boundedness

All evaluation and execution occur over a finite horizon:

[
H \in (0, \infty)
]

Horizon may be measured in:

* Seconds
* Cycles
* Episodes
* Project duration
* Operational lifespan

Claims without declared or inferable horizon are incomplete for execution analysis.

No infinite-horizon evaluation is physically realizable under E1–E5.

---

# E7 — Structured Topology

Execution occurs in structured systems representable as graphs:

[
G = (V, E)
]

where:

* ( V ) = loci (nodes)
* ( E ) = interaction edges

Edges may represent:

* Energy transfer
* Information transfer
* Material flow
* Authority pathways
* Economic obligation

Load accumulation at node ( v ):

[
\Delta L_v = \sum_{in} f_e - \sum_{out} f_e
]

Disturbance must propagate through edges.

Without topology:

* No load routing
* No cost localization
* No disturbance accumulation

Execution implies structured coupling.

---

# E8 — Conservation and Consequence Propagation

For any state transition:

Energy, momentum, and conserved quantities obey:

[
\sum_{in} = \sum_{out} + \text{dissipation}
]

Disturbance introduced at node ( v ) propagates via:

* Network flow
* Coupling coefficients
* Latency
* Buffer capacity

Disturbance may:

* Dissipate
* Transform domains
* Redistribute
* Accumulate
* Amplify
* Attenuate

But cannot vanish without compensating process.

Consequence propagation is governed by:

* Topology (E7)
* Resource constraints (E1)
* Information limits (E2)
* Irreversibility (E3)
* Drift (E5)

No executed action is consequence-free.

---

# Non-Primitives (Removed From Core)

The following are NOT execution primitives:

* Viability
* Agency
* Responsibility
* Metrics
* Optimization
* Legitimacy
* Governance
* Meaning
* Norms

These are higher-layer constructs derived from E1–E8.

---

# Minimality Claim

The set {E1–E8} is minimal in the following sense:

* Removing E1 permits infinite slack models incompatible with physics.
* Removing E2 permits omniscience inconsistent with channel limits.
* Removing E3 permits costless reversal.
* Removing E4 permits lossless full representation under finite resources.
* Removing E5 permits global stationarity.
* Removing E6 permits horizon-free evaluation.
* Removing E7 eliminates load localization.
* Removing E8 permits consequence-free execution.

Each primitive corresponds to measurable physical or informational constraints.

---

# Derived Concepts (Not Primitive)

Concepts such as:

* Collapse
* Stability
* Viability
* Survival
* Robustness

are trajectory predicates defined over:

* Resource vectors (E1)
* Drift magnitude (E5)
* Topology (E7)
* Horizon (E6)

They are not ontological axioms.

---

# Summary

Execution in bounded physical systems requires:

1. Finite measurable resource vectors.
2. Information acquisition limits.
3. Thermodynamic irreversibility.
4. Lossy representation and branch collapse.
5. Parameter drift.
6. Finite evaluation horizon.
7. Structured topology.
8. Conservation-governed consequence propagation.

Everything else in the stack must reduce to these measurable constraints.

Nothing below this layer.

Everything above it must type-check against it.
