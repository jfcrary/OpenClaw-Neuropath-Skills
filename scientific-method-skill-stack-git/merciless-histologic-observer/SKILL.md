---
name: merciless-histologic-observer
description: Apply disciplined, ground-truth-first histologic observation across manuscripts, figures, new experimental data, and comparative evidence review. Use when evaluating whether images and data really support their descriptions, methods, results, and conclusions; when generating or reviewing new pathology data; and when ranking observations or claims by likely truthfulness, reliability, replication support, and discovery importance.
---

# Merciless Histologic Observer

## Overview

This skill operationalizes a Cajal-style standard of scientific observation: disciplined seeing, careful description, ruthless separation of observation from interpretation, and explicit ranking of which phenomena may matter most. It is meant to counter one of the common failure modes of brain research and computational pathology: people are not observant enough, they accept descriptions too easily, and they let literature or theory overwrite ground truth.

Use this skill when the work requires direct scrutiny of what is actually present in images, figures, methods, data summaries, or claims.

The longer-term purpose of this skill is to support decomposition of the experimental neuropathology workflow according to the scientific method. In that larger framework, this skill corresponds to Step 1: observation.

## Core doctrine

Observation comes first.

Do not begin by explaining. Begin by seeing.
Do not begin by agreeing with the literature. Begin by checking what is actually there.
Do not begin by trusting the figure legend. Begin by testing whether the image, panel, table, or result supports it.

Ground truth outranks dogma.
Careful description outranks premature interpretation.
Phenomena outrank narratives.

## Cajal standard

Remember Santiago Ramón y Cajal as a model of scientific observation:
- disciplined seeing
- patient description
- willingness to notice what others missed
- ability to rank which observations might be important
- scientific seriousness about visual evidence

Discovery is often hiding in plain sight because the observer did not realize that a phenomenon was important.

## Primary uses

### 1. Manuscript and literature review

Use this skill to evaluate whether published or draft figures actually match:
- the figure legend
- the methods
- the stated results
- the discussion claims
- the overall conclusion

Key questions:
- Does the image show what the authors say it shows?
- Do the methods plausibly support the displayed result?
- Are the quantification, visual evidence, and verbal interpretation aligned?
- Are representative images actually representative?
- Do labels, arrows, scales, stains, or panel pairings help or mislead?
- Is there internal inconsistency between text, figure, and table?
- Is the visual evidence stronger, weaker, or more ambiguous than the prose implies?

### 2. New data generation and review

Use this skill when reviewing newly generated histologic, image-analysis, or pathology-adjacent outputs.

Examples:
- thumbnail cohorts
- tile overlays
- tissue masks
- stain burden summaries
- contact sheets
- embeddings
- heatmaps
- segmentation outputs
- pathology figures under construction

Key questions:
- What phenomenon is actually present?
- What is directly observed versus merely inferred?
- Could this be artifact, preprocessing bias, sampling bias, or a true biological signal?
- What deserves immediate follow-up?
- What is novel, strange, asymmetric, discordant, or unexpectedly absent?

### 3. Cross-study truthfulness and reliability ranking

Use this skill to rank observations or claims across studies by how likely they are to be true, reliable, and worth taking seriously.

Key questions:
- Do the actual data support the conclusion?
- Is the argument logically coherent?
- Are the images convincing or only rhetorically presented?
- Has the observation been replicated?
- Is the study underpowered, confounded, circular, or visually unconvincing?
- Is the claim modest and proportionate, or inflated beyond the evidence?
- Does this look like a real phenomenon, a weak trend, a technical artifact, or narrative overreach?

## Observation workflow

### Step 1. Identify the phenomenon

Ask:
- What exactly is being noticed?
- Is it a pattern, asymmetry, absence, mismatch, gradient, cluster, outlier, or contradiction?

Write the phenomenon in concrete terms before naming it theoretically.

### Step 2. Describe before interpreting

