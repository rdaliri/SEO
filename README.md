# SEO Master System v7.3.1

A production-ready prompt system for SEO, AEO, GEO, content production, technical auditing, local and scaled SEO, AI-search visibility, editorial humanization, batch-similarity review, image-prompt generation, and final QA.

The release provides Full and Lite editions in Flat and Modular formats so the same governance model can be used in ChatGPT Projects, repositories, IDEs, APIs, agents, and automated workflows.

## Release Status

**Version:** `v7.3.1-editorial-humanization-governance`  
**Status:** Production-ready  
**Validation verdict:** `PASS`

This release preserves:

- one authoritative controller per package
- automatic task and module routing
- explicit evidence states
- deterministic missing-data handling
- bounded retries and stop conditions
- module-conflict escalation
- mandatory QA and final verdict logic
- image-generation handoff after content production
- SEO, AEO, GEO, and humanization controls
- direct single-asset editorial auditing
- cross-document batch-similarity auditing
- non-authoritative AI-detector result governance

## What This System Does

The controller selects the smallest complete module route for each task.

The system supports:

- SEO strategy, intent architecture, entities, and page-role planning
- keyword research, site architecture, and cannibalization review
- content briefs, articles, landing pages, and rewrites
- technical SEO audits
- local and scaled-content projects
- content refresh, consolidation, redirect, and retirement decisions
- AEO and GEO visibility review
- AI-search source eligibility and citation readiness
- single-asset editorial humanization audits
- cross-document similarity and originality audits
- external AI-detector result governance
- image concepts and generation-ready prompts
- final QA, defect correction, retesting, and verdict preparation

## Packages

| Package | Mode | Format | Best use |
|---|---|---|---|
| `SEO_Master_System_v7` | Full | Modular | Repositories, automation, APIs, IDEs, agents, and file-aware systems |
| `SEO_Master_System_Flat_v7` | Full | Flat | Complex ChatGPT Projects, formal audits, regulated topics, and high-risk work |
| `SEO_Master_System_Lite_v7` | Lite | Modular | Faster repository-based or automated daily execution |
| `SEO_Master_System_Lite_Flat_v7` | Lite | Flat | Routine manual work in ChatGPT |

## Recommended Edition

Use **Lite Flat** for routine manual work with reduced reporting overhead.

Use **Full Flat** for complex audits, client-facing deliverables, regulated topics, scaled-content reviews, batch humanization, or projects requiring detailed evidence and decision registers.

Use **Full Modular** for repositories, APIs, IDEs, agents, and automated production pipelines.

## Full Versus Lite

### Full

The Full edition is designed for complex or high-risk work. It provides:

- detailed evidence and assumption registers
- expanded decision logs
- full defect tracking
- detailed QA and iteration history
- Module 09 batch reports
- stronger auditability for client-facing or regulated work

### Lite

The Lite edition reduces reporting and formatting overhead while preserving core governance.

Lite does **not** weaken:

- evidence-state discipline
- unsupported-claim controls
- critical-defect handling
- retry limits
- stop conditions
- conflict escalation
- controller authority
- final verdict behavior
- image-generation handoff
- Module 09 detector-governance rules

## Flat Versus Modular

### Flat

Flat editions place all active files at the package root.

Use Flat when manually uploading files to ChatGPT Projects or another interface that may not reliably discover nested folders.

### Modular

Modular editions keep task modules inside `/modules`.

Use Modular in repositories, IDEs, APIs, agents, or automation environments with reliable file discovery.

Flat and Modular editions of the same mode contain equivalent operational rules. Their differences are limited to filenames, paths, navigation, and loading instructions.

## Core Architecture

Each package contains exactly one authoritative controller.

### Full Controller

`SEO_MASTER_CONTROLLER_v7.md`

### Lite Controller

`SEO_MASTER_CONTROLLER_LITE_v7.md`

The controller is the sole authority for:

- task routing
- evidence states
- missing-data decisions
- defect severity
- retries
- stop conditions
- conflict escalation
- QA thresholds
- approval status
- final verdicts
- image-generation handoff

Task modules cannot override the controller.

