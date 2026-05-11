# Scientific-Method Skill Pipeline for Experimental Neuropathology

This repository contains a handoff-aware skill stack for experimental neuropathology research organized around the scientific method.

The design goal is not just to generate prose or isolated analyses, but to carry a project from first observation to manuscript assembly with explicit boundaries, canonical intermediate artifacts, reconstruction modes, and audit modes.

## Pipeline overview

The stack is organized into two modules.

### Module A, pre-data scientific design
1. **merciless-histologic-observer**
   - role: disciplined observation and phenomenon ranking
   - canonical output: **Observed Phenomena List**

2. **epistemic-cartographer**
   - role: question formation and uncertainty mapping
   - canonical output: **Question Map**

3. **hypothesis-incubator**
   - role: explanatory-model formation and prediction generation
   - canonical output: **Hypothesis Packet**

4. **experiment-designer**
   - role: test design and operational bridge into execution
   - canonical output: **Study Design Packet**

### Module B, post-data execution and inference
5. **data-collector**
   - role: collection, logging, preservation, and dataset freezing
   - canonical outputs:
     - **Data Collection Ledger**
     - **Frozen Analysis Dataset Package**

6. **data-analyzer**
   - role: inferential analysis and belief-updating from frozen data
   - canonical output: **Analysis Result Memo**

7. **interpretation-discussion**
   - role: meaning-making, competing interpretations, and scope-aware discussion
   - canonical output: **Interpretation Memo**

8. **conclusion**
   - role: final claim calibration and decision consequence
   - canonical output: **Conclusion Block**

9. **publication-manuscript-drafting**
   - role: manuscript assembly and stage-aware publication drafting
   - canonical output: **Manuscript Draft Package**

## Canonical artifact chain

The full handoff chain is:

1. **Observed Phenomena List**
2. **Question Map**
3. **Hypothesis Packet**
4. **Study Design Packet**
5. **Data Collection Ledger**
6. **Frozen Analysis Dataset Package**
7. **Analysis Result Memo**
8. **Interpretation Memo**
9. **Conclusion Block**
10. **Manuscript Draft Package**

## Core design principles

- observation before explanation
- uncertainty made explicit
- hypotheses must generate discriminating predictions
- experiment design must define the expected downstream dataset
- data collection must preserve provenance, exclusions, and missingness
- analysis must distinguish true negative, contradictory, and failed-to-test outcomes
- interpretation must separate technical from biologic meaning
- conclusions must stay scoped to what the evidence actually earned
- manuscript drafting must not silently upgrade weak science into confident prose

## Shared architectural features

Across the stack, skills are designed to support:

- **clear role and boundary**
- **handoff in / handoff out**
- **canonical emitted artifact**
- **reconstructed entry mode** for late-entry projects
- **audit mode** for critique of existing work

Several later-stage skills also support retrospective use, where archival or already-collected data must be analyzed honestly without pretending they arose from a fully prospective design.

## Special note on the breakpoint skill

`experiment-designer` is the key breakpoint in the pipeline.

It marks the transition from:
- conceptual scientific design

to:
- actual execution, collection, and data generation

That skill is responsible for turning a hypothesis into a realistic, testable study design with explicit design path, sample-size or feasibility logic, expected frozen dataset schema, and collection deliverables.

## Manuscript drafting stages

`publication-manuscript-drafting` supports three drafting stages:

1. **outline**
2. **first draft**
3. **final draft**

It also includes a readiness gate so that a project can be classified as:
- outline-ready
- first-draft-ready
- final-draft-ready
- or not yet manuscript-ready

This is meant to prevent premature polishing and force honesty about scientific maturity.

## Repository contents

Each top-level folder corresponds to one skill and contains its `SKILL.md` file.

## Intended use

This stack is designed for experimental neuropathology research, especially projects that begin with direct tissue observation, evolve through explicit uncertainty and design logic, and aim for publishable outputs without losing epistemic discipline along the way.
