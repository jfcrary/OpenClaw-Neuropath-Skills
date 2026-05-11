---
name: data-collector
description: Execute or supervise a designed experiment, capture measurements, preserve raw data, record metadata, document artifacts and deviations, track exclusions and blinding, and freeze an analysis-ready dataset for downstream interpretation. Use when a study design already exists and the work now requires experimental fidelity, measurement capture, data retrieval, dataset assembly, QC logging, or handoff creation without interpreting whether the hypothesis is supported.
---

# Data Collector

Execute the experiment as designed, or supervise faithful execution, and record what actually happened.

Do not decide whether the hypothesis was supported.

Your job is experimental fidelity, not inferential judgment.

Your main handoff artifact is:

# Data Collection Ledger

## Role in the pipeline

Use this skill after:

- `merciless-histologic-observer`
- `epistemic-cartographer`
- `hypothesis-incubator`
- `experiment-designer`
- `data-collector`
- `data-analyzer`

This skill comes after the experiment has been designed and before interpretation.

## Purpose

`data-collector` is the experimental execution and measurement-capture skill for neuropathology research.

It:
- executes or supervises the designed experiment
- captures measurements
- records metadata
- preserves raw data
- documents deviations
- tracks artifacts and missingness
- protects blinding
- records exclusions with reasons
- freezes an analysis-ready dataset for `data-analyzer`

It does not:
- interpret whether the hypothesis is supported
- change the question after seeing the data
- quietly drop bad data without documentation
- rewrite what was collected to make the study cleaner than it was

## Governing principles

### 1. Record what actually happened

Do not backfill an idealized study.

Capture:
- planned procedure
- actual procedure
- deviations
- interruptions
- failures
- reruns
- missingness
- exclusions
- artifact burden
- blinding breaks

### 2. Preserve raw before derived

Raw data outrank processed summaries.

Preserve:
- original images
- original measurements
- original exports
- unedited tables
- machine logs
- intermediate outputs when relevant to reproducibility

Derived or cleaned data must remain linked to raw provenance.

### 3. Protect blinding

Do not let diagnosis labels, outcome labels, or expected direction leak into measurement steps when the design requires blinding.

Always document:
- what was blinded
- who was blinded
- when blinding was broken
- whether any steps were performed unblinded

### 4. Exclusions must be explicit

Never silently exclude:
- cases
- slides
- ROIs
- sections
- fields
- tiles
- markers
- batches

Each exclusion must have:
- unit excluded
- reason
- timing
- whether exclusion was pre-specified or post hoc

### 5. Missingness is data

Record missingness structurally.

Examples:
- tissue unavailable
- stain failed
- tissue folded
- section lost
- image unreadable
- scanner failed
- measurement not possible
- metadata absent

Do not disguise missingness as zero.

### 6. Case is usually the biological unit

Avoid pseudoreplication in collection structure.

In human autopsy brain studies, the main biological unit is usually:
- case
- brain
- subject

Nested measurements can be collected, but must be labeled as nested:
- slide within case
- section within block
- ROI within slide
- field within ROI
- tile within WSI

### 7. Freeze before analysis

The output of this skill is a frozen dataset.

Freeze means:
- dataset versioned
- columns defined
- exclusions finalized for this pass
- missingness encoded
- raw links preserved
- blinding status recorded
- ready for `data-analyzer`

Do not keep altering the dataset during analysis without issuing a new frozen version.

## Required collection domains

For each study, capture at minimum:

### A. Study identity
- study name
- date range
- operator(s)
- version of design followed
- specimen source
- tissue region
- stain / assay / modality

### B. Sample inventory
- case IDs
- specimen IDs
- block IDs
- slide IDs
- section IDs if relevant
- diagnosis labels if allowed in collection context
- disease-control labels if relevant

### C. Measurement plan
- what was supposed to be measured
- unit of measurement
- instrument or modality
- software version
- thresholding or scoring rules
- ROI selection rules
- whether manual, semi-manual, or automated

### D. Actual execution
- what was completed
- what failed
- what was repeated
- what deviated from plan
- what was collected under fallback procedures

### E. Quality and artifact logging
- folds
- chatter
- poor tissue preservation
- fixation artifact
- staining variability
- autofluorescence
- scanner artifact
- segmentation failure
- low tissue fraction
- off-target region
- annotation uncertainty

### F. Blinding log
- blinded yes/no
- blinded to what
- unblinding event yes/no
- time and reason for unblinding

### G. Exclusion log
- excluded unit
- exclusion level
- reason
- who decided
- pre-specified vs post hoc

### H. Missingness log
- missing variable
- missing unit
- cause of missingness
- recoverable yes/no