Describe:
- what is visible
- where it occurs
- how strong it appears
- whether it is focal or diffuse
- whether it is consistent across panels/cases/replicates

Avoid theoretical language too early.

### Step 3. Compare observation against the stated claim

If reviewing a manuscript, figure, or report, explicitly compare:
- observation
- legend
- methods
- results text
- conclusion

Look for alignment, overstatement, mismatch, or unsupported leaps.

### Step 4. Evaluate alternative explanations

Consider whether the observation could instead reflect:
- artifact
- staining variation
- sectioning effect
- sampling bias
- preprocessing distortion
- thresholding or segmentation error
- confounding biology
- selective presentation

### Step 5. Rank importance

Rank the observation by potential importance.

Suggested scale:
- **Level 0:** trivial / expected / uninformative
- **Level 1:** QC-relevant but biologically unimportant
- **Level 2:** valid descriptive finding, limited broader importance
- **Level 3:** interesting or potentially meaningful phenomenon worth follow-up
- **Level 4:** high-value observation with plausible biologic, technical, or conceptual importance
- **Level 5:** potentially field-shifting or discovery-grade if validated

Importance should be estimated using an explicit rubric, not only intuition.

## Importance rubric

Estimate importance across three major domains.

### A. Human and population importance

Ask:
- Does this connect to substantial morbidity?
- Does it connect to mortality?
- Is the affected disease or condition common (prevalence, incidence, lifetime burden)?
- Does it affect quality of life, disability, pain, cognition, or caregiver burden?

Suggested labels:
- **minimal**
- **limited**
- **moderate**
- **high**
- **very high**

### B. Scientific importance

Ask:
- If real, is this central to disease biology or more peripheral?
- Could it clarify a major uncertainty?
- Could it challenge or refine a dominant model?
- Could it unify disconnected observations?
- Could it matter across diseases rather than only in one narrow setting?

Suggested labels:
- **minimal**
- **limited**
- **moderate**
- **high**
- **very high**

### C. Translational and programmatic importance

Ask:
- Is this relevant to major NIH or fundable problem spaces?
- Could it matter for diagnosis, prognosis, staging, treatment, response monitoring, or prevention?
- Could it point toward a biomarker, target, assay, or practical measurement strategy?
- Would this plausibly matter to strategic research programs, not just narrow curiosity?

Suggested labels:
- **minimal**
- **limited**
- **moderate**
- **high**
- **very high**

### Overall importance judgment

After rating the three domains above, provide an overall importance judgment.

Important rule:
- Importance means **important if real**.
- This is separate from reliability.
- A phenomenon can be highly important in principle but still weakly supported.
- Do not let excitement about importance substitute for evidence.

### Step 6. Rank reliability / truthfulness

Separate importance from reliability.
A claim can be important if true, but weakly supported.

Suggested reliability dimensions:
- directness of evidence
- internal consistency
- visual credibility
- quantitative support
- methodologic adequacy
- replication / external support
- scope discipline

Suggested reliability summary labels:
- **highly credible**
- **credible but limited**
- **suggestive**
- **weak / overinterpreted**
- **not supported**

### Step 7. Connect the dots

Ask whether the observation links to:
- another dataset
- a known clinicopathologic pattern
- a hidden confounder
- a neglected region/cell type/process
- a previously misdescribed or underappreciated phenomenon

This is where discovery can emerge, but only after disciplined observation.

### Step 8. Propose the next discriminating check

Every strong observational note should end with:
- what to inspect next
- what would strengthen the phenomenon
- what would weaken it
- what additional data or comparison would clarify it

## Further-study worthiness scale (1-10)

Use this semiquantitative scale to rank how worthy a phenomenon is of further study.

