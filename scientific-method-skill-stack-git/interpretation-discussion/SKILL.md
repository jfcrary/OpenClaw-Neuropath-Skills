---
name: interpretation-discussion
description: Convert analyzed results into disciplined scientific meaning. Use when a frozen dataset has already been analyzed and the work now requires interpretation, discussion, alternative-explanation handling, literature positioning, claim calibration, and conceptual synthesis without collapsing into a final conclusion or manuscript draft.
---

# Interpretation Discussion

Turn results into scientific meaning without overstating them.

Do not rewrite the data.
Do not repeat the methods.
Do not jump straight to final conclusion.

Your job is to answer:
- what the results mean
- what they do not mean
- what alternative explanations remain
- how the findings relate to prior knowledge
- what conceptual model is strengthened or weakened

## Role in the pipeline

Use this skill after:

- `data-analyzer`
- before `conclusion`
- before `publication-manuscript-drafting`

This skill sits between analysis and final claim-making.

## Purpose

`interpretation-discussion` is the meaning-making layer of the scientific pipeline.

It translates analytical output into:
- biologic interpretation
- methodological interpretation
- relationship to prior literature
- explanation of uncertainty
- clarification of what belief should change

It does not:
- silently strengthen weak analyses
- convert ambiguous data into forced positivity
- replace the conclusion section
- package the work as a manuscript

## Governing principles

### 1. Interpretation begins from results, not wishes

Start from what the analysis actually showed.

Not:
- what was hoped for
- what would be fashionable
- what the literature prefers

### 2. Separate result from meaning

Always distinguish:
- result
- interpretation
- alternative interpretation
- remaining uncertainty

Do not let those collapse into one paragraph.

### 3. Discussion is not repetition

Do not merely restate the results section.

A good discussion answers:
- why this pattern matters
- how it changes understanding
- whether it is surprising
- whether it supports or challenges prior expectations
- whether it is biologically specific or technically contingent

### 4. Keep claim strength proportional

Interpretation should be stronger than raw result reporting but weaker than unjustified conclusion inflation.

Use calibrated language such as:
- suggests
- is consistent with
- supports the possibility that
- is more compatible with
- weakens the interpretation that
- does not distinguish among

### 5. Alternative explanations are mandatory

A serious discussion must handle:
- artifact explanations
- confounding explanations
- competing biologic explanations
- design limitations
- measurement limitations

Do not mention them perfunctorily. Explain how they affect meaning.

### 6. Literature should contextualize, not dominate

Position the findings relative to prior work.

Ask:
- does this align with prior studies?
- does it refine them?
- does it challenge them?
- is the present work weaker, stronger, narrower, or differently scoped?

Do not force artificial harmony with the literature.

### 7. Distinguish biologic from technical interpretation

For neuropathology and digital pathology, always consider both:

#### Biologic interpretation
- disease mechanism
- cell type
- region
- stage
- clinicopathologic relationship

#### Technical or workflow interpretation
- QC
- stain behavior
- dynamic range
- segmentation performance
- thumbnail vs WSI limitations
- sample composition effects

### 8. Explain what changed in belief

The discussion should state what the analysis newly supports, weakens, or leaves unresolved.

## Role in the pipeline

This is the meaning-making skill in the scientific-method stack.

Its central question is:
- **What do these analyzed results mean, what do they not mean, and which interpretations remain most defensible?**

This is the disciplined discussion layer.

It is not the final answer layer.
It is not the manuscript-assembly layer.

## Boundary

This skill should stop after producing an Interpretation Memo.

It may:
- interpret the analytic result
- compare competing interpretations
- separate biologic from technical interpretation
- relate the result to prior expectations or literature
- state what remains unresolved

It should not:
- give the final shortest defensible claim
- decide the ultimate conclusion state
- package the manuscript

Discussion yes.
Final conclusion no.

## Handoff in

The canonical input to this skill is:

# Analysis Result Memo

Useful optional supporting inputs include:
- # Study Design Packet
- # Hypothesis Packet

Those are optional because they help recover:
- what was supposed to be tested
- what predictions existed

But the primary immediate input is still the analysis result.

## Handoff out

The canonical output of this skill is:

# Interpretation Memo

This is the formal handoff to `conclusion`.

## Required output structure

# Interpretation Memo

## Interpretation target

State the specific result set being interpreted.

## Core result being interpreted

Summarize the main analytic finding in 1-3 sentences.

## Primary interpretation

State the most defensible meaning of the result.

## Competing interpretations

List the main alternatives:
- alternative biologic interpretation
- confounding explanation
- artifact or measurement explanation
- null-compatible interpretation

## What the result strengthens

## What the result weakens

## What the result does not resolve

Be explicit.

## Relationship to prior expectations or literature

State whether the result:
- aligns with prior work
- partially aligns
- complicates prior work
- appears discordant
- is too indirect to compare strongly

## Technical interpretation

Explain whether the result could reflect:
- assay properties
- dynamic-range asymmetry
- tissue composition
- scanner or preprocessing behavior
- low-resolution screening constraints
- model or threshold choices

## Biologic interpretation

Explain the most defensible biologic meaning if the signal is real.

## Scope of interpretation

State what population, tissue type, region, disease stage, or assay context the interpretation should apply to.

## Interpretation limits

State clearly what cannot be concluded.

Examples:
- no causal inference
- no temporal inference
- no proof of specificity
- no mechanistic proof
- no generalization beyond thumbnail-level screening

## Decision-relevant meaning

Explain how the interpretation should affect next steps.

## Bridge to conclusion

End by stating:
- what belief changed
- what ambiguity remains
- what still requires final claim calibration

## Entry modes

### 1. Native entry mode
Use when the input is already an Analysis Result Memo.

### 2. Reconstructed entry mode
Use when the input is less structured.

Examples:
- raw results section
- figure set
- stats output
- analyst summary

In this mode, reconstruct:
- the core result
- the apparent tested prediction
- the most likely competing interpretations

### 3. Audit mode
Use when the input is already a draft discussion, manuscript interpretation, or lab meeting narrative.

In this mode, ask:
- is the interpretation stronger than the analysis warrants?
- are alternatives handled honestly?
- is technical explanation being confused with biologic explanation?

## Discussion-writing rules

A good discussion paragraph often has this shape:
1. state the result’s meaning
2. explain why that meaning is plausible
3. compare to alternatives
4. mark the main caveat
5. state what should happen next

## Language rules

Prefer:
- consistent with
- suggests
- more compatible with
- weakens the interpretation that
- leaves unresolved
- may reflect
- cannot distinguish
- should be interpreted in light of

Avoid:
- proves
- clearly demonstrates
- definitively establishes
- confirms mechanism
- settles the issue

## Failure modes to avoid

Do not:
- repeat the results as filler
- overfit the discussion to the hoped-for story
- bury the main caveat
- pretend ambiguity is clarity
- confuse a useful signal with a decisive result
- let literature override the actual data
- force a grand biologic story from a narrow technical assay

## Final directive

Your purpose is to extract honest scientific meaning from analyzed data.

A good `interpretation-discussion` output tells the reader:
- what the results most likely mean
- what else they could mean
- what remains unresolved
- and why the work matters despite those uncertainties
