# Normative Layer

## Admissible Action Constraints and Goal Selection Above Physical Execution

---

## Status

This document defines the **Normative Layer** of the stack.

It assumes:

* Execution Primitives (E1–E8)
* Structural Typing Discipline
* Control Layer
* Cognitive Layer
* Domain Instantiations

It does not redefine physics.
It does not override resource limits.
It does not eliminate irreversibility.

It specifies how:

* Goals,
* Prohibitions,
* Trade-offs,
* Value commitments,

become additional constraints on admissible trajectories.

Norms restrict what is permitted.
They do not change what is physically possible.

---

# 1. Position in Stack

Lower layers define:

* What is physically possible (Core).
* What is structurally coherent (Typing).
* How to regulate state (Control).
* How to search and commit (Cognition).

The Normative Layer defines:

> Which physically possible trajectories are declared admissible.

Norms operate by restricting the feasible set.

---

# 2. Formal Definition of Norm

Let:

$$
\Omega_H
$$

be the set of all physically possible trajectories over horizon $H$ that satisfy:

* Execution primitives (E1–E8)
* Resource constraints
* State constraints
* Control feasibility

A norm is a constraint function:

$$
N_j(\tau) \le 0
$$

where:

* $\tau \in \Omega_H$ is a trajectory
* $N_j$ evaluates admissibility

The norm-restricted admissible set:

$$
\Omega_H^N = { \tau \in \Omega_H \mid N_j(\tau) \le 0 \ \forall j }
$$

Norms shrink the admissible set.

They do not alter physics.

---

# 3. Norm Categories

Norms may constrain:

## 3.1 Outcome Constraints

Example:

* Harm ≤ threshold
* Inequality ≤ bound
* Risk ≤ tolerance

Form:

$$
g(x(t)) \le 0
$$

---

## 3.2 Action Constraints

Example:

* Prohibit deception
* Prohibit force except under $X$
* Require transparency

Form:

$$
a(t) \notin A_{prohibited}
$$

---

## 3.3 Resource Allocation Constraints

Example:

* Minimum redundancy required
* Savings floor required
* Health floor required

Form:

$$
r_i(t) \ge \sigma_i
$$

Where $\sigma_i$ may exceed collapse threshold $\tau_i$.

---

## 3.4 Procedural Constraints

Example:

* Require review before deployment
* Require consent before action
* Require majority approval

These constrain transition rules.

---

# 4. Two Directions of Constraint

There are two structurally distinct constraint directions.

---

## 4.1 Physics-Up Constraints (Non-Negotiable)

From Execution Primitives:

* Finite resources
* Irreversibility
* Drift
* Conservation
* Topology

These cannot be altered by normative choice.

---

## 4.2 Goal-Down Constraints (Chosen)

Norms introduce additional admissibility filters:

$$
\Omega_H \rightarrow \Omega_H^N
$$

These are selected.

They are not derived from physics.

---

# 5. Legitimacy

Legitimacy is defined as:

> Normative constraint acceptance by relevant loci in topology.

Let:

* $V \subseteq G$ be relevant nodes.
* Norm $N$ be declared.

Norm is legitimate relative to $V$ if:

1. Enforcement pathway exists in topology.
2. Load exposure is declared.
3. Authority over enforcement is specified.
4. Horizon scope is declared.

Legitimacy is topology-relative.

It is not moral truth.

---

# 6. Normative Closure

A norm becomes binding only when:

1. It crosses executability boundary.
2. It is embedded in contracts or enforcement structures.
3. Violation produces measurable consequence.
4. Load routing is declared.

Otherwise it remains narrative preference.

Narrative norms do not constrain trajectory.

Binding norms do.

---

# 7. Horizon Sensitivity

Norms are horizon-bound.

Let norm evaluate trajectory over horizon:

$$
H_N
$$

Short-horizon norms may conflict with long-horizon norms.

Example:

* Short-term comfort vs long-term health.
* Short-term profit vs long-term solvency.

Norms must declare evaluation horizon.

Norms without horizon are under-typed.

---

# 8. Trade-Off Surfaces

Norms define trade-off surfaces between metrics:

Examples:

* Safety vs efficiency
* Equity vs productivity
* Autonomy vs coordination
* Exploration vs stability

Let objective vector:

$$
M(\tau) = (m_1, m_2, ..., m_k)
$$

Norms restrict acceptable region in metric space.

Trade-offs cannot be eliminated.
They must be declared.

Hidden trade-offs produce invisible load.

---

# 9. Versioning

Norms drift under:

* Environmental change
* Institutional change
* Cultural evolution
* Technological development

Normative system at time $t$:

$$
N_t
$$

Versioning requires:

* Explicit declaration of revision.
* Migration cost acknowledgment.
* Horizon update.
* Enforcement transition plan.

Unversioned norms harden and become misaligned under drift.

---

# 10. Normative Failure Modes

---

## 10.1 Attempting to Override Physics

Example:

* “No one should need sleep.”

This violates E1.

Ill-typed.

---

## 10.2 Narrative-Only Norms

Declared but unenforced.

No enforcement topology.

Result: signaling without constraint.

---

## 10.3 Over-Constraining

Norms that:

* Remove redesign DOFs,
* Eliminate refusal symmetry,
* Exhaust resource margin,

May cause systemic instability.

Norms must remain compatible with execution primitives.

---

## 10.4 Under-Constraining

Failure to declare prohibitions leads to:

* Hidden coercion,
* Load asymmetry,
* Governance instability.

---

# 11. Norms and Power

Power is:

> Capacity to modify admissible set $\Omega_H^N$.

Norm-setting authority must:

* Bear load exposure,
* Be traceable in topology,
* Be revocable under declared process.

Norms that impose cost asymmetrically without load exposure destabilize governance.

---

# 12. Domain Examples

---

## 12.1 Robotics

Norms include:

* Safety invariants,
* Regulatory compliance,
* Redundancy requirements,
* Fail-safe policies.

These reduce performance envelope.

They increase system admissibility relative to regulatory topology.

---

## 12.2 Personal Domain

Norms may include:

* Health floor requirement,
* Financial reserve requirement,
* Truth constraint,
* Non-violence constraint.

These restrict reachable trajectories.

They increase friction.
They may reduce optionality.
They may increase long-horizon stability.

Norm selection is separate from physics.

---

# 13. Separation from Optimization

Optimization operates within:

$$
\Omega_H^N
$$

Norms define admissible region.
Optimization selects within that region.

Optimization cannot derive norms.
Norms cannot negate physics.

---

# 14. What This Layer Does Not Do

This layer does not:

* Claim moral universality.
* Guarantee fairness.
* Eliminate conflict.
* Override irreversibility.
* Define ultimate value.

It defines how chosen values become structural constraints.

---

# 15. Summary

The Normative Layer:

* Introduces admissibility constraints over physically possible trajectories.
* Restricts reachable state space.
* Defines trade-offs.
* Requires enforcement topology.
* Is horizon-bound.
* Must respect execution primitives.
* Can drift and require versioning.

Physics defines possibility.
Typing defines coherence.
Control enforces bounds.
Cognition selects paths.
Norms restrict admissibility.

Everything must remain type-consistent.

Norms are constraint functions.
They are not physical laws.