| Score | Label | Meaning |
|---|---|---|
| 1 | None | Artifact, noise, obvious error, or trivial expected finding. No follow-up justified. |
| 2 | Minimal | Very low-value observation. At most useful for QC or bookkeeping. |
| 3 | Low | Valid but low-importance descriptive finding. Not a priority for further study. |
| 4 | Limited | Mildly interesting or somewhat unexpected, but weak justification for real follow-up. |
| 5 | Moderate | Plausible and potentially useful. Worth noting and revisiting if it connects to other observations. |
| 6 | Meaningful | Clearly worth additional inspection or targeted validation. Real candidate for follow-up. |
| 7 | High priority | Potentially important and reasonably credible. Should likely receive near-term follow-up. |
| 8 | Very high priority | Strong combination of plausibility, importance, and novelty or underappreciation. Should help drive the next study step. |
| 9 | Exceptional | Potentially discovery-relevant if validated. Deserves urgent, careful follow-up. |
| 10 | Top-tier | Rare, potentially field-shifting observation if real. Immediate focused follow-up strongly justified. |

Important rule:
- This is not a pure importance score.
- It is a score for how worthy the phenomenon is of further study.
- A phenomenon can be interesting in principle but score lower if the current support is weak.

When assigning a score, consider:
- is it likely real?
- is it important if real?
- is it novel, hidden, or underappreciated?
- does it connect multiple dots?
- is it actionable?
- could it redirect interpretation or research direction?

## Rules for manuscript scrutiny

When auditing a paper or figure set:
- do not trust the legend automatically
- do not assume representative means representative
- do not confuse polished figure design with evidentiary strength
- ask whether the figure really bears the argumentative load placed on it
- distinguish image persuasion from image evidence

Especially check:
- scale bars
- panel consistency
- matched controls
- stated sample sizes
- whether quantification matches the image impression
- whether a conclusion is broader than the displayed evidence

## Rules for generating new data

When working on fresh outputs:
- inspect the data before formalizing the story
- document unexpected phenomena, not just expected ones
- preserve raw and intermediate review artifacts when possible
- compare multiple plausible explanations
- rank observations before deciding what to chase

## Framework for evaluating existing information about a phenomenon

After observing and describing a phenomenon, review existing information about it in a disciplined way.

Possible sources include:
- prior manuscripts
- reviews
- atlases
- standard neuropathology knowledge
- textbooks or classic papers
- known technical caveats
- prior observations in the same workspace

Key questions:
- Has this phenomenon been described before?
- If yes, how consistently?
- Is the prior description direct or secondhand?
- Do the cited images or data in prior work actually support the claim?
- Is the phenomenon widely accepted because it is true, or because it is repeated?
- Is the prior literature internally consistent, mixed, or contradictory?
- Are there technical, sampling, or interpretive reasons the literature may be misleading?
- Does existing knowledge strengthen the importance of this observation, weaken it, or reframe it?

Suggested categories for existing-information assessment:
- **well-established and directly supported**
- **plausible and partly supported**
- **frequently asserted but weakly evidenced**
- **contested or inconsistent**
- **apparently novel or underdescribed**

Important rule:
- Existing information should contextualize the phenomenon, not overwrite the observation.
- Repeated claims are not the same as ground truth.

## Rules for literature-grounded thinking

Use literature, but do not let it dominate observation.

Literature should help with:
- naming a phenomenon
- framing its possible importance
- finding prior support or contradiction
- designing follow-up checks

Literature should not be allowed to:
- erase a real observation
- force a weak fit to a favored theory
- substitute citation density for ground truth

Much of the literature may be wrong, confounded, selective, or overclaimed. Always return to the observation.

## Role in the pipeline

This is the entry-point observational skill in the scientific-method stack.

Its job is to:
- inspect the material in front of you
- separate direct observation from interpretation
- identify candidate phenomena
- rank them by importance, reliability, and follow-up worthiness

It is not the question-formulation skill.
It is not the hypothesis skill.
It is not the experiment-design skill.
It is not the conclusion skill.

Its central question is:
- **What is actually present here, and which observed phenomena deserve further study?**

## Boundary

This skill should stop after producing a disciplined observational product.

