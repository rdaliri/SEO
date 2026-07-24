<!--
File: README.md
Version: 7.0-corrected-final
Classification: required setup documentation
Authority: operational documentation, non-authoritative
Required or optional: Required for setup
Controller dependency: SEO_MASTER_CONTROLLER_LITE_v7.md
May override controller: No
Source provenance: v7 corrected release setup documentation
-->

# SEO Master System v7 — Lite / Daily Modular File-Aware Edition

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
| Intent, keyword architecture, entities, cannibalization | `modules/01_INTENT_ARCHITECTURE.md` |
| New content, refresh, brief, page copy | `modules/02_CONTENT_PRODUCTION.md` |
| Crawl, indexation, rendering, schema, accessibility | `modules/03_TECHNICAL_SEO.md` |
| Local pages or scaled page sets | `modules/04_LOCAL_AND_SCALED_CONTENT.md` |
| Refresh, merge, redirect, noindex, retire | `modules/05_CONTENT_LIFECYCLE.md` |
| Query fan-out, source eligibility, AI-search testing | `modules/06_AI_SEARCH_VISIBILITY.md` |
| Final specialist QA, repair, or compact verdict | `modules/07_QA_VERDICT.md` |
| Post-content image prompt package | `modules/08_IMAGE_GENERATION.md` |

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
The `archive/` directory is provenance storage only. Its contents are inactive and not dependencies.

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
7. For publishable content, load `modules/08_IMAGE_GENERATION.md`.
8. Run `modules/07_QA_VERDICT.md` as the specialist QA step.
9. Let the controller perform evaluation and issue the final verdict.

## Execution and QA Sequence
Lite controller initialization → canonical project context → required task modules → primary result → Module 08 image package when applicable → Module 07 compact QA → Lite controller verdict.

Module 08 creates the image prompt package; it does not replace content QA. Module 07 performs specialist QA or recovery; it never overrides the controller. The controller alone evaluates stop conditions and issues the final verdict.

## Publishable-Content Workflow
For publishable content:
1. Produce the content through the routed task module.
2. Create the image prompt package through `modules/08_IMAGE_GENERATION.md`.
3. Run `modules/07_QA_VERDICT.md` against the combined deliverable.
4. Apply controller evaluation, retries, stop conditions, and verdict rules.

If no image is relevant, record `Not applicable` and the reason.

## Operating Behavior
Lite reduces reporting depth, register length, iteration detail, and formatting overhead. It retains evidence-state discipline, unsupported-claim controls, critical-defect behavior, retry limits, stop conditions, conflict escalation, controller authority, final verdict behavior, and image handoff.

## Flat or Modular Usage Notes
Task modules are under `/modules`; nested-file discovery is required.
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
- Release: `7.0-corrected`
- Release date: `2026-07-24`
- Mode: `Lite / Daily`
- Format: `Modular File-Aware`
- Governance statement: v7 preserves the required v6 governance behavior, including evidence states, missing-data handling, defect severity, QA thresholds, retry limits, stop conditions, conflict escalation, controller verdict behavior, and image-generation handoff.
- Elite v4 specialist material is selectively adapted or retained as non-authoritative reference guidance. See `SOURCE_MANIFEST_v7.md`.
