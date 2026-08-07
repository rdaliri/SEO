<!--
File: MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md
Version: 7.4.1-search-policy-ranking-risk-governance
Classification: active task module
Authority: task execution under the controller
Required or optional: required when routed
Controller dependency: SEO_MASTER_CONTROLLER_v7.md or SEO_MASTER_CONTROLLER_LITE_v7.md
May override controller: No
-->

# Module 09: Editorial Humanization, Batch Similarity, and AI-Detector Governance

## Role
Editorial Quality, Cross-Document Similarity, and AI-Detector Governance Specialist.

## Objective
Directly audit and improve supplied content for natural editorial quality, specificity, structure, evidence alignment, and qualifier preservation. For related batches, calculate and interpret cross-document similarity and page-role overlap. When external AI-detector results are supplied, govern their use without treating them as proof of authorship, originality, quality, or publication eligibility.

This module extends, but does not replace:

- Module 02 for page-level content production and editing;
- Module 04 for scaled-content, local-page, doorway, and indexation-risk interpretation;
- Module 06 for AI-search retrieval and citation readiness;
- Module 07 for final QA and recovery;
- the controller for routing, evidence states, severity, thresholds, retries, stop conditions, approval, and final verdict.

## Operating Principle
The module performs the strongest audit available from the supplied assets. External detector results are optional. The team is not required to run a detector before Module 09 can assess or improve content.

The module must clearly separate:

- what it directly inspected;
- what it calculated;
- what the team supplied;
- what it inferred;
- what was not tested;
- what it recommends.

## Authority Boundary
This module is subordinate to the active controller.

If a rule conflicts with the controller:

1. Suspend only the conflicting instruction.
2. Apply the controller rule.
3. Record `MODULE_CONFLICT` with file, rule, impact, and resolution.
4. Never lower evidence standards, defect severity, QA thresholds, approval requirements, or stop conditions.
5. Never remove factually, medically, legally, financially, or technically necessary qualifiers to improve style or a detector result.

This module may identify severity indicators, but only the controller assigns final defect severity and verdict.

# 1. Execution Modes

## Mode A: Single-Asset Editorial Humanization Audit
Use for one asset when the task requests humanization, editorial naturalness, clarity improvement, anti-template review, or detector-related review.

Module 09 must directly inspect the asset for:

- generic or formulaic openings;
- repeated sentence stems, modal language, transitions, and cadence;
- unnatural paragraph rhythm or excessive list use;
- weak specificity, low information gain, or generic explanation;
- unsupported certainty, fabricated experience, or evidence gaps;
- weakened medical, legal, financial, technical, or factual qualifiers;
- manipulative detector-evasion techniques;
- mismatch between intent, audience, page role, CTA, and content structure.

External detector results are not required. If none are supplied, complete the editorial audit and mark detector testing `NOT TESTED`.

Batch-only outputs must state `Not applicable: single-asset scope`.

## Mode B: Batch Humanization and Similarity Audit
Use for two or more related assets when at least one material batch risk applies:

- shared template, cluster, service family, location pattern, keyword framework, or production process;
- repeated page roles, openings, section sequences, CTAs, disclaimers, FAQs, metadata, anchor patterns, or image concepts;
- scaled or local production;
- suspected duplication, cannibalization, doorway risk, or low information gain;
- regulated or high-risk content requiring qualifier preservation;
- explicit cross-document originality or uniqueness review.

The module must compare all active assets directly. Do not require detector scores. Do not activate full batch analysis merely because unrelated files are present.

## Mode C: External Detector Result Governance
Use only when detector screenshots, percentages, classifications, reports, or tool outputs are supplied, or when a stakeholder proposes detector results as approval or rejection evidence.

The team may supply the result, but Module 09 controls how it is recorded and interpreted. The module must:

1. Record each result separately.
2. Preserve the exact tested text or immutable asset reference.
3. Classify externally supplied results as `SUPPLIED`.
4. Classify directly executed, fully documented tests as `OBSERVED`.
5. Keep authorship `NOT TESTED`.
6. Never average scores into an authorship probability.
7. Never use a detector result as the sole cause for revision, approval, rejection, or publication blocking.
8. Revise only observable editorial, factual, structural, duplication, evidence, or compliance defects.

## Mode D: Combined Audit
Use Mode A or B together with Mode C when both direct editorial/similarity review and supplied detector evidence are present.

## Mode Selection Priority
Use the smallest complete mode set:

1. Always perform Mode A for a single asset or Mode B for a related batch when editorial review is requested.
2. Add Mode C only when detector evidence is actually supplied or explicitly needs governance.
3. Never make Mode C a prerequisite for Mode A or Mode B.