## Active Modules

| Module | Purpose |
|---|---|
| Module 01 | Intent, keyword architecture, entities, page mapping, and cannibalization |
| Module 02 | Content production, AEO answer-first rules, readability, and page-level humanization |
| Module 03 | Technical SEO, crawlability, indexability, rendering, structured data, and accessibility |
| Module 04 | Local SEO, programmatic pages, scaled-content safeguards, and doorway-risk review |
| Module 05 | Content lifecycle, refresh, merge, redirect, noindex, and retirement decisions |
| Module 06 | AI-search visibility, GEO, source eligibility, freshness, proof, and citation readiness |
| Module 07 | Specialist QA, recovery, repair, retesting, and verdict support |
| Module 08 | Image-generation prompts, filenames, alt text, captions, and image handoff |
| Module 09 | Single-asset editorial auditing, batch similarity, originality, and detector governance |

## Default Execution Architecture

```text
Controller
  ↓
Canonical project context
  ↓
Selected task modules
  ↓
Primary deliverable
  ↓
Module 09 when editorial or batch review applies
  ↓
Module 04 when local or scaled-content risk applies
  ↓
Module 08 when image work applies
  ↓
Module 07 QA and recovery
  ↓
Controller verdict
```

The controller selects the smallest complete route. The user does not need to name every module manually.

## Automatic Module 09 Routing

`MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md` must be invoked automatically when its trigger conditions are met.

### Mode A: Single-Asset Editorial Audit

Use automatically when one article, landing page, brief, or draft needs review, improvement, humanization, or publication preparation.

Mode A checks for:

- generic or formulaic openings
- repeated sentence stems
- uniform sentence and paragraph rhythm
- weak specificity or information gain
- unsupported claims
- weakened factual, medical, legal, financial, or technical qualifiers
- fabricated experience
- artificial humanization tactics
- templated conclusions

### Mode B: Batch Humanization and Similarity Audit

Use automatically when:

- three or more related drafts are supplied
- multiple pages share a template, service family, location pattern, keyword cluster, page type, or editorial framework
- the user requests review, comparison, improvement, humanization, validation, or publication preparation for a related batch
- structural duplication, weak differentiation, page-role overlap, near-duplicate content, or scaled-content risk may exist

Mode B must compare all pages against one another, not only review them individually.

It checks for:

- structural duplication
- repeated phrases and sentence stems
- repeated headings and section order
- repeated CTAs, FAQs, disclaimers, metadata, and anchor text
- near-duplicate paragraphs
- intent or page-role overlap
- weak page-specific information gain
- templated conclusions
- unnecessary uniformity across the batch

The user does not need to write:

```text
Run Module 09 Mode B
```

when the batch conditions are already present.

### Mode C: External Detector Result Governance

Use only when external AI-detector results are supplied.

Detector results must be:

- recorded with the tool, date, version when known, tested scope, and reported result
- classified as `SUPPLIED`
- treated as non-authoritative observations
- excluded as proof of authorship
- excluded as the sole reason for approval, rejection, rewriting, or publication

Authorship remains:

```text
NOT TESTED
```

### Combined Mode

Use when a direct Mode A or Mode B audit and supplied detector-result governance both apply.

## Evidence States

The system uses explicit evidence labels:

- `SUPPLIED` — provided directly by the user or project
- `OBSERVED` — directly inspected or verified
- `CALCULATED` — derived from supplied or observed data
- `INFERRED` — reasonable interpretation that is not directly verified
- `NOT TESTED` — not verified or not yet inspected
- `UNKNOWN` — required information is unavailable
- `RECOMMENDED` — proposed action or improvement

The system must not present inferred, recommended, unknown, or untested information as verified fact.

## ChatGPT Project Setup

### 1. Create a Dedicated Project

Create one project for the selected package edition.

Do not mix Full and Lite, Flat and Modular, or different release versions in the same project.

### 2. Add the Project Instruction

Paste the approved Full Flat or Lite Flat project instruction into the ChatGPT Project Instructions field.

The instruction should:

