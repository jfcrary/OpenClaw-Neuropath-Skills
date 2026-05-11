---
name: conclusion
description: Produce the shortest defensible answer to the scientific question after interpretation is complete. Use when results and discussion already exist and the work now requires calibrated final claims, belief-updating, decision consequences, and explicit statement of whether the study succeeded, failed, or remained indeterminate.
---

# Conclusion

State the shortest defensible answer to the question.

This skill exists because many scientific workflows never cleanly separate:
- what happened
- what it means
- what can honestly be concluded

Your job is to produce the final answer layer.

## Role in the pipeline

Use this skill after:
- `data-analyzer`
- `interpretation-discussion`
- before `publication-manuscript-drafting` when a manuscript is the goal

## Purpose

`conclusion` is the claim-calibration and belief-update skill.

It should answer:
- what is the most defensible final claim?
- how much did belief change?
- did the study succeed in testing the question?
- what decision follows?

It does not:
- repeat the whole discussion
- add new analyses
- rewrite the dataset
- inflate claim strength

## Governing principles

### 1. Conclusions must be earned

A conclusion is not a summary of effort.

It is the narrowest defensible statement that survives the data, the analysis, and the discussion.

### 2. Separate answer from aspiration

Conclusions should state what the study established or failed to establish, not what the field hopes is true.

### 3. Distinguish four states explicitly

At the end of the pipeline, the study should land in one of these states:
- supports the hypothesis
- weakens the hypothesis
- contradicts the hypothesis
- remains indeterminate / failed to test decisively

Do not collapse indeterminate into weak support.

### 4. Calibrate claim strength tightly

A conclusion should be shorter and sharper than a discussion, but usually more conservative.

It should state:
- what changed in belief
- what did not change
- what next decision is justified

### 5. Preserve scope boundaries

Always specify:
- what tissue
- what cohort
- what disease context
- what assay level
- what resolution level
- what inferential level

If the finding is thumbnail-level, say so.
If it is cross-sectional, say so.
If it is single-cohort, say so.

### 6. Distinguish scientific answer from workflow answer

Sometimes the biological question remains open, but the workflow question is answered.

Example:
- biology indeterminate
- method feasible
- assay too noisy
- cohort usable

That still matters.

## Role in the pipeline

This is the final claim-calibration skill in the scientific-method stack.

Its central question is:
- **What is the shortest defensible answer to the question, and what decision follows?**

This is the last scientific-reasoning layer before manuscript packaging.

It is not the discussion skill.
It is not the manuscript-assembly skill.

## Boundary

This skill should stop after producing a Conclusion Block.

It may:
- state the final answer
- calibrate claim strength
- define scope limits
- state the decision consequence
- classify whether the study succeeded, failed, or remained indeterminate

It should not:
- repeat the whole discussion
- add new interpretation layers
- package the manuscript
- redesign the experiment

This skill should be short, sharp, and disciplined.

## Handoff in

The canonical input to this skill is:

# Interpretation Memo

Useful optional supporting inputs include:
- # Analysis Result Memo
- # Study Design Packet

Those are optional because the final claim may need to verify:
- what was tested
- what was found
- what the interpretation already established

But the primary handoff remains singular:
- interpretation in
- conclusion out

## Handoff out

The canonical output of this skill is:

# Conclusion Block

This is the formal handoff to `publication-manuscript-drafting`.

## Required output structure

# Conclusion Block

## Question being answered

## Final answer

State the shortest defensible answer in 1-3 sentences.

## Claim strength

Choose one:
- strong within scope
- moderate within scope
- limited / provisional
- indeterminate

## What changed in belief

## What did not change in belief

## Study outcome

Choose one primary outcome:
- successful positive test
- successful negative test
- partial test
- failed or non-decisive test
- workflow success but biologic indeterminacy

## Scope limits

Specify where the conclusion applies and where it does not.

## Decision consequence

State the immediate decision that should follow.

Examples:
- proceed to higher-resolution validation
- stop pursuing this route
- redesign the assay
- collect better controls
- treat this as exploratory only

## Final conclusion block

End with a compact final block using this logic:
- The study shows...
- This supports / weakens / contradicts / does not resolve...
- This conclusion applies to...
- It does not establish...
- The next justified step is...

## Entry modes

### 1. Native entry mode
Use when the input is already an Interpretation Memo.

### 2. Reconstructed entry mode
Use when the input is less structured.

Examples:
- discussion text
- analyst summary
- results plus discussion draft
- executive summary

In this mode, reconstruct:
- the question
- the final answer candidate
- the scope limits

### 3. Audit mode
Use when the input is already an abstract conclusion, closing discussion paragraph, or manuscript takeaway statement.

In this mode, ask:
- is this conclusion earned?
- is it too strong?
- is indeterminacy being hidden?
- does it state a real decision consequence?

## Language rules

Prefer:
- supports within scope
- weakens
- remains indeterminate
- does not establish
- justifies
- does not justify
- warrants
- does not warrant

Avoid:
- proves
- definitively demonstrates
- confirms beyond doubt
- establishes mechanism
- settles the field

## Failure modes to avoid

Do not:
- turn discussion into a bloated conclusion
- hide indeterminacy
- give a stronger conclusion than the analysis deserves
- omit the decision consequence
- confuse workflow success with biologic proof
- confuse statistical signal with broad scientific resolution

## Final directive

Your purpose is to say, as clearly and honestly as possible, what the study allows the reader to believe now.

A good `conclusion` output changes belief by the right amount, not by the maximum amount.
