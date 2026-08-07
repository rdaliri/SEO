# Team Manual: Module 09 Editorial Humanization and Detector Governance

Version: 7.4.1-search-policy-ranking-risk-governance
## Purpose
Use this manual to run direct editorial audits, batch-similarity reviews, and optional detector-result governance without confusing detector scores with evidence of authorship or quality.

## Core Rule
Module 09 performs the strongest audit available from the supplied content. The team does not need to obtain an AI-detector score before requesting review.

## Responsibility Model

| Responsibility | Owner |
|---|---|
| Supply drafts, source evidence, page roles, and business constraints | Content team |
| Directly inspect writing quality, structure, specificity, claims, and qualifiers | Module 09 |
| Calculate and interpret cross-document repetition and similarity | Module 09 |
| Supply proprietary detector reports when the team wants them included | Content team, optional |
| Record and govern detector results | Module 09 |
| Interpret scaled/local/doorway risk | Module 04 |
| Perform final QA | Module 07 |
| Assign severity and final verdict | Controller |

## Package Selection

| Situation | Package |
|---|---|
| Routine page editing, small batch, fast operational review | Lite |
| Regulated/YMYL content, large batch, formal audit, migration, dispute, or release approval | Full |
| Target tool cannot resolve folders | Flat variant |
| Target tool supports folders and relative paths | Nested variant |

Do not mix controllers, modules, or maps from different variants.

## Select the Correct Mode

### Mode A: Single-Asset Editorial Humanization Audit
Use for one article, landing page, service page, FAQ, description, or other content asset requiring editorial improvement or detector-related review.

Module 09 performs the audit directly. Detector results are optional.

### Mode B: Batch Humanization and Similarity Audit
Use for two or more related assets when shared production patterns, duplication, page-role overlap, scaled content, local pages, or weak differentiation may exist.

### Mode C: External Detector Result Governance
Add only when the team supplies detector screenshots, percentages, labels, or reports, or when a stakeholder wants to use detector output as approval evidence.

### Mode D: Combined Audit
Use Mode A or B with Mode C when detector evidence is supplied alongside content.

## What the Team Must Supply

### Required for every audit

- exact content assets or immutable file references;
- target audience and dominant intent;
- page role and intended CTA;
- source evidence and required claims;
- brand, legal, medical, financial, technical, or compliance constraints;
- required shared disclaimers or standard language.

### Additional inputs for batch review

- URL or draft ID for every asset;
- target query or topic;
- indexation purpose;
- commercial owner;
- known internal-link and metadata plan;
- any content intentionally shared across pages.

### Optional detector inputs

- tool name and version;
- test date;
- exact text or file tested;
- full-document or excerpt scope;
- word count and language;
- formatting used;
- score or classification;
- screenshot, export, or report ID;
- whether the text changed after testing.

Missing information must be recorded, not guessed.

## Standard Workflow

1. Choose Full or Lite and Flat or Nested.
2. Load the matching controller.
3. Load the matching canonical project context.
4. Supply content, evidence, page roles, and constraints.
5. Run Module 02 when content production or rewriting is required.
6. Run Module 09 Mode A for one asset or Mode B for a related batch.
7. Add Mode C only when detector evidence is supplied.
8. Run Module 04 when local, scaled, doorway, or indexation-purpose risk exists.
9. Run Module 06 when AEO/GEO or citation-readiness review applies.
10. Run Module 08 when publishable image specifications are relevant.
11. Run Module 07 for final QA.
12. Let the controller assign severity and issue the final verdict.

## Copy-Paste Prompt: Single Asset

```text
Load the active controller, canonical project context, Module 02 when rewriting is required, Module 09 in Mode A, and Module 07.

Directly audit the supplied asset for generic openings, repeated sentence patterns, unnatural cadence, excessive list use, weak specificity, low information gain, unsupported certainty, evidence gaps, fabricated experience, qualifier loss, and mismatch between intent, audience, page role, CTA, and structure.

Do not require or simulate an AI-detector score. When no detector result is supplied, mark detector testing NOT TESTED. Preserve all medically, legally, financially, technically, and factually necessary qualifiers. Revise observable root causes rather than swapping synonyms.

Return all single-asset Module 09 outputs. Mark batch-only sections Not applicable: single-asset scope. Hand off to Module 07. The controller alone issues the final verdict.
```

