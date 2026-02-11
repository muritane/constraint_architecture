# Constraint Architecture for Bounded Execution

A layered constraint framework for reasoning about action in bounded, irreversible, drifting systems.

This repository defines:

- A **minimal execution core**
- A **static typing discipline** for executional claims
- Layered separation of structural, control, cognitive, and domain constraints
- A governance model for disciplined redesign
- Applied mappings to robotics and long-horizon personal systems

This is not a philosophy project.  
It is an execution-grounded architecture.

---

# Why This Exists

Most frameworks about agency, optimization, responsibility, and coordination:

- mix structural and normative claims,
- assume infinite resources implicitly,
- ignore irreversibility,
- collapse topology into metaphor,
- allow horizon sliding,
- treat narrative as binding constraint.

This repository separates constraint classes explicitly.

It provides a **static checker for discourse about execution**.

---

# Core Principle

> Optimization is undefined without viability.  
> Responsibility is undefined without load tracing.  
> Agency is undefined without a decidable refusal boundary.  
> Metrics are invalid unless they can fail explicitly.  

Everything else is interpretation.

---

# Architecture Overview

The system is layered. Lower layers constrain higher ones.

0_core/ → Physical execution invariants  
1_structural/ → Typing discipline for executional claims  
2_control/ → Stability and feedback under constraint  
3_cognitive/ → Bounded traversal and representation limits  
4_domain/ → Application-specific constraints (robotics, personal systems)  
5_normative/ → Goal specification and optimization envelopes  
6_governance/ → Rules for modifying the stack itself  


Each layer:

- Declares its horizon assumptions
- Identifies load topology
- States closure points
- Defines failure semantics
- References lower layers
- Does not contradict lower layers

---

# Layer Summary

## 0 — Core

Non-negotiable execution primitives:

- Bounded resources
- Partial observability
- Irreversibility
- Unavoidable abstraction
- Drift / non-stationarity
- Horizon-bounded validity
- Topological load propagation

These are structural properties of action in time.

If these are invalid, the entire framework changes.

---

## 1 — Structural (Typing Layer)

Defines what counts as a well-formed executional claim:

- Executability boundary
- Viability gating
- Closure and degree-of-freedom partition
- Decidable agency boundaries
- Responsibility via load tracing
- Metric validity constraints
- Regime → kinematics → dynamics → optimization ordering

This layer behaves like a static type checker.

It does not tell you what to do.
It tells you when what you are saying could possibly be true.

---

## 2 — Control

Addresses:

- Feedback loops
- Stability under disturbance
- Buffer management
- Error correction
- Variance bounding

Operates within Core and Structural constraints.

---

## 3 — Cognitive

Addresses:

- Bounded rationality
- Exploration vs exploitation
- Effective infinity
- Path dependence
- Irreversible abstraction in representation

Explains how agents cope with the Core.

---

## 4 — Domain

Application-specific instantiations.

Current focus:

- Robotics (ROS/ROS2, embodied systems, autonomy boundaries)
- Long-horizon personal systems (discipline, optionality preservation, viability under drift)

Other domains can be added or forked without modifying the Core.

---

## 5 — Normative

Specifies:

- Desired outcomes
- Trade-offs
- Optimization targets
- Forbidden actions

Goals must respect viability and structural constraints.

Optimization without a viability witness is ill-typed.

---

## 6 — Governance

Defines:

- When constraints can be modified
- What invalidates a primitive
- What counts as sufficient evidence
- How redesign escalates between layers

This prevents silent mutation of the stack.

---

# Applied Focus

## Robotics

Robotics is a stress test for executional coherence:

- Real-time horizons
- Hard irreversibility
- Physical load propagation
- Safety-critical control loops
- Explicit interface boundaries

The robotics domain demonstrates how the abstract stack maps to embodied systems.

---

## Personal Long-Horizon Systems

Long-horizon personal systems are treated as bounded executors:

- Finite time and energy
- Irreversible commitments
- Path-dependent traversal
- Optionality management
- Viability before optimization

This domain tests agency typing, redesign discipline, and horizon management.

---

# What This Repository Is Not

- Not a moral framework
- Not a productivity system
- Not a political theory
- Not a motivational doctrine
- Not a general metaphysics

It is a constraint discipline for bounded execution.

---

# How to Use

1. Start at `0_core/`.
2. Move upward layer by layer.
3. Do not modify higher layers without checking lower ones.
4. When applying to a domain:
   - Declare horizon
   - Identify topology
   - Specify closure
   - Define failure semantics
   - Declare redesign conditions

If you skip a layer, you are likely making an ill-typed claim.

---

# Extension Policy

- New domains go in `4_domain/`.
- Structural changes require updating `1_structural/`.
- Core changes require explicit governance discussion in `6_governance/`.

Core primitives should change only if physics-level constraints change.

---

# Compression

This repository separates:

- What execution cannot escape,
- What reasoning must respect,
- How systems stabilize,
- How agents traverse possibility space,
- What goals are pursued,
- And how the architecture itself evolves.

Lower layers constrain higher ones.

Everything above the Core is adaptive.
The Core is stable unless reality itself changes.
