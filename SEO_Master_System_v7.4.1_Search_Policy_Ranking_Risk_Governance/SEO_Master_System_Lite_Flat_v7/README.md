<!--
File: README.md
Version: 7.4.1-search-policy-ranking-risk-governance
Classification: required setup documentation
Authority: operational documentation, non-authoritative
Required or optional: Required for setup
Controller dependency: SEO_MASTER_CONTROLLER_LITE_v7.md
May override controller: No
Source provenance: v7 corrected release setup documentation
-->

# SEO Master System v7 — Lite / Daily Flat GPT Edition

## Package Purpose
This package runs production SEO tasks with one authoritative controller, explicit evidence handling, deterministic missing-data behavior, bounded retries, conflict escalation, image handoff, QA, and final verdict logic.

## Sole Controller
`SEO_MASTER_CONTROLLER_LITE_v7.md` is the only authoritative controller in this package. No module, reference file, README, playbook, legacy controller, or orchestration document may override it.

## Required Files
1. `SEO_MASTER_CONTROLLER_LITE_v7.md`
2. `CANONICAL_PROJECT_CONTEXT_LITE_v7.md`
3. Only the active task module or modules selected by the route map

`START_HERE.md` and this README are required setup documentation but are not controllers.

## Optional Active Modules
| Task | Exact file |
|---|---|
| Intent, keyword architecture, entities, cannibalization | `MODULE_01_INTENT_ARCHITECTURE.md` |
| New content, refresh, brief, page copy | `MODULE_02_CONTENT_PRODUCTION.md` |
| Crawl, indexation, rendering, schema, accessibility | `MODULE_03_TECHNICAL_SEO.md` |
| Local pages or scaled page sets | `MODULE_04_LOCAL_AND_SCALED_CONTENT.md` |
| Refresh, merge, redirect, noindex, retire | `MODULE_05_CONTENT_LIFECYCLE.md` |
| Query fan-out, source eligibility, AI-search testing | `MODULE_06_AI_SEARCH_VISIBILITY.md` |
| Final specialist QA, repair, or compact verdict | `MODULE_07_QA_VERDICT.md` |
| Post-content image prompt package | `MODULE_08_IMAGE_GENERATION.md` |
| Editorial humanization, batch similarity, detector-result governance | `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` |
| Search-policy compliance, ranking-risk prevention, diagnosis, recovery | `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md` |

## Reference-Only Files
- `REFERENCE_QUERY_FANOUT_AND_SOURCE_ELIGIBILITY_v7.md`
- `REFERENCE_CONTENT_STRUCTURE_PLAYBOOK_v7.md`
- `REFERENCE_CONTEXT_HANDLING_v7.md`
- `SOURCE_MANIFEST_v7.md`
- `SEO_V7_MIGRATION_REPORT.md`
- `IMAGE_PIPELINE_DEVELOPER_NOTE.md`

Reference files are optional, never controllers, cannot alter the output contract, and must not be loaded by default.

## Reference-Loading Triggers
| Reference file | Load only when | Do not use it for |
|---|---|---|
| `REFERENCE_QUERY_FANOUT_AND_SOURCE_ELIGIBILITY_v7.md` | AI-search research, query expansion, source analysis, citation eligibility, or platform-test design | General content work without AI-search research |
| `REFERENCE_CONTENT_STRUCTURE_PLAYBOOK_v7.md` | Selecting, comparing, or adapting a page or content structure | Routing, evidence classification, QA, or verdict governance |
| `REFERENCE_CONTEXT_HANDLING_v7.md` | Long-running projects, context compression, handoff preparation, or project-state cleanup | Creating unverified facts or overriding canonical context |

Loading all reference files by default is discouraged.

## Archive-Only Files
No archive directory is required in the flat release. Legacy files remain in controlled storage outside this active package.

## Files That Must Never Be Loaded Together
- Full and Lite controllers
- Flat and Modular copies of the same active system
- Any v4, v5, v6, Elite v4, or alternate v7 controller with this controller
- Legacy orchestration, mode-activation, or QA-governance prompts with v7
- Duplicate copies of the same task module

## Loading Order
1. Read `START_HERE.md`.
2. Load `SEO_MASTER_CONTROLLER_LITE_v7.md`.
3. Load `CANONICAL_PROJECT_CONTEXT_LITE_v7.md`.
4. Identify the task type using the route map.
5. Load only the required active module or modules.
6. Load one optional reference playbook only when its trigger applies.
7. Run Module 09 automatically when its Mode A/B/C trigger applies.
8. Run Module 10 when its automatic trigger applies before final QA.
9. For publishable content, load `MODULE_08_IMAGE_GENERATION.md`.
10. Run `MODULE_07_QA_VERDICT.md` as the specialist QA step.
11. Let the controller perform evaluation and issue the final verdict.

## Execution and QA Sequence
Lite controller initialization → canonical project context → required task modules → primary result → Module 09 when triggered → Module 10 when triggered → Module 08 when relevant → Module 07 compact QA → controller verdict.

Module 08 creates the image prompt package; it does not replace content QA. Module 07 performs specialist QA or recovery; it never overrides the controller. The controller alone evaluates stop conditions and issues the final verdict.

## Publishable-Content Workflow
For publishable content:
1. Produce the content through the routed task module.
2. Run Module 09 when editorial humanization or batch-comparison triggers apply.
3. Run Module 10 as the mandatory policy/ranking-risk gate.
4. Create the Module 08 image prompt package when an image is relevant.
5. Run Module 07 against the combined deliverable.
6. Apply controller evaluation, retries, stop conditions, and verdict rules.