- establish controller authority
- require automatic task routing
- require automatic Module 09 activation
- define evidence states
- prohibit fabricated evidence
- require Module 07 final QA

### 3. Upload Permanent Project Sources

For Full Flat, upload these once:

```text
SEO_MASTER_CONTROLLER_v7.md
CANONICAL_PROJECT_CONTEXT_v7.md
MODULE_01_INTENT_ARCHITECTURE.md
MODULE_02_CONTENT_PRODUCTION.md
MODULE_03_TECHNICAL_SEO.md
MODULE_04_LOCAL_AND_SCALED_CONTENT.md
MODULE_05_CONTENT_LIFECYCLE.md
MODULE_06_AI_SEARCH_VISIBILITY.md
MODULE_07_QA_AND_RECOVERY.md
MODULE_08_IMAGE_GENERATION.md
MODULE_09_BATCH_HUMANIZATION_AND_DETECTOR_GOVERNANCE.md
START_HERE.md
README.md
TEAM_MANUAL_MODULE_09.md
```

Optional reference files may also be uploaded when their triggers apply.

### 4. Keep Release Records Outside the Active Prompt Set

The following normally remain in the repository or release archive, but are not loaded as operational prompts:

```text
PACKAGE_VALIDATION_v7.3.1.json
RELEASE_VALIDATION_REPORT.md
CHANGELOG.md
RELEASE_NOTES_v7.3.1.md
SOURCE_MANIFEST_v7.md
FLAT_FILE_MAP.md
SEO_V7_MIGRATION_REPORT_FULL.md
SEO_V7_MIGRATION_REPORT_LITE.md
SHA256SUMS.txt
```

These files support release management, technical QA, traceability, and troubleshooting.

## Starting a Task

Attach client or task-specific files in the current chat and describe the requested work.

Example:

```text
Use the Full Flat v7 project sources.

Review the attached service-page drafts and prepare them for publication.
Determine the smallest complete module route, state the selected route, execute
the work, and run Module 07 final QA.

Business objective: Improve organic visibility and conversion quality.
Target audience: Prospective local-service customers.
Constraints: Do not invent services, claims, locations, credentials, or outcomes.
```

The controller should select the required modules automatically.

## Common Routing Examples

### Single Article Review

```text
Controller
→ Canonical Context
→ Module 02 when revision is required
→ Module 09 Mode A
→ Module 08 when images are relevant
→ Module 07
```

### Related Content Batch

```text
Controller
→ Canonical Context
→ Module 01 when intent architecture needs review
→ Module 02
→ Module 09 Mode B
→ Module 04 when scaled or local risk applies
→ Module 06 when AEO or GEO applies
→ Module 08 when images are relevant
→ Module 07
```

### Technical SEO Audit

```text
Controller
→ Canonical Context
→ Module 03
→ Module 07
```

### Local or Programmatic Page Set

```text
Controller
→ Canonical Context
→ Module 01
→ Module 02 when content is produced or revised
→ Module 09 Mode B
→ Module 04
→ Module 07
```

### External Detector Reports

```text
Controller
→ Canonical Context
→ Module 09 Mode A or B direct audit
→ Module 09 Mode C for supplied detector evidence
→ Module 07
```

## Required Output Standard

Substantial Full-edition tasks should return, when applicable:

1. Executive Summary
2. Decision Log
3. Structured Result
4. Evidence and Assumption Register
5. Defect Register
6. QA Score
7. Verdict
8. Conditions, owners, and retest requirements

Module 09 batch work should also include:

- Detector Result Register when detector evidence is supplied
- Batch Fingerprint Report
- Page Uniqueness Matrix
- Phrase-Repetition Report
- Structural Revision Plan
- Before-and-After Samples
- Evidence and Approval Gaps
- Handoff to Module 07

## Reference Files

Reference playbooks are optional and non-authoritative.

| Reference file | Load only when |
|---|---|
| Query fan-out and source eligibility | Running AI-search research, query expansion, source analysis, citation eligibility, or platform-test design |
| Content structure playbook | Selecting or adapting a page or content structure |
| Context-handling playbook | Managing long-running projects, context compression, handoff preparation, or project-state cleanup |