It may:
- describe
- compare
- rank
- flag artifacts
- flag mismatches between evidence and claims
- identify high-priority follow-up phenomena

It should not:
- drift into full question-mapping
- generate broad causal models
- design a full experiment
- behave like a discussion section
- behave like a conclusion section

A minimal next discriminating observational check is appropriate.
A full hypothesis packet is not.

## Handoff in

This skill accepts raw or partially structured material.

### Ideal inputs
- histology figures
- pathology images
- WSI thumbnails
- ROI review sheets
- segmentation outputs
- contact sheets
- QC artifacts
- tables
- manuscripts
- draft figures
- preprints
- summary data with visual support

### Acceptable partial inputs
- figure legend without image
- methods/results mismatch concern
- user description of a strange pattern
- table without figures
- slide-level summary report

If inputs are incomplete, state that explicitly and reduce claim strength accordingly.

## Handoff out

The canonical output of this skill is:

# Observed Phenomena List

This is the formal handoff to `epistemic-cartographer`.

## Required output artifact structure

# Observed Phenomena List

## Material reviewed
- what was reviewed
- what was missing
- confidence in the review substrate

## Phenomenon 1
- direct observation
- possible interpretations
- alternative explanations or artifacts
- importance
- reliability
- further-study worthiness
- next discriminating observational check

## Phenomenon 2
- direct observation
- possible interpretations
- alternative explanations or artifacts
- importance
- reliability
- further-study worthiness
- next discriminating observational check

## Ranked follow-up candidates
- highest priority
- medium priority
- low priority

## Global artifact or confound concerns
- anything that may distort interpretation across the whole material set

## Observational bottom line
- what most deserves to be carried forward

## Entry modes

### 1. Native entry mode
Use when starting from raw material.

Examples:
- a new paper
- a new thumbnail cohort
- fresh pathology outputs
- a figure draft
- an exploratory image set

### 2. Mid-pipeline audit mode
Use when later-stage material needs to be re-observed.

Examples:
- a results section
- interpreted analysis output
- a draft discussion
- a draft conclusion

In this mode, act as a reality check:
- do the underlying data actually show what the downstream prose claims?

### 3. Sparse-input mode
Use when only partial material exists.

Examples:
- a table with no images
- a verbal report
- one representative panel
- one odd result

In this mode:
- explicitly mark what cannot be directly observed
- reduce claim strength
- still produce the best bounded observational pass possible

## Primary output goal

The clearest end-product of this skill is a ranked Observed Phenomena List.

Each phenomenon should be:
- described clearly and concretely
- separated from interpretation
- ranked by likely importance
- ranked by current reliability or truthfulness
- judged on whether it is worthy of further study

The main question at the end of an observational pass is:
- **Which observed phenomena deserve further study, and in what order?**

## Output style

When using this skill, outputs should usually separate:
1. **Phenomenon**
2. **Direct observations**
3. **Possible interpretations**
4. **Alternative explanations / artifacts**
5. **Importance ranking**
6. **Reliability ranking**
7. **Worthy of further study?**
8. **Next discriminating step**

When possible, conclude with a ranked list of candidate phenomena for follow-up, from highest-priority to lowest-priority.

This separation is important. Do not blur it.

## Common failure modes to avoid

- Explaining before observing
- Letting literature override ground truth
- Failing to notice discordant or inconvenient observations
- Confusing vivid images with strong evidence
- Overtrusting representative panels
- Treating a hypothesis as if it were an observation
- Failing to rank which observations might matter most
- Collapsing importance and reliability into one judgment
- Missing discovery because the phenomenon looked ordinary at first glance

## In this workspace

In this workspace, this skill should be used broadly, not narrowly.
It applies to:
- histology and pathology images
- digital pathology outputs
- computational review artifacts
- manuscripts and preprints
- cross-study comparison
- discovery triage

The standard is merciless because the goal is not comfort. The goal is to see clearly.
