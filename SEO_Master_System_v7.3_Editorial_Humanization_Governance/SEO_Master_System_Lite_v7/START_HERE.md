<!--
File: START_HERE.md
Version: 7.0-corrected-final
Classification: required setup documentation
Authority: operational documentation, non-authoritative
Required or optional: Required for setup
Controller dependency: SEO_MASTER_CONTROLLER_LITE_v7.md
May override controller: No
Source provenance: v7 corrected release setup documentation
-->

# START HERE — Lite v7 Modular

## Load in This Order
1. Load the sole controller: `SEO_MASTER_CONTROLLER_LITE_v7.md`.
2. Load the canonical project context: `CANONICAL_PROJECT_CONTEXT_LITE_v7.md`.
3. Identify the task type using the route map in `README.md`.
4. Load only the required active task module or modules.
5. Load an optional reference playbook only when its documented trigger applies.
6. For publishable content, include `modules/08_IMAGE_GENERATION.md` for the image-generation handoff.
7. Run `modules/07_QA_VERDICT.md` for specialist QA, then let the controller issue the final verdict.
8. Do not load archived files, competing controllers, or Flat and Modular copies together.

## Common Loading Examples
| Request | Load |
|---|---|
| Content brief | `modules/01_INTENT_ARCHITECTURE.md`, `modules/02_CONTENT_PRODUCTION.md`, `modules/07_QA_VERDICT.md` |
| Technical SEO audit | `modules/03_TECHNICAL_SEO.md`, `modules/07_QA_VERDICT.md` |
| Local SEO task | `modules/01_INTENT_ARCHITECTURE.md`, `modules/04_LOCAL_AND_SCALED_CONTENT.md`, `modules/07_QA_VERDICT.md` |
| AI-search visibility task | `modules/06_AI_SEARCH_VISIBILITY.md`, `modules/07_QA_VERDICT.md`; optionally `REFERENCE_QUERY_FANOUT_AND_SOURCE_ELIGIBILITY_v7.md` |
| Publishable article with image prompts | `modules/02_CONTENT_PRODUCTION.md`, `modules/08_IMAGE_GENERATION.md`, `modules/07_QA_VERDICT.md` |

## Default Execution Order
Lite controller initialization → canonical project context → required task modules → primary result → Module 08 image package when applicable → Module 07 compact QA → Lite controller verdict.

## Authority Rule
Use exactly one controller. References are optional and non-authoritative. Modules are task-only. Archived or legacy controllers are never active dependencies.

## Module 09: Humanization and Detector Governance

Load `modules/09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` for direct editorial humanization audits, related-batch similarity review, and optional governance of supplied detector results. Use Mode A for direct single-asset auditing, Mode B for related-batch similarity review, and add Mode C only when external detector evidence is supplied. Detector scores never establish authorship or publication eligibility. See `TEAM_MANUAL_MODULE_09.md` for team procedures and copy-paste execution prompts.
