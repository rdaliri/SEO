# SEO Master Prompt System v6

## Purpose
A repeatable SEO production SOP with one controller, explicit evidence handling, deterministic routing, bounded refinement, and auditable approval rules.

## Load Order
1. `SEO_MASTER_CONTROLLER_v6.md`
2. `CANONICAL_PROJECT_CONTEXT_v6.md`
3. Only the required file(s) in `/modules`
4. `modules/07_QA_AND_RECOVERY.md` for final validation

Do not load v4, v5, or any other controller, orchestration, execution-guide, mode, or QA-governance prompt alongside the v6 controller.

## Standard Run
1. Complete or update the canonical context.
2. Give the controller the requested deliverable and source files.
3. Let the controller select the minimum route.
4. Review the Executive Summary, Decision Log, Structured Result, QA record, verdict, and Next Actions.
5. Approve or supply evidence for conditional items.
6. Update the evidence and task registers.

## File Governance
### Keep Active
- `SEO_MASTER_CONTROLLER_v6.md`
- `CANONICAL_PROJECT_CONTEXT_v6.md`
- `SEO_SYSTEM_AUDIT_REPORT_v6.md`
- `SOURCE_MANIFEST_v6.md`
- `README.md`
- `/modules/*.md`

### Archive Only
All v4 and v5 files. Preserve them for provenance, but do not load them during execution.

### Do Not Maintain Separately
Orchestration, execution guide, production modes, context governance, and module-specific quality-loop files. Their active rules now live in the sole controller.

## Primary Prompt Filename
`SEO_MASTER_CONTROLLER_v6.md`

## Mandatory Decision Behavior
- Missing `IMPORTANT` or `OPTIONAL` inputs: continue with explicit states and conditions.
- A partially blocking fact: reduce scope and deliver the safe, usable portion.
- A fully blocking fact that the user can provide: ask one bundled question only.
- An unresolved blocking safety, legal, identity, authorization, or material factual issue: stop with `FAIL` and return partial safe work.
- Any module/controller conflict: the controller wins; log `MODULE_CONFLICT`. Escalate unresolved conflicts through the blocking-fact rule.

## Mandatory Run Output
Every run must include the Executive Summary, Decision Log, Structured Result, Assumptions Register, Untested and Pending Verification Register, QA and Iteration Record, and Next Actions.
