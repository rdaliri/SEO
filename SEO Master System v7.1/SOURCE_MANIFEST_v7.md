<!--
File: SOURCE_MANIFEST_v7.md
Version: 7.0-corrected
Classification: optional reference playbook
Authority: Operational documentation; non-authoritative
Required or optional: Optional
Controller dependency: Sole package controller
May override controller: No
Source provenance: v7 release documentation
-->

# Source Manifest v7 — Corrected

## Release Metadata
- v7 release version: 7.0-corrected
- Migration date: 2026-07-24
- Reviewer/owner: Project owner or designated SEO systems reviewer
- Source package versions: Full v6 Image, Lite v6 Image, Elite v4 AI Search
- Destination file version: 7.0-corrected
- Checksum/content hash: generated in `RELEASE_VALIDATION_REPORT.md`

## File-Level Migration Traceability
| Source package | Source file | Source section or capability | v7 destination | Action | Final status | Notes |
|---|---|---|---|---|---|---|
| SEO_Framework_Elite_v4_AI_Search.zip | AI_SEARCH_VISIBILITY_MODULE_v4.md | Query fan-out and AI-search testing | Module 06; REFERENCE_QUERY_FANOUT_AND_SOURCE_ELIGIBILITY_v7.md | adapted | active module + reference-only | Specialist methodology retained; authority removed |
| SEO_Framework_Elite_v4_AI_Search.zip | TECHNICAL_SEO_GOVERNANCE.md | Source eligibility and technical accessibility | Module 03; query/source reference playbook | adapted | active module + reference-only | Checks remain evidence-bound |
| SEO_Framework_Elite_v4_AI_Search.zip | SEARCH_INTENT_AND_ENTITY_SYSTEM.md | Intent and entity mapping | Module 01 | merged | active module | Task-only guidance |
| SEO_Framework_Elite_v4_AI_Search.zip | AI_CONTEXT_AND_MEMORY_RULES.md | Context compression and memory handling | Canonical context; REFERENCE_CONTEXT_HANDLING_v7.md | adapted | active context + reference-only | No Module 09; no new fact authority |
| SEO_Framework_Elite_v4_AI_Search.zip | SEO_Content_System_Complete_Prompt_Kit.md | Content structures and production patterns | Module 02; REFERENCE_CONTENT_STRUCTURE_PLAYBOOK_v7.md | condensed | active module + reference-only | Formulaic rules removed |
| SEO_Framework_Elite_v4_AI_Search.zip | LOCAL_SEO_ARCHITECTURE_MODULE.md | Local SEO depth and differentiation | Module 04 | merged | active module | Proof and doorway controls preserved |
| SEO_Framework_Elite_v4_AI_Search.zip | CONTENT_LIFECYCLE_MANAGEMENT.md | Refresh, merge, redirect, retire | Module 05 | adapted | active module | Controller remains approval authority |
| SEO_Framework_Elite_v4_AI_Search.zip | ERROR_RECOVERY_AND_QA_PROTOCOL.md | Recovery and QA logic | Controller and Module 07 | rejected | archive-only | Competing QA authority not activated |
| SEO_Framework_Elite_v4_AI_Search.zip | PRODUCTION_MODES_FRAMEWORK.md | Production modes | README Full/Lite selection | condensed | reference-only | Mode concept retained without controller behavior |
| SEO_Framework_Elite_v4_AI_Search.zip | MODE_ACTIVATION_RULES.md | Mode activation | None | rejected | excluded | Would create competing activation logic |
| SEO_Framework_Elite_v4_AI_Search.zip | PROMPT_ORCHESTRATION_MAP.md | Routing and orchestration | None | archived | archive-only | Routing belongs exclusively to v7 controller |
| SEO_Framework_Elite_v4_AI_Search.zip | AI_WORKFLOW_KERNEL_MASTER_CONTROLLER.md | Master controller | None | archived | archive-only | Competing controller |
| SEO_Framework_Elite_v4_AI_Search.zip | SEO_TEAM_AI_SEARCH_MASTER_PROMPT_v4.md | Master prompt/controller behavior | None | archived | archive-only | Competing controller |
| SEO_Framework_Elite_v4_AI_Search.zip | ELITE_EXECUTION_START_HERE.md | Legacy load order | None | archived | archive-only | Superseded by v7 START_HERE |
| SEO_Framework_Elite_v4_AI_Search.zip | README_AI_SEO_Content_Workflow.md | Legacy workflow documentation | Migration report and provenance | moved to reference | reference-only | Historical context only |
| SEO_Framework_Elite_v4_AI_Search.zip | execution_guide_prompt_download.md | Legacy execution guide | None | archived | archive-only | Competing workflow guidance |
| SEO_Framework_Elite_v4_AI_Search.zip | CHANGELOG_v2.md; CHANGELOG_v3_ELITE.md; CHANGELOG_v4_AI_SEARCH.md | Historical changes | Controlled source storage | archived | archive-only | Not execution inputs |
| Full v6 image package | SEO_MASTER_CONTROLLER_v6.md | Evidence, missing-data, defects, QA, retries, stop and conflict rules | SEO_MASTER_CONTROLLER_v7.md | adapted | active controller | Required behavior preserved |
| Lite v6 image package | SEO_MASTER_CONTROLLER_LITE_v6.md | Compact daily execution contract | SEO_MASTER_CONTROLLER_LITE_v7.md | adapted | active controller | Reporting reduced; safety retained |
| v6 image packages | 08_IMAGE_GENERATION.md | Post-content image handoff | Module 08 | retained | active module | Runs before Module 07 and controller verdict |