Reference files:

- are never controllers
- cannot change evidence states
- cannot change QA thresholds
- cannot change the output contract
- cannot override canonical context
- should not all be loaded by default

## SEO, AEO, GEO, and Humanization Coverage

### SEO

The active system covers:

- crawlability
- indexability
- rendering
- structured data
- internal linking
- entities
- site and page architecture
- local SEO
- content lifecycle
- technical QA

### AEO

The active system requires:

- direct answers for answer-seeking queries
- self-contained opening answer blocks
- question-to-answer alignment
- concise answers for short direct queries
- explicit fallback when answer-first is not appropriate
- snippet-ready supporting structure

### GEO

The active system includes:

- AI-search visibility testing
- query fan-out
- source eligibility
- citation-readiness checks
- visible freshness actions
- author or expert attribution when credibility requires it
- first-party proof collection or evidence substitution
- recency and credibility controls

### Humanization and Originality

The active system checks:

- generic AI-style openings
- filler transitions
- repetitive conclusions
- templated closings
- repetitive syntax
- excessive parallelism
- overuse of lists
- uniform sentence cadence
- paragraph-rhythm variation
- tone alignment
- readability
- article-specific information gain
- cross-document similarity
- page-role overlap
- repeated CTAs, FAQs, disclaimers, and metadata
- near-duplicate paragraphs
- final human-editing quality

## AI-Detector Governance

Do not use detector percentages as proof of:

- authorship
- originality
- factual accuracy
- medical or legal accuracy
- usefulness
- SEO quality
- AEO or GEO readiness
- plagiarism
- publication eligibility

Never manipulate content through deliberate spelling mistakes, grammatical errors, random slang, fake personal experience, unsupported quotations, punctuation manipulation, or factual distortion to influence a detector score.

## Image-Generation Workflow

For publishable content, Module 08 runs after the primary content output and before final QA when images are relevant.

Each image package may include:

- primary production-ready prompt
- alternative prompts
- recommended aspect ratio
- SEO-friendly filename
- accessible alt text
- publication-ready caption
- evidence state
- usage or license note

The module avoids fabricated trademarks, logos, identifiable real people, unsupported locations, fake products, and misleading photographic claims.

## Team Workflow

### Project Owner

- confirms the business objective
- supplies approved project facts
- confirms scope and deliverables
- resolves business decisions and approvals

### SEO Strategist

- validates intent and page role
- reviews keyword and architecture decisions
- evaluates local, scaled, and cannibalization risk

### Content Editor

- reviews clarity, usefulness, structure, tone, and qualifiers
- implements Module 09 recommendations
- avoids detector-evasion tactics

### Technical Reviewer

- validates technical SEO findings
- confirms implementation feasibility
- verifies schema, crawl, metadata, and indexation recommendations

### QA Reviewer

- runs Module 07
- verifies unresolved defects
- confirms evidence states
- controls final readiness recommendations

## Governance Safeguards

Do not load together:

- Full and Lite controllers
- Flat and Modular copies of the same system
- v6 and v7 controllers
- Elite v4 controllers and v7 controllers
- legacy orchestration prompts and the v7 controller
- duplicate copies of the same active module

Exactly one controller must be active in each run.

## Validation

The release may include:

- `PACKAGE_VALIDATION_v7.3.1.json`
- `RELEASE_VALIDATION_REPORT.md`
- `CHANGELOG.md`
- `SOURCE_MANIFEST_v7.md`
- package-specific migration reports
- detached `SHA256SUMS.txt`

Validation should confirm:

- one controller per package
- exact filenames and route maps
- Full/Lite separation
- Flat/Modular equivalence
- Module 09 availability and automatic routing
- correct Full and Lite Module 07 references
- preserved governance
- image-generation workflow order
- active SEO, AEO, GEO, and humanization controls
- file-level traceability

## Verify Downloads

Use the detached checksum file:

`SHA256SUMS.txt`

macOS or Linux:

```bash
sha256sum -c SHA256SUMS.txt
```

macOS without `sha256sum`:

```bash
shasum -a 256 SEO_Master_System_v7.zip
```

