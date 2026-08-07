<!--
File: START_HERE.md
Version: 7.4.1-search-policy-ranking-risk-governance
Classification: required setup documentation
Authority: operational documentation, non-authoritative
Required or optional: Required for setup
Controller dependency: SEO_MASTER_CONTROLLER_v7.md
May override controller: No
Source provenance: v7 corrected release setup documentation
-->

# START HERE — Full v7 Flat GPT

## Load in This Order
1. Load the sole controller: `SEO_MASTER_CONTROLLER_v7.md`.
2. Load the canonical project context: `CANONICAL_PROJECT_CONTEXT_v7.md`.
3. Identify the task type using the route map in `README.md`.
4. Load only the required active task module or modules.
5. Load an optional reference playbook only when its documented trigger applies.
6. For publishable content, include `MODULE_08_IMAGE_GENERATION.md` for the image-generation handoff.
7. Run `MODULE_07_QA_AND_RECOVERY.md` for specialist QA, then let the controller issue the final verdict.
8. Do not load archived files, competing controllers, or Flat and Modular copies together.

## Common Loading Examples
| Request | Load |
|---|---|
| Content brief | `MODULE_01_INTENT_ARCHITECTURE.md`, `MODULE_02_CONTENT_PRODUCTION.md`, `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`, `MODULE_07_QA_AND_RECOVERY.md` |
| Technical SEO audit | `MODULE_03_TECHNICAL_SEO.md`, `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`, `MODULE_07_QA_AND_RECOVERY.md` |
| Local SEO task | `MODULE_01_INTENT_ARCHITECTURE.md`, `MODULE_04_LOCAL_AND_SCALED_CONTENT.md`, `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`, `MODULE_07_QA_AND_RECOVERY.md` |
| AI-search visibility task | `MODULE_06_AI_SEARCH_VISIBILITY.md`, `MODULE_07_QA_AND_RECOVERY.md`; optionally `REFERENCE_QUERY_FANOUT_AND_SOURCE_ELIGIBILITY_v7.md` |
| Publishable article with image prompts | `MODULE_02_CONTENT_PRODUCTION.md`, `MODULE_08_IMAGE_GENERATION.md`, `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`, `MODULE_07_QA_AND_RECOVERY.md` |
| Single-asset humanization audit | `MODULE_02_CONTENT_PRODUCTION.md` when revision is required, `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` Mode A, `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`, `MODULE_07_QA_AND_RECOVERY.md` |
| Related content-batch audit | `MODULE_01_INTENT_ARCHITECTURE.md`, `MODULE_02_CONTENT_PRODUCTION.md`, `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` Mode B, `MODULE_04_LOCAL_AND_SCALED_CONTENT.md` when scaled/local risk applies, `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`, `MODULE_07_QA_AND_RECOVERY.md` |
| Supplied detector-result review | Run `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` Mode A or B first, then add Mode C; finish with `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`, `MODULE_07_QA_AND_RECOVERY.md` |

## Default Execution Order
Controller initialization → canonical project context → required task modules → primary content or audit result → Module 08 image package when applicable → Module 07 QA and recovery → controller evaluation → final verdict and registers.

## Authority Rule
Use exactly one controller. References are optional and non-authoritative. Modules are task-only. Archived or legacy controllers are never active dependencies.

## How to Call Module 09 in a Project

1. Load the selected package controller and canonical project context.
2. Load the normal production or audit modules required by the project.
3. Load `MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` when the project includes humanization, related-page similarity, batch originality, or supplied detector evidence.
4. Select Mode A for one asset or Mode B for a related batch. Add Mode C only when external detector results are supplied.
5. Run `MODULE_07_QA_AND_RECOVERY.md` after Module 09 and let the controller issue the final verdict.

Use this instruction after the files are loaded:

```text
Run Module 09 on the supplied project assets. Perform the direct audit yourself. Use Mode A for one asset or Mode B for a related batch. Add Mode C only for supplied external detector results. Do not require detector scores, do not infer authorship, preserve necessary qualifiers, and hand unresolved defects to Module 07.
```

For detailed intake and output procedures, open `TEAM_MANUAL_MODULE_09.md`.


## How Module 10 Is Called Automatically

The controller must invoke `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md` without requiring the user to name it whenever publication, indexation, policy, ranking-risk, scaled/local, link, structured-data, migration, recovery, security, or traffic-drop conditions apply.

The team supplies the task and evidence. The system selects the route and states it before execution.

## Mandatory Publication/Policy Gate

Before final QA, load `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md` whenever the output is intended for publication/indexation or the task involves material search-policy or ranking risk. The user does not need to name Module 10; the controller must route it automatically.

Do not issue publication-ready `PASS` while an applicable material policy category remains unresolved or `NOT TESTED`.
