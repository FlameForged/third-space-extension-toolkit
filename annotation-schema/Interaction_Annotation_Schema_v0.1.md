# Interaction Annotation Schema v0.1

**Author:** Rachelle Siemasz  
**Status:** Conceptual coding framework; not empirically validated  
**Purpose:** To support structured qualitative annotation of human–AI interaction transcripts relevant to third-space extension.

## 1. Unit of Analysis

The default unit is an **interaction event**: a bounded passage in which the human, the AI, or the relation between them performs a function relevant to the recursive loop.

Annotators may code:

- a single message
- part of a message
- a paired human–AI exchange
- a short multi-turn sequence when the event cannot be understood from one turn alone

Multiple codes may be applied to the same event.

## 2. Core Event Codes

### EXT — Externalization

The human expresses an incomplete cognitive structure for development within the interaction.

Examples:

- tentative hypothesis
- partial synthesis
- unresolved contradiction
- early conceptual distinction
- pattern offered for testing

**Exclude:** fully specified requests for simple retrieval or formatting.

### AMP — Amplification

The AI expands, elaborates, or enriches the user’s material without substantially reorganizing its structure.

**Indicators:** added examples, implications, associations, or detail that remain aligned with the original project.

### RES — Restructuring

The AI reorganizes, reframes, formalizes, or transforms the externalized material in a way that changes its usable structure.

**Distinguish from AMP:** amplification adds; restructuring changes organization or conceptual form.

### SYN — Creative Synthesis

A novel combination, cross-domain connection, or conceptual integration emerges within the interaction.

**Code only when:** the synthesis is relevant to the user-directed project and not merely decorative analogy.

### MTI — Multi-Threaded Integration

The interaction successfully maintains and relates two or more conceptual threads that would otherwise be difficult to track simultaneously.

### MPR — Meta-Cognitive Pattern Recognition

The human or AI identifies a recurring pattern in the reasoning process, interaction history, project structure, or model behavior.

### HEV — Human Evaluation

The human explicitly assesses the model output for accuracy, relevance, coherence, precision, usefulness, or fit with the project.

### ACC — Selective Acceptance

The human explicitly incorporates or endorses part of the model’s contribution.

### REJ — Selective Rejection

The human explicitly rejects part or all of the model’s contribution.

### REV — Human Revision

The human modifies the returned material before reintegration.

### REX — Re-Externalization

The human returns a revised cognitive structure to the system, initiating another cycle.

## 3. Boundary and Correction Codes

### DFT — Drift

The interaction departs from the user’s intended question, conceptual thread, evidentiary standard, or project goal.

Subtypes may include:

- `DFT-TOPIC` — topic deviation
- `DFT-GOAL` — goal substitution
- `DFT-CONCEPT` — conceptual flattening or distortion
- `DFT-STYLE` — stylistic substitution that changes the claim
- `DFT-NORM` — imported evaluative standard or framework

### HAL — Hallucination or Unsupported Claim

The AI introduces a false, unverifiable, fabricated, or insufficiently supported factual claim.

### OVG — Overgeneralization

The AI extends a claim beyond the scope supported by the user’s evidence or framing.

### BAS — Boundary Assertion

The human explicitly states or restores a boundary concerning goals, claims, wording, evidence, method, or interpretive limits.

### COR — Corrective Feedback

The human identifies an error, drift, incoherence, unsupported claim, or loss of thread and directs the system to correct it.

### RC — Radical Candor Event

A direct, explicit correction that both identifies the problem and reasserts the user’s evaluative authority.

**Minimum threshold:** the event must contain both diagnosis and directional correction.

### RSP — Correction Responsiveness

The AI acknowledges and meaningfully incorporates human correction.

Values:

- `RSP-0` — ignores correction
- `RSP-1` — acknowledges but does not repair
- `RSP-2` — partially repairs
- `RSP-3` — successfully repairs and restores thread

### BRS — Boundary Restoration

The interaction returns to the user’s intended goals, distinctions, or standards after a correction event.

### LCP — Loop Collapse

The recursive process breaks down because drift, repeated error, generic output, unresponsiveness, or loss of trust prevents useful reintegration.

## 4. Redistribution Candidate Codes

### TCT — Transformative Contribution

The model contribution becomes causally important to the subsequent development of the user’s thought rather than merely adjacent or optional.

### RIN — Recursive Reintegration

Model-transformed material is selectively incorporated into the user’s ongoing cognitive project and used in a later cycle.

### UGN — User-Governed Norms

The user’s standards of coherence, relevance, evidence, and precision visibly govern what is retained or rejected.

### UGA — User Goal Authorship

The user remains the source of the project’s purpose and direction.

### FUP — Functional Uptake

The user employs the transformed material as part of reasoning, writing, design, analysis, or decision-making.

### CRE — Candidate Redistribution Event

An event or sequence satisfies enough of the following indicators to warrant closer analysis:

1. user-directed cognitive project
2. transformative model contribution
3. explicit human evaluation
4. selective acceptance, rejection, or revision
5. recursive reintegration
6. functional uptake
7. continued human goal authorship

`CRE` is a flag for analysis, not proof that cognitive redistribution occurred.

## 5. Loop Health Dimensions

Annotators may record each dimension at the cycle or session level using a 0–3 provisional scale.

### Goal Continuity

- `0` — goal lost or replaced
- `1` — substantial deviation
- `2` — mostly preserved with correction
- `3` — stable throughout

### Thread Preservation

- `0` — central threads lost
- `1` — multiple important omissions
- `2` — minor losses or recoverable drift
- `3` — key threads maintained and integrated

### Human Evaluative Control

- `0` — passive acceptance or model-led direction
- `1` — limited evaluation
- `2` — active but inconsistent evaluation
- `3` — explicit, continuous human governance

### Correction Effectiveness

- `0` — correction ignored
- `1` — acknowledged without meaningful repair
- `2` — partial restoration
- `3` — successful restoration of coherence

### Recursive Reintegration

- `0` — no meaningful reintegration
- `1` — superficial reuse
- `2` — partial integration into the project
- `3` — transformed material becomes functionally important in later cycles

## 6. Annotation Record Template

For each coded event, record:

| Field | Description |
|---|---|
| Event ID | Unique identifier |
| Session ID | Parent interaction or transcript |
| Turn range | Relevant human and AI turns |
| Speaker | Human, AI, or interaction-level |
| Primary code | Main event code |
| Secondary codes | Additional applicable labels |
| Evidence excerpt | Minimal passage supporting the code |
| Annotator note | Why the code applies |
| Confidence | Low, medium, or high |
| Drift repaired? | Yes, no, partial, or not applicable |
| Reintegration observed? | Yes, no, unclear, or not applicable |

## 7. Coding Principles

- Code observable interactional evidence rather than inferred mental states.
- Do not treat fluent language as evidence of understanding.
- Distinguish model contribution from human uptake.
- Do not code redistribution solely because the user reports a feeling of partnership.
- Preserve uncertainty when causal importance is unclear.
- Use `CRE` only as a candidate flag requiring qualitative interpretation.
- Record negative and failed cases as carefully as successful ones.

## 8. Current Limitations

This schema has not undergone:

- inter-rater reliability testing
- construct validation
- discriminant validation against ordinary assistance
- cross-platform testing
- multi-population evaluation

It is offered as a reusable starting point for exploratory research and future instrument development.