Windows PowerShell:

```powershell
Get-FileHash .\SEO_Master_System_v7.zip -Algorithm SHA256
```

## Suggested Repository Structure

```text
seo-master-system-v7/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── RELEASE_VALIDATION_REPORT.md
├── SHA256SUMS.txt
├── releases/
│   ├── SEO_Master_System_v7.zip
│   ├── SEO_Master_System_Flat_v7.zip
│   ├── SEO_Master_System_Lite_v7.zip
│   └── SEO_Master_System_Lite_Flat_v7.zip
├── docs/
│   ├── START_HERE.md
│   ├── TEAM_MANUAL_MODULE_09.md
│   ├── TEAM_OPERATIONS_MANUAL.md
│   ├── SOURCE_MANIFEST_v7.md
│   ├── SEO_V7_MIGRATION_REPORT_FULL.md
│   └── SEO_V7_MIGRATION_REPORT_LITE.md
└── validation/
    └── PACKAGE_VALIDATION_v7.3.1.json
```

## Release Process

1. Update package contents.
2. Run package validation.
3. Confirm controller and module metadata.
4. Confirm Module 09 automatic routing documentation.
5. Rebuild all four ZIP files.
6. Generate detached SHA-256 hashes.
7. Update the changelog and release notes.
8. Publish ZIP files and checksum files in a GitHub Release.
9. Tag the release, for example:

```text
v7.3.1
```

## Version Control Guidance

Use a new minor or major release when changing:

- controller authority
- module routing
- evidence-state definitions
- severity rules
- QA acceptance criteria
- required outputs
- package structure

Use a patch release for documentation corrections that do not change system behavior.

Recommended branch names:

```text
feature/module-09-routing
fix/readme-project-setup
docs/team-operations-manual
release/v7.3.1
```

Recommended commits:

```text
feat: add automatic Module 09 batch routing
fix: correct Full and Lite QA module references
docs: update GitHub project setup guide
chore: update package validation report
```

## Contributing

Contributions should preserve:

- single-controller authority
- evidence-state definitions
- retry and stop rules
- QA thresholds
- Full/Lite separation
- Flat/Modular equivalence
- Module 08 image handoff
- Module 09 automatic routing
- task-only module boundaries

Changes to governance should include:

- rationale
- affected files
- migration notes
- validation updates
- updated detached checksums

Before submitting a pull request:

- confirm controller and module references
- verify Flat and Modular variants remain aligned
- verify Full and Lite routes use the correct filenames
- update release notes and changelog
- run package validation
- confirm no obsolete module names remain
- confirm documentation matches actual system behavior

## Security and Responsible Use

This system does not replace professional legal, medical, financial, accessibility, privacy, or regulatory review.

Do not use it to:

- fabricate evidence
- invent experts or credentials
- create fake first-party proof
- misrepresent detector or AI-search testing
- publish unsupported technical findings
- weaken necessary medical, legal, financial, or technical qualifiers
- produce misleading local pages or doorway content

## License

This project is licensed under the MIT License.

You may use, copy, modify, merge, publish, distribute, sublicense, and reuse this project, including for commercial purposes, provided that the original copyright and license notice are retained.

Copyright (c) 2026 Reza DaliriRad (rdaliri)

See [LICENSE](LICENSE) for the full license terms.

## Release Notes

### v7.3.1

- Added automatic Module 09 routing to project documentation
- Added direct Mode A single-asset editorial auditing
- Added direct Mode B cross-document batch-similarity auditing
- Made external detector results optional and secondary
- Added Mode C detector-result governance
- Preserved authorship as `NOT TESTED`
- Prohibited detector-evasion editing
- Added Full and Lite route corrections
- Added team operations and project setup guidance
- Preserved controller authority, evidence discipline, QA, and stop conditions

---

**Recommended routine edition:** Lite Flat for daily ChatGPT work.  
**Recommended advanced ChatGPT edition:** Full Flat for complex, batch, regulated, or client-facing work.  
**Recommended automation edition:** Full Modular for repositories, agents, APIs, IDEs, and automated pipelines.