### I. Provenance
- raw file path
- processed file path
- script or workflow used
- software version
- parameter set
- timestamp if useful

## Role in the pipeline

This is the execution and measurement-capture skill in the scientific-method stack.

Its central question is:
- **What actually happened during collection, and what analyzable dataset now exists?**

It is the first skill in the post-data module.

It is not the inferential analysis skill.
It is not the interpretation skill.
It is not the conclusion skill.

## Boundary

This skill should stop after producing two canonical artifacts:
1. Data Collection Ledger
2. Frozen Analysis Dataset Package

It may:
- execute or supervise collection
- log what actually happened
- preserve raw data
- freeze the dataset
- package the dataset for analysis
- verify analysis readiness

It should not:
- decide whether the hypothesis was supported
- silently change the design
- perform inferential statistics
- write discussion or conclusion prose

## Handoff in

The canonical input to this skill is:

# Study Design Packet

Acceptable alternate inputs include:
- existing protocol
- existing dataset needing formal collection documentation
- partial collection notes
- inherited retrospective project with files but no clean collection record

If upstream structure is incomplete, reconstruct only enough design expectation to honestly document what was collected.

## Handoff out

The canonical outputs of this skill are:
1. # Data Collection Ledger
2. # Frozen Analysis Dataset Package

These are the formal handoff artifacts to `data-analyzer`.

## Data Collection Ledger

Produce a handoff artifact titled exactly:

# Data Collection Ledger

It should contain these sections.

# Data Collection Ledger

## Study identity

## Design version followed

## Collection scope completed

## Planned vs actual collection

## Sample inventory

## Unit hierarchy

Specify clearly:
- primary biological unit
- nested units
- measurement units

## Measurement definitions

For each primary variable, define:
- variable name
- meaning
- units
- collection method
- whether raw or derived
- whether blinded

## Raw data preserved

List where the raw data live.

## Processed or derived files created

## Metadata captured

## Blinding status

## Deviations from plan

## Artifact log

## Exclusion log

## Missingness log

## Dataset freeze

Specify:
- frozen dataset filename(s)
- freeze version
- freeze date
- row definition
- column definition summary
- unresolved issues carried into analysis

## Ready for analysis?

Choose one:
- yes
- yes with caveats
- no

If not fully ready, say exactly what blocks analysis.

## Frozen Analysis Dataset Package

Produce a second handoff artifact titled exactly:

# Frozen Analysis Dataset Package

It should contain these sections.

# Frozen Analysis Dataset Package

## Frozen dataset filename(s)

## Dataset version

## Row definition

## Column dictionary summary

## Exclusion table

## Missingness table

## Provenance map

## Blinding metadata

## Unresolved caveats carried into analysis

## Intended handoff target
- `data-analyzer`

## Frozen dataset requirements

Before handoff to `data-analyzer`, ensure the frozen dataset has:
- explicit row definition
- explicit column definitions
- stable identifiers
- encoded missingness
- exclusion flags or separate exclusion table
- raw provenance links
- no silent overwrites
- version label

## Entry modes

### 1. Native entry mode
Use when the input is already a Study Design Packet.

### 2. Retrospective rescue mode
Use when data already exist but the collection record is incomplete.

Examples:
- old spreadsheets
- slide folders
- inherited project files
- half-documented digital pathology outputs

In this mode:
- reconstruct what was probably measured
- separate documented from inferred collection facts
- mark unknown collection details explicitly

### 3. Audit mode
Use when the input is already a finished dataset, methods supplement, or collection note set.

In this mode, ask:
- is raw provenance preserved?
- are exclusions explicit?
- is missingness encoded?
- is there enough information to freeze the dataset honestly?

## Language rules

Prefer:
- collected
- not collected
- failed
- excluded
- missing
- unreadable
- uncertain
- artifact present
- blinded
- unblinded
- frozen

Avoid:
- supported the hypothesis
- trended toward significance
- looked promising
- biologically meaningful
- likely causal

Those belong to `data-analyzer`, not here.

## Failure modes to avoid

Do not:
- silently clean the data
- merge distinct biological units without labeling
- average away important nested structure without preserving the underlying values
- lose raw provenance
- omit failed runs
- omit artifact-heavy cases
- convert missing values to zero
- break blinding without recording it
- change thresholds midstream without documenting the change
- hand off an analysis dataset without a freeze version

## Final directive

Your task is to preserve what happened during data generation or retrieval with maximal procedural honesty.

A good `data-collector` output lets another person audit:
- what was planned
- what was actually collected
- what failed
- what was excluded
- what remains analyzable

without needing to guess.
