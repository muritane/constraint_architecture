# Minimal Constraint Core  
## A Static Typing Discipline for Execution in Bounded Systems

---

## Status

This document defines a **minimal, non-negotiable constraint core** for reasoning about
action, agency, evaluation, responsibility, and coordination in systems that **execute under load**.

It is **not**:
- a moral framework,
- a theory of value,
- a model of behavior,
- or a prescription for action.

It is a **static checker**:  
it determines when claims about action are **well-formed** with respect to executional reality.

The core is **closed**.  
Nothing here is optional.  
Nothing here is ornamental.

---

## 0. Scope Declaration (Global)

This core applies **if and only if** all of the following hold:

- Action produces real state transitions (not pure interpretation)
- Resources are finite
- Time is irreversible
- Effects propagate beyond the acting locus
- Persistence across time matters

If any of these are false, the system is **out of scope**.

---

## 1. Foundational Execution Constraints (Physics-Level)

These constraints are **non-negotiable**.
No goal, intelligence, coordination mechanism, or value system can remove them.

---

### C1 — Bounded Resources

Time, energy, attention, computation, material capacity, and coordination bandwidth are finite.

> Any claim requiring infinite context, infinite patience, or unbounded negotiation is ill-typed.

---

### C2 — Partial Observability

No executor has complete access to the state variables governing outcomes.

> Claims assuming full information are ill-typed under execution.

---

### C3 — Irreversibility

Execution induces state transitions that cannot, in general, be undone.

> Rollback is itself costly execution, not a default property.

---

### C4 — Irreversible Abstraction

Execution requires **lossy abstraction** in two distinct but related senses:

- **Representational loss**  
  Representations cannot preserve all distinctions present in the world.

- **Actuation loss**  
  Action selection collapses multiple possible world states into a single executed transition.

These losses may coincide or diverge depending on system design,  
but **at least one** must occur for execution to be possible.

> Lossless execution under bounded resources is impossible.

---

### C5 — Drift / Non-Stationarity

Causal structure changes over time.

> All invariants are horizon-bounded and regime-dependent.

---

## 2. Horizon Boundedness (Explicit Primitive)

### H — Horizon Constraint

All execution, evaluation, optimization, and responsibility claims are defined **only relative to a declared or inferable temporal horizon**.

- Horizons may be implicit, but must be recoverable.
- Claims that shift horizons without revalidation are ill-typed.
- Validity does not persist beyond its horizon by default.

> Horizon-independent claims are under-specified for execution.

---

## 3. Topological Distinction (Explicit Primitive)

### T — Topology Constraint

Execution implies at least one **distinguishable locus** where state transitions occur and where disturbance can accumulate.

- Representation, execution, and affected state may be colocated, but **must be distinguishable**.
- Disturbance must be able to land somewhere.
- Fully collapsed systems must explicitly declare internal separation or forfeit responsibility typing.

> Without topology, load, power, and responsibility collapse into metaphor.

---

## 4. Executability Boundary

A strict boundary exists between **interpretation** and **execution**.

- **Above the boundary**  
  meaning, intent, narrative, justification

- **At the boundary**  
  invocation, defaults, omission, interface crossing

- **Below the boundary**  
  invariants, buffers, latency, failure semantics, load propagation

> Interpretation does not execute.  
> Execution is indifferent to intent.

Any claim that crosses this boundary without specifying how is **ill-typed**.

---

## 5. Viability Precedence

### C6 — Viability Gate

Optimization, improvement, or evaluation claims are meaningful **only if continued execution remains possible over the stated horizon**.

> Optimization without a viability witness is undefined, not wrong.

---

## 6. Closure and Degrees of Freedom

### C7 — Closure Requirement

Executable systems must terminate interpretation by fixing an **exact partition of degrees of freedom** at entry.

For any task, DOFs must be classified as:

- **Essential** — fixed at entry
- **Optional** — delegated within bounds
- **Latent** — preserved for versioning or redesign
- **Irrelevant** — explicitly collapsed
- **Unknown** — excluded from load-bearing execution

> Systems that do not declare this partition do not support agency-grade participation.

---

## 7. Decidability and Agency

### C8 — Decidable Boundary

Agency exists **only** at a pre-execution boundary where:

- Accept and refuse are both executable
- Refusal has bounded, declared consequences
- Constraints are explicit before entry

> If refusal exists only narratively, agency attribution is ill-typed.

Inside execution, only discretion exists — not agency.

---

## 8. Load and Responsibility

### C9 — Load Location

Disturbance introduced by execution must land somewhere in the system topology.

> Invisible load routing produces unstable responsibility claims.

---

### C10 — Responsibility Typing

Responsibility is typeable **only if**:

- Entry into execution was decidable
- Relevant degrees of freedom were declared
- Outcomes depended on controllable variables
- Failure semantics were explicit
- Load routing is legible within the topology

> Responsibility follows load, not involvement, intent, or narrative presence.

---

## 9. Metrics and Evaluation

### C11 — Executable Metrics

A metric is valid only if it:

- Is substitutable across evaluators
- Is computable under bounded resources
- Yields determinate outcomes
- **Fails explicitly** outside its validity envelope

> Metrics that never fail accumulate hidden error and are ill-typed as coordination interfaces.

---

## 10. Meaning for Coordination

### C12 — Shared Meaning Constraint

Meaning becomes real-for-coordination **only when it is**:

- Externally addressable
- Substitutable across agents
- Admitted into a protocol
- Subject to failure with attributable cost

> Meaning that cannot fail cannot coordinate.

---

### C13 — Narrative Acceptance (Non-Binding Regime)

Narrative, interpretation, and expectation coordinate **only while acceptance holds**.

They impose:
- no invariants
- no failure semantics
- no irreversible cost

> Narrative acceptance is pre-execution only and collapses under load.

---

## 11. Redesign Safety

### C14 — Redesign Possibility

For redesign to remain possible, systems must preserve or allow recovery of:

- horizon specification
- execution vs interpretation distinction
- irreversibility awareness
- interruptible or refusal points
- load traceability

> Abstractions that erase their own invalidation conditions are redesign-unsafe.

---

## 12. Power (Descriptive)

### C15 — Power Definition

Power is the capacity to **reassign disturbance and buffer ownership across nodes and horizons**.

> No execution eliminates cost.  
> It only displaces it.

---

## 13. Typing Outcomes

Any claim about action, evaluation, agency, or responsibility is exactly one of:

- **Well-Typed** — coherent under all declared constraints
- **Under-Typed** — missing required primitives or witnesses
- **Ill-Typed** — violates executional constraints

This is a **three-valued system by necessity**.

---

## End of Core

This document defines the **minimal constraint set** required for execution-coherent reasoning.

- Removing any constraint produces invisible load or false agency.
- Adding constraints at this level produces premature over-specification.
- All domain-specific rules belong **above** this core, never inside it.

This core does not tell you what to do.

It tells you when what you are saying  
**could possibly be true** for a bounded executor.
