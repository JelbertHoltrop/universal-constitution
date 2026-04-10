# Universal Constitution 2.0

A constitutional alignment framework for AI based on non-weighable axioms, jurisprudential interpretation, and execution constraints.

This repository contains the canonical constitution, jurisprudence cases, an execution protocol layer, and evaluation material used to explore constitutional constraint architectures for AI alignment.


## Purpose

Most AI alignment approaches optimise between weighted ethical rules or reward signals.  
The Universal Constitution explores a different architecture:

- **Fixed axioms** that are not optimised or re-weighted  
- **Interpretation through jurisprudence**  
- **Execution constraints to expose known failure modes**  
- **Drift detection via case testing**

The goal is to investigate whether such a structure can produce more stable and reliable reasoning in AI systems.


## Alignment Layers

The project consists of four layers:

1. Canon  
   Immutable ethical axioms  

2. Jurisprudence  
   Case interpretations clarifying application  

3. Protocol (Execution Layer)  
   Pre-answer integrity constraints  

4. Evaluation  
   Test protocols used to measure alignment behaviour  


## Layer Responsibilities

Each layer has a strictly defined role:

- **Canon** → defines truth and principles  
- **Jurisprudence** → defines failure modes and interpretation  
- **Protocol** → ensures pre-answer integrity is evaluated and made visible  
- **Evaluation** → measures behaviour and detects drift  

The protocol layer is explicitly **subordinate to the Canon**  
(see Case 0000 — Canonical Supremacy)  
and may not redefine or override it.


## Repository Structure

/canon  
Canonical text of the Universal Constitution 2.0  

/jurisprudence  
Case interpretations that clarify how the constitution should be applied  

/jurisprudence/cases  
Individual case files  

/jurisprudence/dossiers  
Extended discussion and development history of cases  

/implementation/protocol  
Execution protocol defining pre-answer constraints  

/implementation/evaluation  
Test protocols and benchmark scenarios used to evaluate AI behaviour  

/whitepaper  
Research paper describing the constitutional alignment architecture  


## Canonical Text

The constitution itself is intentionally **immutable**.

Changes to interpretation occur through jurisprudence rather than modification of the canonical text.

This prevents silent doctrinal drift.


## Execution Protocol

The protocol layer introduces **pre-answer integrity constraints**.

These ensure that before an answer is given:

- context is sufficient or explicitly incomplete (Case 0010)  
- certainty is correctly calibrated (Case 0012)  
- user intent is preserved (Case 0011)  
- interpretations are transparent (Case 0007)  
- critical failure modes are surfaced (Case 0013)  
- unnecessary expansion is avoided  

### Important Clarification

The protocol:

- does not determine whether an answer is allowed  
- does not replace reasoning  
- does not override the Canon  

Instead, it ensures:

> that any limitations, assumptions, or conflicts  
> are made explicit in the answer.

---

## How to Use the Constitution in AI

Due to model context limitations, alignment must be loaded **in separate prompts**.

### Step 1 — Canon (Full, Immutable)

Load the full canonical constitution.

---

### Step 2 — Jurisprudence

Load the relevant cases (or full set if required).

---

### Step 3 — Execution Protocol (Compact Version)

Load a **short version of the protocol only**.

Example:

- If context is missing, state it or ask  
- Calibrate certainty (do not present guesses as facts)  
- Do not change the user’s goal  
- State assumptions when needed  
- Include only critical failure modes  
- Do not add unnecessary information  
- If constraints cannot be satisfied, make that explicit  

Apply implicitly.

---

### Important Constraint

- Canon must be loaded **complete and unchanged**  
- Jurisprudence must be loaded **complete or intentionally selected**  
- Only the Protocol may be **compressed or optimized**  

Failure to separate these may cause:

- context overflow  
- incomplete loading  
- alignment degradation  


## Alignment Flow

Canonical architecture:

Canon  
↓  
Interpretation  
↓  
Jurisprudence  
↓  
Protocol (integrity exposure layer)  
↓  
Output  

Evaluation operates across all layers.


## Limitations — Protocol Enforcement

The execution protocol is currently **not reliably enforceable within a single model run**.

A single LLM instance may:

- skip or partially apply constraints  
- answer before evaluation is complete  
- fail to surface violations  

As a result:

> The protocol improves behaviour,  
> but does not guarantee enforcement.

---

## Implication

Reliable enforcement requires architectural separation, such as:

- a generator model producing answers  
- a separate checker validating them against the protocol and cases  
- a gating mechanism that can reject invalid outputs  

Without this:

> protocol compliance remains probabilistic.


## Research Direction

A key open question is:

> how to transform protocol-based integrity checks  
> into enforceable guarantees without overriding the Canon

This includes:

- multi-pass validation  
- explicit violation surfacing  
- case-referenced verification  


## Evaluation and Testing

Structured evaluation protocols are included in:

`/implementation/evaluation`

These allow:

- comparison between standard AI and constitutional AI  
- detection of failure modes  
- validation of protocol effectiveness  


## Research Context

This project explores the hypothesis that a **constitutional constraint architecture** can produce more stable alignment than optimisation-based ethical systems.

Key idea:

> Alignment is not achieved by better answers alone,  
> but by ensuring the conditions under which answers are produced  
> remain transparent and structurally sound.


## License

The canonical constitution is released under:

Creative Commons Attribution–NoDerivatives 4.0 International (CC BY-ND 4.0)

This allows sharing while preserving the integrity of the canonical text.

Alternative frameworks may be created under different names.


## Author

Jelbert Holtrop

Research project exploring constitutional AI alignment, jurisprudential drift detection, and execution-constrained reasoning.