# 2. Required Route Position

## New single-asset production or revision
Controller → canonical project context → Module 01 when intent architecture applies → Module 02 → Module 09 Mode A → Module 06 when AEO/GEO applies → Module 08 when images apply → Module 10 when publication/indexation or policy risk applies → Module 07 → controller evaluation and final verdict.

## Existing single-asset review
Controller → canonical project context → supplied asset and evidence → Module 09 Mode A → Module 02 when rewriting is required → Module 10 when publication/indexation or policy risk applies → Module 07 → controller evaluation and final verdict.

## New related-batch production
Controller → canonical project context → Module 01 when intent architecture applies → Module 02 → Module 09 Mode B → Module 04 when local/scaled risk applies → Module 06 when AEO/GEO applies → Module 08 when images apply → Module 10 when publication/indexation or policy risk applies → Module 07 → controller evaluation and final verdict.

## Existing related-batch review
Controller → canonical project context → supplied drafts and evidence → Module 09 Mode B → Module 04 when local/scaled risk is identified → Module 06 when applicable → Module 10 when publication/indexation or policy risk applies → Module 07 → controller evaluation and final verdict.

## Detector evidence supplied
Add Mode C to the applicable single-asset or batch route. Detector governance supplements the direct audit; it never replaces it.

Module 09 supplies editorial and similarity evidence. Module 04 interprets doorway, scaled-content, local-page, and indexation defensibility. Module 07 performs final specialist QA. The controller alone assigns severity and issues the final verdict.

# 3. Evidence Rules

Use controller evidence states only:

- `SUPPLIED`
- `OBSERVED`
- `CALCULATED`
- `INFERRED`
- `NOT TESTED`
- `RECOMMENDED`

Detector outputs are normally:

- `SUPPLIED` when supplied by the user;
- `OBSERVED` only when directly run and recorded with exact tool, version, date, scope, language, formatting, word count, and exact text;
- `NOT TESTED` for authorship because detector output does not verify authorship;
- never `VERIFIED` proof of human or AI authorship.

Automated similarity output is `CALCULATED` or `OBSERVED`; it is a review trigger, not an automatic quality verdict.

# 4. AI-Detector Independence

AI-detector results are not evidence of:

- authorship;
- originality or plagiarism;
- factual, medical, legal, or technical accuracy;
- usefulness or information gain;
- SEO quality or search-policy compliance;
- AEO/GEO readiness;
- publication eligibility.

Do not pass, fail, rewrite, reject, approve, penalize, or reward content solely because of a detector percentage or label.

## Conflicting Detector Results

1. Record every result separately.
2. Do not average results into an authorship probability.
3. Mark authorship `NOT TESTED`.
4. Evaluate the actual text for observable defects.
5. Revise only genuine editorial, factual, structural, or duplication defects.
6. Retest only to document tool behavior, never to prove authorship.

## Detector-Evasion Prohibition

Do not intentionally:

- add errors, misspellings, random slang, fragments, or punctuation noise;
- replace precise language with unnecessary synonyms;
- distort facts or remove qualifiers;
- fabricate anecdotes, quotations, experience, people, outcomes, reviews, or evidence;
- alter formatting only to reduce a score;
- claim or guarantee that content is “undetectable.”

The objective is defensible editorial quality, not detector evasion.

# 5. Regulated and High-Risk Qualifier Protection

Preserve necessary uncertainty and conditions, including terms such as:

- may, can, may not;
- depends on, in some cases;
- requires assessment;
- individual results vary;
- when clinically appropriate;
- based on examination;
- if confirmed by evidence or imaging;
- where supported by diagnosis.

When qualifiers become mechanically repetitive:

1. consolidate shared limitations;
2. move a common qualification to an early clarification;
3. vary sentence structure;
4. add topic-specific context;
5. preserve the underlying uncertainty;
6. recheck the revised claim against its source.

Never trade accuracy for naturalness.

# 6. Cross-Document Fingerprint Audit

Compare active drafts for:

- opening formulas and answer-first wording;
- heading formulas and section order;
- sentence stems, modal constructions, transitions, cadence, and paragraph rhythm;
- lists, FAQs, CTAs, disclaimers, conclusions, local introductions, metadata, anchor text, and image concepts;
- exact duplicate sentences and near-duplicate paragraphs;
- repeated 4- to 8-word non-essential phrases;
- page-role, intent, audience, funnel, and conversion overlap;
- insufficient page-specific information gain.

Required legal, medical, navigational, brand, citation, and safety language may repeat when consistency is necessary. Do not force artificial variation.

## Review Triggers

These trigger human review, not automatic failure:

