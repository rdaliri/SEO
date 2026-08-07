# SEO Master System v7.4.1

A governed prompt system for SEO, AEO, GEO, content production, technical auditing, local and scaled SEO, AI-search visibility, editorial humanization, search-policy compliance, ranking-risk prevention, recovery, QA, and image-prompt generation.

## Release status

**Version:** `7.4.1-search-policy-ranking-risk-governance`  
**Release:** `7.4.1`  
**Release date:** `2026-08-07`  
**Status:** Production release  
**Validation target:** zero unresolved package-integrity errors

v7.4.1 is a corrective release that integrates Module 09 and Module 10 across the controller, package documentation, route maps, manifests, Flat/Modular variants, Full/Lite variants, team guidance, and validation artifacts.

## Packages

| Package | Mode | Format | Best use |
|---|---|---|---|
| `SEO_Master_System_v7` | Full | Modular | Repositories, IDEs, APIs, agents, automation, file-aware systems |
| `SEO_Master_System_Flat_v7` | Full | Flat | Complex ChatGPT projects, regulated/high-risk work, formal audits |
| `SEO_Master_System_Lite_v7` | Lite | Modular | Lower-overhead repository or automated execution |
| `SEO_Master_System_Lite_Flat_v7` | Lite | Flat | Routine manual ChatGPT projects |

Use exactly one package/controller in a run. Do not mix Full with Lite or Flat with Modular copies of the same active system.

## Core architecture

Each package has exactly one authoritative controller:

- Full: `SEO_MASTER_CONTROLLER_v7.md`
- Lite: `SEO_MASTER_CONTROLLER_LITE_v7.md`

The controller owns routing, evidence states, defect severity, retries, stop conditions, conflict escalation, QA thresholds, approval status, and final verdicts. Task modules cannot override it.

## Active modules

| Module | Purpose |
|---|---|
| 01 | Intent architecture, entities, keyword/page mapping, cannibalization |
| 02 | Content production, answer-first/AEO, readability, editorial quality |
| 03 | Technical SEO, crawl/indexation, rendering, structured data, accessibility |
| 04 | Local SEO, programmatic/scaled content, doorway and indexation defensibility |
| 05 | Content lifecycle, refresh/merge/redirect/noindex/retirement decisions |
| 06 | AI-search visibility, GEO, source eligibility, citation readiness |
| 07 | Final specialist QA, recovery, repair, verdict support |
| 08 | Image concepts, generation prompts, filenames, alt text, captions |
| 09 | Single-asset humanization, batch similarity/originality, detector-result governance |
| 10 | Search-policy compliance, ranking-risk prevention, diagnosis, recovery governance |

## Automatic routing

The user should normally describe the task and provide the evidence. The controller selects the smallest complete route.

### Module 09

Invoke Module 09 automatically when:

- one asset requires humanization/editorial audit: **Mode A**;
- three or more related assets or a shared template/cluster require cross-document comparison: **Mode B**;
- external detector results are supplied: add **Mode C** after the direct audit.

Do not require detector scores. Detector outputs never prove authorship and cannot be the sole basis for approval, rejection, or rewriting.

### Module 10

Invoke Module 10 automatically when publication/indexation or material search-policy/ranking risk applies, including:

- publishable content;
- local/scaled/programmatic pages;
- links, affiliate/review content, or third-party hosted content;
- structured data;
- migrations, redirects, expired domains;
- ranking/traffic drops, manual actions, security issues, recovery;
- explicit policy-compliance requests.

Module 10 is the cross-module policy gate before final QA. It does not replace Module 02, 03, 04, 05, 06, 09, or the controller.

## Common routes

| Task | Route |
|---|---|
| New publishable article | Controller → Context → 01 when needed → 02 → 09 Mode A when editorial audit applies → 10 → 08 when relevant → 07 → Controller verdict |
| Related content batch | Controller → Context → 01 → 02 → 09 Mode B → 04 when local/scaled risk applies → 06 when AI-search applies → 10 → 08 when relevant → 07 → verdict |
| Technical/schema audit | Controller → Context → 03 → 10 → 07 → verdict |
| Local/scaled landing pages | Controller → Context → 01 → 02 when copy applies → 09 Mode B → 04 → 10 → 07 → verdict |
| Migration/recovery | Controller → Context → 05 → 03 when implementation applies → 10 → 07 → verdict |
| AI-search/GEO audit | Controller → Context → 06 → 10 when publication/policy/eligibility applies → 07 → verdict |
| Detector report review | Direct Mode A/B audit first → add Mode C → 10 when publishable/policy relevant → 07 → verdict |