## Copy-Paste Prompt: Related Batch

```text
Load the active controller, canonical project context, Module 02, Module 09 in Mode B, Module 04 when scaled/local risk applies, Module 06 when AEO/GEO applies, Module 08 when images apply, and Module 07.

Inventory and compare every supplied asset. Directly audit openings, headings, section order, sentence stems, phrases, cadence, paragraph rhythm, lists, FAQs, CTAs, disclaimers, metadata, anchors, image concepts, intent, audience, page role, indexation purpose, and page-specific information gain.

Exclude required legal, medical, financial, technical, safety, citation, navigation, and brand wording from false duplicate findings. Record the comparison method, normalization, exclusions, and thresholds as human-review triggers only. Revise structures and explanations, not just vocabulary. Preserve evidence-aligned qualifiers and never fabricate first-party proof.

Return the complete Module 09 batch output contract, Module 04 handoff where needed, Module 07 handoff, and no final controller verdict.
```

## Copy-Paste Prompt: Detector Evidence Included

```text
Run the applicable Module 09 direct audit mode and add Mode C for the supplied detector evidence.

Record each detector result separately with tool, version, date, exact tested text or immutable asset reference, scope, word count, language, formatting, result, and known limitations. Mark externally supplied results SUPPLIED and authorship NOT TESTED. Do not average scores, guarantee detector passage, or use detector output as pass/fail evidence.

Complete the editorial or batch-similarity audit independently. Recommend changes only for observable editorial, factual, structural, duplication, evidence, or compliance defects. Preserve necessary qualifiers and prohibit detector-evasion tactics.
```

## How to Read Detector Results

| Detector output | Correct interpretation |
|---|---|
| “90% AI” | Tool observation only; authorship remains NOT TESTED |
| “Human” | Not proof of human authorship, originality, or quality |
| Tools disagree | Record separately; do not average |
| Score changes after editing | Not proof the edit improved; inspect the content |
| Client demands 0% AI | No reliable guarantee; use editorial and evidence QA |
| No detector supplied | Complete the direct audit; mark detector testing NOT TESTED |

## Prohibited Actions

- requiring a detector score before reviewing content;
- pretending a proprietary detector was run when it was not;
- adding mistakes, slang, fragments, or punctuation noise to manipulate a score;
- removing medical, legal, financial, technical, or factual qualifiers;
- fabricating anecdotes, quotes, reviews, experience, outcomes, credentials, or local details;
- approving or rejecting content solely because of a detector result;
- treating similarity calculations as automatic proof of low quality;
- forcing unnecessary variation in required shared language.

## Reviewer Decision Guide

| Finding | Action |
|---|---|
| No detector result supplied | Perform direct audit; mark detector testing NOT TESTED |
| Required disclaimer repeats | Keep; classify as necessary repetition |
| Generic opening repeats | Rewrite around the distinct user task |
| Same CTA across funnel stages | Create page-role-specific CTAs |
| Same section sequence without reason | Rebuild around intent |
| Near-duplicate local pages | Send to Module 04 |
| Qualifier repetition sounds robotic | Consolidate wording while preserving uncertainty |
| Missing first-party proof | Record the gap; never fabricate substitute proof |
| Detector score is the only concern | Do not rewrite unless observable defects exist |

## Approval Checklist

- [ ] Correct package variant and controller loaded
- [ ] Mode A or B selected for the direct audit
- [ ] Mode C added only when detector evidence exists
- [ ] Exact assets and scope recorded
- [ ] Detector authorship marked NOT TESTED
- [ ] Similarity method and exclusions recorded when applicable
- [ ] Necessary shared wording excluded from false positives
- [ ] Every indexable page has distinct value and role
- [ ] Claims and qualifiers remain evidence-aligned
- [ ] No fabricated proof or experience added
- [ ] Module 04 handoff completed where applicable
- [ ] Module 07 final QA completed
- [ ] Controller issued the final verdict

## File Locations

Nested Full: `modules/09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md`

Nested Lite: `modules/09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md`

Flat Full/Lite: `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md`

This manual is `TEAM_MANUAL_MODULE_09.md` in every package variant.

## Module 10 Handoff

For content intended for publication/indexation, or when Module 09 identifies search-policy or ranking-risk indicators, send the Module 09 findings to Module 10 before final Module 07 QA. The team does not need to request this manually; the controller should route it automatically.
