# Structural Typing Discipline  
## A Static Checker for Claims About Execution in Bounded Systems

---

## Status

This document defines the **structural typing layer** built on top of the Execution Primitives.

It does not introduce new physics.
It does not introduce values.
It does not prescribe behavior.

It specifies when claims about:

- action,
- optimization,
- agency,
- responsibility,
- evaluation,
- meaning,
- coordination,
- governance,

are **well-formed** with respect to bounded execution under drift.

If `0_core/execution_primitives.md` defines what must be true for systems to run,  
this document defines what must be true for statements about those systems to be coherent.

---

## Dependency

This layer assumes all primitives from:

> `0_core/execution_primitives.md`

If any execution primitive is invalidated,  
all typing guarantees in this document must be re-evaluated.

---

# 1. Typing Environment

All execution-relevant claims must be typed relative to an explicit or inferable environment:

- **E** — Observation set and measurement quality  
- **T̂** — Provisional consequence topology model  
- **H** — Declared or inferable horizon  
- **R** — Resource bounds and remaining margins  

Claims that do not specify or imply `(E, T̂, H, R)` are **under-typed**.

Under-typed does not mean false.
It means structurally incomplete for execution reasoning.

---

# 2. Executability Boundary

A strict boundary exists between:

### Interpretation (Non-Binding)
- meaning
- intent
- justification
- narrative
- value declaration

### Execution (Binding)
- invocation
- interface crossing
- default triggering
- state transition
- constraint engagement
- resource consumption
- load propagation

Interpretation does not execute.

Any claim that moves from interpretation to execution without specifying the crossing is **ill-typed**.

---

# 3. Viability Gate

Optimization, improvement, or evaluation claims are meaningful only if:

- continued execution remains possible over the declared horizon.

If viability is failing or undefined:

- optimization claims are **undefined**, not wrong.

> Viability precedes optimization.

---

# 4. Closure and Degree-of-Freedom Partition

Executable participation requires closure.

For any load-bearing task, degrees of freedom must be partitioned into:

- **Essential** — fixed at entry
- **Optional** — delegated within declared bounds
- **Latent** — preserved for redesign or regime shift
- **Irrelevant** — explicitly collapsed
- **Unknown** — excluded from load-bearing execution

Systems that do not declare this partition cannot support agency-grade participation.

Undeclared degrees of freedom create invisible constraint surfaces.

---

# 5. Decidable Boundary (Agency Typing)

Agency is typeable only at a pre-execution boundary where:

- acceptance and refusal are both executable,
- refusal has bounded and declared consequences,
- constraints are explicit prior to entry.

If refusal exists only narratively,  
agency attribution is ill-typed.

Inside execution, only discretion exists — not agency.

---

# 6. Responsibility Typing

Responsibility is structurally coherent only when:

- entry into execution was decidable,
- relevant degrees of freedom were declared,
- outcomes depended on controllable variables,
- failure semantics were explicit,
- load routing is legible in topology.

Responsibility follows load location, not:

- intent,
- moral narrative,
- proximity,
- status,
- or rhetorical involvement.

Absent load traceability, responsibility claims are under-typed.

---

# 7. Metric Validity

A metric is valid as a coordination interface only if it:

- is substitutable across evaluators,
- is computable within resource bounds,
- yields determinate outcomes under a protocol,
- **fails explicitly** outside its envelope.

Metrics that never fail accumulate hidden drift and are ill-typed as coordination artifacts.

Implicit reinterpretation of metric failure is structural decay.

---

# 8. Meaning for Coordination

Meaning becomes structurally binding only when it is:

- externally addressable,
- substitutable across agents,
- admitted into a protocol,
- subject to attributable failure cost.

Meaning that cannot fail cannot coordinate.

Internal meaning remains real for the agent  
but is not system-binding.

---

# 9. Narrative Regime (Non-Binding Coordination)

Narrative and interpretation coordinate only while acceptance holds.

Narrative imposes:

- no enforced invariants,
- no structural failure semantics,
- no irreversible cost.

Narrative regimes are valid in exploratory contexts.

They collapse under load-bearing execution.

Confusing narrative acceptance with executional constraint is ill-typed.

---

# 10. Redesign Safety

Systems remain redesign-safe only if they preserve or allow recovery of:

- horizon specification,
- execution vs interpretation distinction,
- irreversibility awareness,
- interruptible boundaries,
- load traceability.

Abstractions that erase their own invalidation conditions are redesign-unsafe.

Redesign is re-typing under updated `(E, T̂, H, R)`.

---

# 11. Power (Descriptive Typing)

Power is the capacity to:

- reassign disturbance,
- reallocate buffer ownership,
- shift cost across nodes,
- extend or compress horizons,
- alter load topology.

Power does not eliminate cost.

It redistributes it.

Claims about power that do not specify topology are under-typed.

---

# 12. Claim Categories

All claims about execution fall into one of:

- **Execution claims** — causal state transition assertions
- **Optimization claims** — improvement assertions
- **Agency claims** — boundary choice assertions
- **Responsibility claims** — load attribution assertions
- **Metric claims** — evaluation interface assertions
- **Meaning claims** — coordination artifact assertions
- **Governance claims** — boundary and redesign authority assertions

Typing errors frequently arise from claim-kind confusion.

---

# 13. Typing Outcomes (Three-Valued)

Every claim is exactly one of:

### Well-Typed
Structurally coherent under declared `(E, T̂, H, R)`.

### Under-Typed
Missing required primitives, witnesses, or declarations.

### Ill-Typed
Violates execution primitives or structural rules.

The three-valued system is necessary under partial observability and horizon bounds.

---

# 14. What This Layer Does Not Do

This discipline does not:

- determine moral correctness,
- determine truth,
- select goals,
- choose optimal policies,
- guarantee success,
- eliminate conflict.

It determines only:

> Whether a claim about bounded execution could possibly be coherent.

---

# Summary

Given the execution primitives:

- finite resources,
- partial observability,
- irreversibility,
- abstraction loss,
- drift,
- horizon boundedness,
- topology,
- consequence propagation,
- structural viability,

this typing discipline:

- rejects category errors,
- marks incomplete reasoning,
- forces explicit horizons and load paths,
- prevents false agency and false responsibility,
- stabilizes coordination claims.

It does not tell you what to want.

It tells you when what you are saying  
is structurally admissible  
for systems that must actually run.