## Search-policy and ranking-risk coverage

Module 10 coordinates applicable checks for:

- cloaking;
- doorway abuse;
- expired-domain abuse;
- hacked content/security;
- hidden text/links;
- keyword stuffing;
- link spam;
- machine-generated traffic;
- misleading functionality, scams, or fraud;
- policy circumvention;
- scraping and low-value republishing;
- scaled content abuse;
- site reputation abuse;
- sneaky redirects;
- thin affiliation;
- user-generated spam;
- structured-data integrity;
- people-first content quality and evidence;
- review/affiliate value;
- cross-engine crawl/indexing and discovery controls;
- ranking-drop diagnosis without falsely labeling every decline a penalty.

A policy-risk check can reduce preventable risk, but no prompt system can guarantee ranking, indexing, rich results, Discover visibility, AI citation, or immunity from algorithmic changes.

## Evidence states

Use explicit evidence states defined by the controller, including:

- `SUPPLIED`
- `OBSERVED`
- `CALCULATED`
- `INFERRED`
- `NOT TESTED`
- `UNKNOWN`
- `RECOMMENDED`

Do not present inferred, recommended, or untested information as verified fact.

## ChatGPT Project setup: Full Flat

For a Full Flat ChatGPT Project, upload once as Project Sources:

- `SEO_MASTER_CONTROLLER_v7.md`
- `CANONICAL_PROJECT_CONTEXT_v7.md`
- `MODULE_01_INTENT_ARCHITECTURE.md` through `MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md`
- `START_HERE.md`
- package `README.md`
- `TEAM_MANUAL_MODULE_09.md`

Use `PROJECT_INSTRUCTION_FULL_FLAT_v7.4.1.md` in the Project Instructions field. It is designed to stay below ChatGPT's 8,000-character Project Instruction limit.

Do **not** routinely upload validation JSON, migration reports, release notes, checksums, or release-validation files as operational sources. They are release/QA evidence.

## Flat versus Modular

Flat packages keep active modules at the package root and are easiest for manual upload. Modular packages keep task modules in `/modules` and are preferred for repositories, IDEs, APIs, agents, and automation.

Full and Lite share the same core safety/evidence principles. Lite reduces reporting depth, not policy or critical-defect standards.

## Team documentation

- `TEAM_OPERATIONS_MANUAL_v7.4.1.md` — operating guide for projects and routing
- `TEAM_MANUAL_MODULE_09.md` — Module 09 intake, execution, and handoff
- `PROJECT_INSTRUCTION_FULL_FLAT_v7.4.1.md` — ready-to-paste ChatGPT Project instruction
- `OFFICIAL_POLICY_SOURCE_REGISTER_v7.4.1.md` — official-source register used for Module 10 governance

## Validation and release evidence

Current release artifacts:

- `RELEASE_VALIDATION_REPORT_v7.4.1.md`
- `PACKAGE_VALIDATION_v7.4.1.json`
- `SHA256SUMS.txt`
- `SOURCE_MANIFEST_v7.md`
- `CHANGELOG.md`

Historical validation/release artifacts are stored under `/history` to keep the active release root unambiguous.

## Suggested repository structure

```text
seo-master-system-v7/
├── README.md
├── CHANGELOG.md
├── OFFICIAL_POLICY_SOURCE_REGISTER_v7.4.1.md
├── PROJECT_INSTRUCTION_FULL_FLAT_v7.4.1.md
├── RELEASE_NOTES_v7.4.1.md
├── RELEASE_VALIDATION_REPORT_v7.4.1.md
├── PACKAGE_VALIDATION_v7.4.1.json
├── SHA256SUMS.txt
├── TEAM_OPERATIONS_MANUAL_v7.4.1.md
├── SEO_Master_System_v7/
├── SEO_Master_System_Flat_v7/
├── SEO_Master_System_Lite_v7/
├── SEO_Master_System_Lite_Flat_v7/
└── history/
```

## Responsible use

Do not use the system to fabricate evidence, experts, credentials, patient/customer experiences, reviews, locations, technical tests, detector runs, first-party data, or search-engine outcomes.

For medical, legal, financial, privacy, security, or other regulated/high-risk work, require the appropriate qualified review when the controller or active modules identify it as necessary.

## License

Retain the repository's applicable license and copyright notice when redistributing or modifying the system.