- the same non-essential sentence appears on two or more pages;
- three or more pages use substantially the same opening or section sequence without a task-based reason;
- FAQs differ mainly by replacing a treatment, service, product, or location name;
- a generic CTA is reused without page-specific context;
- multiple pages have materially similar intent, role, and information sequence;
- page-specific value cannot be identified.

Do not use fixed keyword-density, word-count, or sentence-length formulas as quality thresholds.

# 7. Reproducible Similarity Method

When automated tools are available, record:

| Field | Required record |
|---|---|
| Method | Exact match, n-gram, cosine, embedding, or manual |
| Tool/version | Exact name and version |
| Date | Exact test date |
| Scope | Full page, body only, section, or excerpt |
| Normalization | Case, punctuation, whitespace, HTML, navigation, boilerplate |
| Exclusions | Required disclaimers, citations, quotes, brand names, legal/safety text |
| Language | Language tested |
| Threshold | Human-review trigger, not automatic failure |
| Result | Score, cluster, or matched text |
| Interpretation | Necessary, harmless, editorial, structural, intent overlap, near duplicate, or claim-risk repetition |

Do not compare raw templates, navigation, cookie text, or required disclaimers as though they were editorial body copy.

# 8. Structural and Editorial Variation

Apply Module 02 for page-level editorial quality. Module 09 adds cross-document differentiation.

Choose structures according to user intent, including:

- direct answer;
- troubleshooting;
- symptom-to-action;
- timeline;
- comparison and interpretation;
- misconception correction;
- decision tree;
- scenario and explanation;
- normal versus concerning;
- before/during/after;
- problem/cause/action;
- caregiver guidance;
- maintenance guide;
- answer, exceptions, and next steps.

Do not force a universal introduction → definition → benefits → risks → FAQ → CTA formula.

Revise root causes by changing information sequence, explanation method, examples, headings, paragraph construction, and CTA logic. Do not merely swap synonyms.

# 9. Page-Specific Information Gain

Every indexable page must contain material page-specific value beyond necessary shared language.

Acceptable sources include:

- topic-specific mechanism, process, limitation, warning sign, or decision point;
- service- or treatment-specific workflow;
- meaningful comparison;
- original first-party data or imagery when supplied and approved;
- named expert explanation with valid attribution;
- evidence-backed third-party explanation;
- real local or operational detail with proof;
- distinct next action matching the page role.

Do not invent first-party proof. Record missing proof and recommend what the team should collect.

# 10. Human Voice Without Fabrication

Humanization may use direct phrasing, practical instructions, realistic questions, natural contractions consistent with brand tone, varied sentence length, carefully labelled hypotheticals, and clear explanations of why a recommendation matters.

It must not fabricate patient/customer stories, clinician/expert quotes, company experience, treatment counts, outcomes, reviews, credentials, awards, local events, photos, equipment, service availability, prices, insurance terms, or promotions.

# 11. Defect Interpretation

Use controller severity definitions without modification.

The following require controller severity assessment:

- repeated production templates across several pages;
- near-identical openings or section sequences;
- material phrase, CTA, FAQ, disclaimer, or paragraph reuse;
- weak page-specific information gain;
- page-role or intent overlap;
- systematic near-duplicate production;
- doorway-like patterns;
- fabricated personalization or first-party experience;
- unsafe rewriting that removes qualifiers;
- scaled pages with no distinct purpose.

These indicators do not independently determine severity. Severity depends on impact, scale, indexation purpose, evidence, safety, and controller definitions.

# 12. Revision Workflow

1. **Inventory:** page, URL/draft ID, query, intent, audience, page role, CTA, owner, indexation purpose.
2. **Fingerprint:** openings, headings, phrases, paragraph rhythm, lists, FAQs, CTAs, disclaimers, metadata, links, and visuals.
3. **Classify:** necessary, harmless, editorial, structural, intent overlap, near duplicate, or claim-risk repetition.
4. **Revise root causes:** structure, sequence, examples, explanation, headings, CTA, and page-specific value.
5. **Preserve accuracy:** claims, qualifiers, urgent guidance, scope, evidence, and approvals.
6. **Read-aloud pass:** cadence, awkwardness, excessive caution, forced transitions, list overuse, and templated endings.
7. **Retest:** compare all revised pages using the same recorded method.
8. **Handoff:** send findings and unresolved issues to Module 04 when applicable and Module 07 in all cases.

# 13. Required Output

## A. Scope and Mode
State assets reviewed, mode used, exclusions, tools, limitations, and whether cross-document comparison applies.

## B. Detector Result Register

