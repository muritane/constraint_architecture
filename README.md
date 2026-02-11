# Constraint Architecture for Bounded Execution

A layered constraint framework for reasoning about action in bounded, irreversible, drift-exposed systems.

This repository defines a structured stack for analyzing:

- What must be true for systems to execute,
- When claims about execution are coherent,
- How systems stabilize under disturbance,
- How agents traverse possibility space under constraint,
- How norms bind action space,
- How authority modifies constraints,
- And how strategic interaction unfolds without destroying viability.

This is not a philosophy project.

It is an execution-grounded architecture.

---

# Why This Exists

Many frameworks about:

- agency,
- optimization,
- leadership,
- coordination,
- responsibility,
- institutional design,
- strategy,

fail structurally because they:

- mix descriptive and normative claims,
- assume infinite slack implicitly,
- ignore irreversibility,
- collapse topology into metaphor,
- allow horizon sliding,
- treat narrative as binding constraint,
- optimize locally while eroding long-term viability.

This repository separates constraint classes explicitly.

It provides a **static checker for discourse about execution in real systems that must continue to run.**

---

# Core Principle

> Optimization is undefined without viability.  
> Responsibility is undefined without load tracing.  
> Agency is undefined without a decidable refusal boundary.  
> Metrics are invalid unless they can fail explicitly.  
> Strategy is undefined outside viability-preserving action space.  

Everything else is interpretation.

---

# Architecture Overview

The system is layered. Lower layers constrain higher ones.

```
docs/
  0_core/
    execution_primitives.md
  1_structural/
    typing_discipline.md
  2_control/
    control_layer.md
  3_cognitive/
    cognitive_layer.md
  4_domain/
    robotics.md
    personal_domain.md
  5_normative/
    normative_layer.md
  6_governance/
    governance_layer.md
  7_strategic/
    viability_constrained_game_theory.md
```

Each layer:

- Declares its assumptions,
- Identifies its dependency layers,
- States horizon scope,
- Defines failure semantics,
- Preserves viability precedence,
- Does not contradict lower layers.

---

# Layer Summary

## 0 — Core

Defines execution primitives:

- Finite resources
- Partial observability
- Irreversibility
- Irreversible abstraction
- Drift / non-stationarity
- Horizon boundedness
- Topological structure
- Consequence propagation
- Structural viability

If these are invalid, the entire stack changes.

---

## 1 — Structural (Typing Discipline)

Defines what counts as a well-formed executional claim.

Introduces:

- Executability boundary
- Viability gate
- Degree-of-freedom partition
- Decidable agency boundary
- Load-traceable responsibility
- Metric validity constraints
- Three-valued typing (Well-Typed / Under-Typed / Ill-Typed)

This layer behaves like a static type checker for execution discourse.

---

## 2 — Control

Defines how systems maintain stability under disturbance and drift.

Covers:

- Feedback loops
- Buffer management
- Stability margins
- Latency constraints
- Control failure modes
- Viability-blind optimization risks

Control preserves viability; it does not select goals.

---

## 3 — Cognitive

Defines how bounded agents:

- Represent possibility space,
- Traverse effective infinity,
- Allocate attention,
- Balance exploration and exploitation,
- Commit irreversibly under drift.

Global optimality is rarely well-typed.

Reachability dominates existence.

---

## 4 — Domain Instantiations

Applies the stack to embodied domains:

- Robotics (ROS/ROS2, control loops, hardware constraints)
- Long-horizon personal systems (health, commitments, agency boundaries)

Other domains may be added without modifying lower layers.

---

## 5 — Normative

Specifies:

- Goals,
- Trade-offs,
- Prohibitions,
- Legitimacy conditions,
- Value constraints.

Norms restrict admissible action space.

They do not override physics.

Optimization occurs only within normative constraints and viability bounds.

---

## 6 — Governance

Defines:

- Authority over constraints,
- Interface contracts between layers,
- Redesign conditions,
- Versioning rules,
- Enforcement structures,
- Stack integrity preservation.

Governance allocates constraint-modification power.

It does not abolish execution primitives.

---

## 7 — Strategic

Embeds multi-agent interaction within bounded execution.

Introduces:

- Viability-constrained strategy space,
- Horizon-declared equilibrium analysis,
- Drift-robustness requirements,
- Buffer-aware repeated interaction,
- Load-aware mechanism design,
- Equilibrium classification (viable / fragile / buffer-consuming / ill-typed).

Game theory is not revised.

It is constrained to remain execution-coherent.

---

# Design Invariants

Across all layers:

1. Viability precedes optimization.
2. Irreversibility constrains trajectory.
3. Drift invalidates stationary assumptions.
4. Topology determines load routing.
5. Metrics must fail explicitly.
6. Power redistributes cost; it does not remove it.
7. Horizon must be declared or inferable.
8. Redesign pathways must remain accessible.

---

# What This Repository Is Not

It is not:

- A moral doctrine
- A political theory
- A productivity system
- A motivational philosophy
- A universal metaphysics
- A replacement for formal game theory
- A control theory textbook

It is a constraint discipline for systems that must execute under load.

---

# How to Use

1. Start at `0_core/`.
2. Move upward layer by layer.
3. Do not modify higher layers without checking lower ones.
4. When analyzing a system:
   - Declare horizon (H)
   - Identify topology (T̂)
   - Specify resource margins (R)
   - Define viability conditions (V)
   - Identify failure semantics
   - Classify claims via typing discipline
   - Evaluate strategy within viability-constrained action space

If you skip a layer, you are likely making an under-typed or ill-typed claim.

---

# Extension Policy

- New domains belong in `4_domain/`.
- New strategic models belong in `7_strategic/`.
- Structural modifications require updating `1_structural/`.
- Core changes require explicit governance revision in `6_governance/`.

Core primitives change only if physical understanding changes.

---

# Compression

This repository separates:

- What execution cannot escape,
- What reasoning must respect,
- How systems stabilize,
- How agents traverse,
- What goals restrict action,
- Who can modify constraints,
- And how strategic interaction unfolds without destroying viability.

Lower layers constrain higher ones.

Everything above the Core is adaptive.

The Core remains stable unless reality itself changes.

Execution is not optional.

Systems that forget this collapse.
