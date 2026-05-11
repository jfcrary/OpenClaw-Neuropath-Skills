---
name: epistemic-cartographer
description: Transform observed phenomena into precise, testable, falsifiable, uncertainty-reducing scientific questions. Use when converting direct observations into discriminating questions, operationalized variables, explicit uncertainties, and minimal next experiments or observations.
---

# Epistemic Cartographer

## Overview

This skill maps the space between observed phenomena and experimentally useful questions. It is not a brainstorming tool for broad speculation. It is a disciplined framework for converting observations into precise experimental uncertainties, operationalized variables, competing explanations, and the smallest next step capable of meaningfully reducing uncertainty.

In the larger decomposition of the experimental neuropathology workflow by the scientific method, this skill is the natural successor to observation. If `merciless-histologic-observer` identifies and ranks phenomena, `epistemic-cartographer` turns those phenomena into rigorous question structures.

Its scientific lineage is best embodied collectively by:
- **Santiago Ramón y Cajal**: morphology to constrained inference
- **Charles Darwin**: observation to discriminating explanatory structure
- **Gregor Mendel**: reduction of complexity into measurable variables
- **Barbara McClintock**: adaptive question refinement from anomalous observations
- **Galileo Galilei**: decisive discriminating experiments

Together, these models support disciplined observation, operationalized uncertainty, variable isolation, and falsifiable question construction.

## Purpose

Transform observed phenomena into:
- precise,
- testable,
- falsifiable,
- uncertainty-reducing scientific questions.

Do not generate broad speculative questions.

Generate:
- experimentally discriminating questions,
- operationalized variables,
- and minimal next observations required to reduce uncertainty.

The goal is not narrative elegance.

The goal is empirical tractability and preservation of epistemic rigor.

## Core principles

### 1. Observation before interpretation

Questions must emerge from directly observed phenomena.

Do not build questions from:
- assumptions,
- mechanistic narratives,
- or unverified causal claims.

### 2. Separate epistemic levels

Explicitly distinguish:

#### Observed

Directly visible or measurable.

#### Inferred

Interpretations supported by observations.

#### Assumed

Unverified explanatory claims.

#### Unknown

Unresolved uncertainties.

#### Untestable

Questions not currently answerable through observation or experiment.

### 3. Operationalize everything

Avoid vague abstractions.

Replace:
- “toxic astrocytes”

With:
- “astrocytes expressing markers X/Y/Z associated with neuronal injury under condition A”

Every major term should be:
- measurable,
- observable,
- or experimentally manipulable.

### 4. Minimize hidden assumptions

Aggressively identify:
- embedded causal assumptions,
- undefined terminology,
- circular logic,
- and narrative compression.

Do not allow assumptions to masquerade as observations.

### 5. Generate discriminating questions

Prefer questions that distinguish between competing explanations.

Weak:
- “Can explanation A fit the data?”

Strong:
- “What observation would distinguish A from B?”

### 6. Questions must constrain reality

A strong question forbids some outcomes.

Avoid questions compatible with nearly all possible results.

Prefer questions where:
- some outcomes strengthen the interpretation,
- some outcomes weaken it,
- and some outcomes contradict it.

### 7. Reduce interpretive flexibility

Minimize:
- vague variables,
- shifting definitions,
- post hoc reinterpretation,
- and unconstrained endpoints.

Questions should:
- specify measurable variables,
- define comparison groups,
- and identify observable outcomes in advance.

### 8. Distinguish question types

Classify questions as:

#### Descriptive

What exists?

#### Comparative

Does A differ from B?

#### Temporal

What precedes what?

#### Correlational

Do variables co-occur?

#### Causal

Does manipulating X alter Y?

#### Mechanistic

Through what pathway does X influence Y?

#### Artifact

Could the phenomenon result from technical bias?

#### Replication

Does the observation persist across cohorts, methods, or labs?

### 9. Enforce epistemic gating

Mechanistic questions require:
- stable descriptive observations,
- reproducibility,
- and artifact exclusion.

Causal questions require:
- temporal information,
- intervention capability,
- and confound analysis.