If no image is relevant, record `Not applicable` and the reason.

## Operating Behavior
Lite reduces reporting depth, register length, iteration detail, and formatting overhead. It retains evidence-state discipline, unsupported-claim controls, critical-defect behavior, retry limits, stop conditions, conflict escalation, controller authority, final verdict behavior, and image handoff.

## Flat or Modular Usage Notes
All active files are at the package root.
- Flat is recommended for manual ChatGPT loading.
- Modular is recommended for repositories, APIs, IDEs, agents, and automation.
- Operational SEO rules must remain equivalent between Flat and Modular editions of the same mode.

## Troubleshooting and Conflict Handling
- Missing file: stop routing to that module and report the exact missing filename.
- Module/controller conflict: suspend only the conflicting module rule, apply the controller, log `MODULE_CONFLICT`, and follow the blocking-fact rule when unresolved.
- Missing blocking fact: follow the controller's continue, reduce-scope, bundled-question, or FAIL decision path.
- Reference conflict: ignore the conflicting reference guidance and follow the controller and active module.
- Duplicate controller detected: stop before execution and unload all but the selected package controller.

## Version and Provenance
- Release: `7.4.1`
- Release date: `2026-08-07`
- Mode: `Lite / Daily`
- Format: `Flat GPT`
- Governance statement: v7 preserves the required v6 governance behavior, including evidence states, missing-data handling, defect severity, QA thresholds, retry limits, stop conditions, conflict escalation, controller verdict behavior, and image-generation handoff.
- Elite v4 specialist material is selectively adapted or retained as non-authoritative reference guidance. See `SOURCE_MANIFEST_v7.md`.

## Module 09: Project Routing and Invocation

Load `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` when the project requires any of the following:

- a direct editorial humanization audit of one draft;
- comparison of three or more related pages or assets;
- investigation of repeated structures, phrases, CTAs, FAQs, disclaimers, headings, metadata, or near-duplicate paragraphs;
- review of supplied AI-detector screenshots, scores, percentages, or classifications;
- regulated or high-risk rewriting where factual, legal, medical, financial, or technical qualifiers must be preserved.

Do not load Module 09 for an unrelated single short task with no humanization, duplication, batch, or detector concern.

### Project Route Examples

| Project request | Required route |
|---|---|
| Humanize or audit one existing article | Controller → canonical context → `MODULE_02_CONTENT_PRODUCTION.md` when revision is required → `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` Mode A → `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md` → `MODULE_07_QA_VERDICT.md` → controller verdict |
| Create and audit one new article | Controller → canonical context → `MODULE_01_INTENT_ARCHITECTURE.md` when intent architecture is needed → `MODULE_02_CONTENT_PRODUCTION.md` → `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` Mode A → `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md` → `MODULE_07_QA_VERDICT.md` → controller verdict |
| Create or review a related content batch | Controller → canonical context → `MODULE_01_INTENT_ARCHITECTURE.md` → `MODULE_02_CONTENT_PRODUCTION.md` → `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` Mode B → `MODULE_04_LOCAL_AND_SCALED_CONTENT.md` when scaled/local risk applies → `MODULE_06_AI_SEARCH_VISIBILITY.md` when AEO/GEO applies → `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md` → `MODULE_07_QA_VERDICT.md` → controller verdict |
| Review supplied detector results for one or more assets | Run Mode A or Mode B first, then add Module 09 Mode C. Detector evidence is optional and never replaces the direct audit. |
| Audit local or scaled landing pages | Controller → canonical context → `MODULE_01_INTENT_ARCHITECTURE.md` → `MODULE_02_CONTENT_PRODUCTION.md` when copy is involved → `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` Mode B → `MODULE_04_LOCAL_AND_SCALED_CONTENT.md` → `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md` → `MODULE_07_QA_VERDICT.md` → controller verdict |

### Exact Project Invocation

After loading the selected controller, canonical project context, and required modules, use:

```text
Run Module 09 on the supplied project assets.

Select the execution mode from the actual scope:
- Mode A for one asset;
- Mode B for a related batch;
- add Mode C only when external detector evidence is supplied;
- use the combined route when both direct auditing and detector-result governance apply.

Perform the direct editorial or batch audit yourself. Do not require detector scores. Treat supplied detector results as non-authoritative evidence only, keep authorship NOT TESTED, preserve necessary qualifiers, revise root causes rather than swapping synonyms, and send unresolved defects to Module 07.
```

See `TEAM_MANUAL_MODULE_09.md` for intake requirements, team responsibilities, output templates, and worked execution prompts.


## v7.4 Module 10: Search Policy and Ranking-Risk Governance

Module 10 is an active module and is automatically routed for publication, indexation, scaled/local content, links, affiliate/review content, third-party hosted sections, structured data, migrations, redirects, expired domains, ranking drops, security issues, manual actions, recovery, and policy-compliance work.

It provides a mandatory cross-module gate for Google spam policies, people-first quality, technical eligibility, structured-data integrity, cross-engine controls, ranking-drop diagnosis, and prevention/recovery planning.

### Typical routes

- New article: Module 02 -> Module 10 -> Module 08 when relevant -> Module 07
- Related batch: Module 09 Mode B -> Module 04 -> Module 10 -> Module 07
- Technical/schema/security: Module 03 -> Module 10 -> Module 07
- Migration/recovery: Module 05 -> Module 03 -> Module 10 -> Module 07
- AI-search: Module 06 -> Module 10 when policy/eligibility applies -> Module 07

Do not issue publication-ready status when an applicable material policy category remains unresolved or untested.