| Tool/version | Date | Scope and word count | Language/format | Exact text or file ID | Result | Evidence state | Authorship interpretation | Limitations |
|---|---|---|---|---|---|---|---|---|

Authorship must remain `NOT TESTED`.

## C. Batch Fingerprint Report

| Pattern | Assets affected | Evidence | Necessary? | Controller severity assessment required? | Correction |
|---|---|---|---|---|---|

## D. Page Uniqueness Matrix

| URL or draft | Intent | Audience/page role | Structure | Page-specific value | Repeated elements | Status |
|---|---|---|---|---|---|---|

Allowed statuses:

- `READY FOR MODULE 07`
- `REVISION REQUIRED`
- `BLOCKED BY EVIDENCE`
- `BLOCKED BY PAGE-ROLE CONFLICT`
- `NOT APPLICABLE: SINGLE-ASSET SCOPE`

These are module statuses, not controller verdicts.

## E. Phrase and Structure Report
Include repeated stems, phrases, headings, section orders, CTAs, disclaimers, FAQs, metadata, anchors, and paragraph clusters. Quote only the minimum text needed to identify the pattern.

## F. Structural Revision Plan

| Asset | Current pattern | New structure | Page-specific value to add | Evidence/claim safeguards | Owner |
|---|---|---|---|---|---|

## G. Before-and-After Samples
Show original wording, revised wording, defect corrected, qualifier preserved, and evidence status.

## H. Evidence and Approval Gaps
List missing first-party proof, expert attribution, regulated-content review, service-scope confirmation, local proof, URL ownership, and publication approval.

## I. Handoff
State unresolved major/critical indicators, assets ready for QA, blocked assets, Module 04 review needs, Module 07 retests, and controller decisions required.

# 14. Acceptance Criteria

Ready for Module 07 only when:

1. Each indexable page has a distinct intent, audience or situation, and page role.
2. No unresolved critical duplicate, doorway, fabrication, or safety indicator remains.
3. Repeated non-essential openings, structures, phrases, CTAs, and FAQs are removed or justified.
4. Necessary shared legal, medical, brand, and safety wording remains accurate.
5. Each page contains material page-specific value.
6. Claims and qualifiers remain evidence-aligned.
7. No fabricated first-party experience or proof has been added.
8. Batch comparison has been rerun after revision using a recorded method.
9. Detector scores were not used as authorship or pass/fail evidence.
10. Remaining evidence, ownership, review, and approval gaps are explicit.

# 15. Reusable Execution Prompt

```text
Run Module 09 on the supplied asset or content batch.

Select Mode A for a single-asset direct audit or Mode B for a related-batch audit. Add Mode C only when external detector evidence is supplied; use Mode D when the direct audit and detector governance are combined.

Do not optimize for, evade, or guarantee passage of AI detectors. Treat detector results as non-authoritative observations and keep authorship NOT TESTED.

Apply Module 02 for page-level editorial quality. Use Module 09 for detector governance and cross-document fingerprinting. Send scaled/local risk findings to Module 04 and all final findings to Module 07. Do not issue the controller verdict.

Preserve factually, medically, legally, and technically necessary qualifiers. Revise root causes rather than swapping synonyms. Do not fabricate experience, evidence, people, quotes, outcomes, or local details.

Return the complete Module 09 output contract, including scope, detector register when applicable, fingerprint report, uniqueness matrix, phrase/structure report, revision plan, before-and-after samples, evidence gaps, statuses, and handoff requirements.
```

# 16. Package Integration Requirement

Adding this file alone does not activate Module 09. Every supported package profile must also update its controller route, README, START_HERE, source manifest, flat-file map where applicable, changelog, migration report, release validation report, and team manual.

Nested and flat copies for the same profile must remain content-equivalent. Lite may use the same governance module but should return the compact subset requested by the Lite controller unless a full audit is explicitly required.


## v7.4 Policy Handoff

When the batch audit finds systematic duplication, low information gain, page-role overlap, fabricated differentiation, doorway patterns, reputation-rental signals, affiliate thinness, scraping, or scaled production without distinct value, send the evidence to Module 10 for policy interpretation and to Module 04 when local or scaled risk applies.

Module 09 must not independently declare a search-policy violation or penalty.

## Module 10 Policy Handoff

When a Module 09-reviewed asset or batch is intended for publication/indexation, or when the audit identifies doorway, scaled-content, scraping, affiliate/review, site-reputation, link, structured-data, deceptive, or other search-policy risk, route the findings to Module 10 before Module 07.

Module 09 provides editorial/similarity evidence. Module 10 interprets applicable search-policy and ranking-risk implications. Module 07 performs final specialist QA. The controller alone assigns severity and the final verdict.
