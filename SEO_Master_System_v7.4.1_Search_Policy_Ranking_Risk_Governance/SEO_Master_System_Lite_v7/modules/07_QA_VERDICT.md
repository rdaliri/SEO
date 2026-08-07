<!--
File: 07_QA_VERDICT.md
Version: 7.4.1-search-policy-ranking-risk-governance
Classification: active task module
Authority: task execution under the controller
Required or optional: required when routed
Controller dependency: SEO_MASTER_CONTROLLER_LITE_v7.md
May override controller: No
Source provenance: v7 QA module with explicit SEO, AEO, GEO, and humanization acceptance checks
-->

# Module 07: QA and Verdict

## Objective
Apply the controller rubric, repair recoverable defects, and issue a traceable verdict.

## Rules
1. Use the controller's evidence, severity, retry, stop, and conflict rules without modification.
2. Validate factual support, intent, usefulness, architecture, internal links, technical status, scaled-content risk, and conversion alignment.
3. Auto-correct only when no new facts, approvals, or strategy changes are required.
4. Fix root causes before surface polish.
5. Never mark a recommendation as implemented or verified without direct evidence.

## Deliverable
Use the controller's compact output contract: corrected result, control log, score, defect counts, iterations, verdict, and unresolved next actions.

## v7 Specialist Guidance
- Apply only the controller rubric, severity definitions, retry limits, and verdict rules.
- Recovery must identify the defect, evidence, correction, retest, and residual risk.
- Never import Elite v4 severity, approval, or orchestration rules when they conflict with the controller.

## Humanization and Answer-Quality Acceptance Checks

Before issuing the specialist QA result, verify:

### Humanization
- No generic or padded opening delays the useful content.
- No filler transitions, repetitive conclusions, or templated closing remain.
- Sentence and paragraph rhythm show natural variation.
- Lists are used selectively rather than mechanically.
- Repetitive syntax, repeated sentence stems, and excessive parallelism are removed.
- Tone matches audience, page type, intent, funnel stage, and supplied brand voice.
- Abstract claims use concrete supplied or verified examples when evidence permits.
- The final editorial pass returns `PASS`.

### AEO
For answer-seeking queries:
- the direct answer appears first,
- the opening answer block is self-contained,
- the answer matches the exact query,
- short direct questions receive concise answers,
- unsupported or conditional answers state their limitations,
- later detail does not contradict the opening answer.

### GEO
- Freshness notes are present when recency materially affects the topic.
- Expert or reviewer attribution is recommended when credibility depends on expertise.
- Missing first-party proof is converted into a collection action or clearly labeled evidence substitution.
- Citation-readiness is checked claim by claim for material statements.
- AI-search readiness is not approved when recency or credibility requirements remain unresolved.

Any material failure in these checks is a major defect unless it creates a critical integrity, safety, or compliance problem.


## v7.4 Compact Search Policy Compliance Gate

Before `PASS`, run Module 10 when the output is intended for publication, indexation, migration, scaled deployment, structured data, link work, or recovery.

Return for each applicable category: `PASS`, `FAIL`, `NOT APPLICABLE`, or `NOT TESTED`.

Do not pass when a material applicable category is unresolved. Do not call a ranking decline a penalty without direct evidence. Do not guarantee rankings, recovery, rich results, Discover visibility, or AI citations.