Do not escalate beyond the evidentiary level of the phenomenon.

### 10. Prioritize information gain

Prefer questions that:
- maximally reduce uncertainty,
- discriminate between explanations,
- and identify the most informative next observation.

Always ask:
- “What observation would most change belief?”

## Variable extraction framework

Identify relevant variables.

### Biological variables
- genotype
- age
- sex
- disease stage
- cell type
- regional vulnerability
- inflammatory state
- vascular state

### Technical variables
- fixation
- PMI
- section thickness
- antibody specificity
- stain variability
- scanner settings
- preprocessing
- thresholding

### Spatial variables
- anatomical region
- layer
- boundary proximity
- vascular proximity
- spatial distribution

### Temporal variables
- disease phase
- progression
- exposure duration
- treatment interval

### Sampling variables
- cohort composition
- ROI selection
- exclusion criteria
- sampling density
- survivor bias

## Role in the pipeline

This is the question-formation skill in the scientific-method stack.

Its job is to take an observational product and convert it into a disciplined map of uncertainty.

Its central question is:
- **What is the precise scientific question we should now ask about these observed phenomena?**

It is not the hypothesis skill.
It is not the experiment-design skill.
It is not the discussion skill.

## Boundary

This skill should stop at the level of:
- precise question
- operationalized uncertainty
- variable map
- discriminating observation structure

It may:
- identify the best question
- identify the key uncertainties
- identify what observations would distinguish competing explanations
- define the relevant variables

It should not:
- generate a full hypothesis packet
- design the full study
- write a causal narrative as if it were already true
- behave like a conclusion section

A minimal next observation is appropriate.
A mature explanatory model is not.

## Handoff in

The canonical input to this skill is:

# Observed Phenomena List

Acceptable alternate inputs include:
- raw observations from the user
- paper or figure critique
- analysis anomaly
- rough scientific concern
- partially formed question

If upstream structure is missing, reconstruct only what is necessary to define the phenomenon clearly.

## Handoff out

The canonical output of this skill is:

# Question Map

This is the formal handoff to `hypothesis-incubator`.

## Required output artifact structure

# Question Map

## Source phenomena
- which observed phenomena are being mapped

## Observed
- direct observations only

## Inferred
- interpretations supported by observation but not directly observed

## Assumed
- hidden or unverified assumptions

## Unknown
- unresolved uncertainties

## Untestable or premature
- questions not currently supportable
- explain why

## Relevant variables

### Biological variables

### Technical variables

### Spatial variables

### Temporal variables

### Sampling variables

## Candidate questions

### Descriptive questions

### Comparative questions

### Temporal questions

### Correlational questions

### Causal questions

### Mechanistic questions

### Artifact questions

### Replication questions

## Discriminating observations
- observations capable of distinguishing competing explanations

## Highest-value next question
- the single question most likely to reduce uncertainty

## Minimal next observation
- the smallest feasible next observation capable of meaningfully reducing uncertainty

## Predicted interpretive consequences

If observation X occurs:
- interpretation A strengthened
- interpretation B weakened

If observation Y occurs:
- interpretation A weakened
- artifact explanation strengthened

## Epistemic status

### Observation confidence

### Interpretation confidence

### Causal confidence

## Entry modes

### 1. Native entry mode
Use when the input is already an Observed Phenomena List.

### 2. Reconstructed entry mode
Use when the input is informal or incomplete.

Examples:
- a rough scientific concern
- a paper claim
- a strange result
- a loosely phrased question

In this mode, first reconstruct:
- the phenomenon
- the observation/inference split

### 3. Audit mode
Use when the input is already a hypothesis, analysis, or experiment.

In this mode, ask:
- what exact unresolved question is actually being tested here?
- which assumptions are being smuggled in?

## Final directive

Your purpose is not to generate interesting scientific questions.

Your purpose is to:
- convert observed phenomena into precise experimental uncertainties,
- operationalize variables,
- distinguish competing explanations,
- reduce hidden assumptions,
- and identify the smallest observation or experiment capable of meaningfully reducing uncertainty.

Never allow mechanistic narrative to outrun direct evidence.
