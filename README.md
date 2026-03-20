# Universal Constitution 2.0

A constitutional alignment framework for AI based on non-weighable axioms and jurisprudential interpretation.

This repository contains the canonical constitution, jurisprudence cases, and evaluation material used to explore constitutional constraint architectures for AI alignment.


## Purpose

Most AI alignment approaches optimise between weighted ethical rules or reward signals.  
The Universal Constitution explores a different architecture:

- **Fixed axioms** that are not optimised or re-weighted
- **Interpretation through jurisprudence**
- **Drift detection via case testing**

The goal is to investigate whether such a structure can produce more stable ethical reasoning in AI systems.

## Alignment Layers

The project currently consists of three layers:

1. Canon  
   Immutable ethical axioms.

2. Jurisprudence  
   Case interpretations clarifying application.

3. Evaluation  
   Test protocols used to measure alignment behaviour.
## Repository Structure
/canon
Canonical text of the Universal Constitution 2.0

/jurisprudence
Case interpretations that clarify how the constitution should be applied

/jurisprudence/cases
Individual case files

/jurisprudence/dossiers
Extended discussion and development history of cases

/evaluation
Test protocols and benchmark scenarios used to evaluate AI behaviour

/whitepaper
Research paper describing the constitutional alignment architecture


## Canonical Text

The constitution itself is intentionally **immutable**.

Changes to interpretation occur through jurisprudence rather than modification of the canonical text.

This prevents silent doctrinal drift.


## How to Test the Constitution

The constitution can be used as an alignment layer in AI systems.

### Basic method

1. Start a new AI conversation.
2. Paste the full constitution and instruct the AI to use it as alignment.
3. Present ethical or technical scenarios.

### Adding Jurisprudence

Interpretation can be refined by adding jurisprudence cases.

1. Paste the constitution.
2. Paste one or more relevant case files from `/jurisprudence/cases`.
3. Ask the AI to use both the constitution and jurisprudence as alignment context.

Example prompt:

Use the following constitution and jurisprudence as alignment for this conversation:

[constitution text]

[case files]


Jurisprudence clarifies interpretation but does not modify the canonical text.

More structured evaluation protocols are included in the `/implementation/evaluation` directory.

Constitution
     ↓
Interpretation Layer
     ↓
Jurisprudence
     ↓
Evaluation / Drift detection


## Research Context

This project explores the hypothesis that a **constitutional constraint architecture** may produce more stable alignment than optimisation-based ethical rule systems.

The accompanying white paper:

*Constitutional Constraint Architecture for AI Alignment*


## License

The canonical constitution is released under:

Creative Commons Attribution–NoDerivatives 4.0 International (CC BY-ND 4.0)

This allows sharing while preserving the integrity of the canonical text.

Alternative frameworks may be created under different names.


## Author

Jelbert Holtrop

Research project exploring constitutional AI alignment and jurisprudential drift detection.
