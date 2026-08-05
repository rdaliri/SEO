<!--
File: SEO_V7_MIGRATION_REPORT.md
Version: 7.1-seo-aeo-geo-humanize
Classification: release migration documentation
Authority: non-authoritative
Required or optional: optional
Controller dependency: SEO_MASTER_CONTROLLER_v7.md
May override controller: No
Source provenance: v7 migration record based on Full/Lite v6 and Elite v4
-->

# SEO v7 Migration Report — Corrected Release

## Release
- Version: 7.0-corrected
- Migration date: 2026-07-24
- Owner/reviewer: Project owner or designated SEO systems reviewer
- Source systems: Full v6 with image handoff, Lite v6 with image handoff, Elite v4 AI Search reference package

## Architecture Decision
v7 uses one authoritative controller per package. Full and Lite remain separate operating profiles. Flat and Modular remain separate packaging formats.

### Context-Handling Decision
`09_CONTEXT_AND_MEMORY_v7.md` was intentionally not created. Project-state authority belongs in the canonical context file:
- `CANONICAL_PROJECT_CONTEXT_v7.md`, or
- `CANONICAL_PROJECT_CONTEXT_LITE_v7.md`.

Extended context compression, carry-forward, handoff, and cleanup techniques remain optional and non-authoritative in `REFERENCE_CONTEXT_HANDLING_v7.md`.

The reference playbook cannot:
- create permanent or unverified project facts,
- override evidence states,
- modify controller rules,
- silently change canonical context,
- or become a competing memory authority.

## Elite v4 Capability Migration
| Elite capability | v7 destination | Action | Final status | Notes |
|---|---|---|---|---|
| Query fan-out methodology | Module 06 and query/source reference playbook | adapted and merged | active module + reference-only | Specialist research method; no routing authority |
| Source eligibility rules | Modules 03 and 06 plus reference playbook | adapted | active module + reference-only | Unchecked eligibility remains `NOT TESTED` |
| Entity mapping | Module 01 | adapted and merged | active module | Task logic only |
| AI-search visibility testing | Module 06 | adapted | active module | Direct observation required for verified test findings |
| Production modes | Full/Lite package selection | condensed | active documentation | No mode controller |
| Context handling | Canonical context plus reference playbook | adapted and moved to reference | active context + reference-only | Module 09 intentionally rejected |
| Content structure templates | Module 02 plus content structure playbook | condensed | active module + reference-only | Optional patterns, not formulas |
| Local SEO depth | Module 04 | adapted and merged | active module | Maintains doorway and proof safeguards |
| Technical accessibility | Module 03 | adapted and merged | active module | Includes rendered-content and accessibility checks |
| Recovery and QA | Existing v6-derived controller and Module 07 | retained; Elite authority rejected | active controller/module | Elite QA cannot override v7 |

## Full and Lite
Lite reduces reporting and formatting overhead only. It preserves evidence discipline, unsupported-claim controls, critical-defect handling, retry and stop rules, conflict escalation, controller authority, verdict behavior, and image handoff.

## Flat and Modular
Flat and Modular editions of the same mode contain equivalent active operational content. Differences are limited to paths, filenames, navigation, archive placement, and manual-loading guidance.

## Legacy Governance
Elite v4 controllers, orchestration maps, mode activation files, production-mode controllers, and alternate QA governance remain archive-only or excluded. They must never be loaded with v7.
