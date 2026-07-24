# SEO Master System v7.1

A production-ready prompt system for SEO, AEO, GEO, humanized content production, technical auditing, local SEO, AI-search visibility, QA, and image-prompt generation.

The release provides four editions so the same governance model can be used in ChatGPT, repositories, IDEs, APIs, agents, and automated workflows.

## Release status

**Version:** `7.1-seo-aeo-geo-humanize`  
**Status:** Production-ready  
**Validation verdict:** PASS

The system preserves:

- one authoritative controller per package
- explicit evidence states
- deterministic missing-data handling
- bounded retries and stop conditions
- module-conflict escalation
- mandatory QA and final verdict logic
- image-generation handoff after content production
- SEO, AEO, GEO, and humanization controls

## Packages

| Package | Mode | Format | Best use |
|---|---|---|---|
| `SEO_Master_System_v7` | Full | Modular | Repositories, automation, APIs, IDEs, agents, and file-aware systems |
| `SEO_Master_System_Flat_v7` | Full | Flat | Complex manual ChatGPT projects, formal audits, and high-risk work |
| `SEO_Master_System_Lite_v7` | Lite | Modular | Fast repository-based or automated daily execution |
| `SEO_Master_System_Lite_Flat_v7` | Lite | Flat | Routine manual work in ChatGPT |

## Recommended edition

Use **Lite Flat v7.1** for routine manual work in ChatGPT.

Use **Full Flat v7.1** for complex audits, client-facing deliverables, regulated topics, scaled-content reviews, or projects requiring detailed evidence and decision registers.

Use **Full Modular v7.1** for repositories, APIs, IDEs, agents, and automated production pipelines.

## Full versus Lite

### Full

The Full edition is designed for complex or high-risk work. It provides:

- detailed assumptions and verification registers
- expanded decision logs
- full defect tracking
- detailed QA and iteration history
- stronger auditability for client-facing or regulated work

### Lite

The Lite edition reduces reporting and formatting overhead while preserving the same core governance.

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

## Flat versus Modular

### Flat

The Flat editions place all active files at the package root.

Use Flat when manually uploading files to ChatGPT or another interface that may not reliably discover nested folders.

### Modular

The Modular editions keep task modules inside `/modules`.

Use Modular in repositories, IDEs, APIs, agents, or automation environments with reliable file discovery.

Flat and Modular editions of the same mode contain equivalent operational rules. Their differences are limited to filenames, paths, navigation, and loading instructions.

## Core architecture

Each package contains exactly one authoritative controller.

### Full controller

`SEO_MASTER_CONTROLLER_v7.md`

### Lite controller

`SEO_MASTER_CONTROLLER_LITE_v7.md`

The controller is the sole authority for:

- routing
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

## Active modules

| Module | Purpose |
|---|---|
| Module 01 | Intent, keyword architecture, entities, page mapping, and cannibalization |
| Module 02 | Content production, AEO answer-first rules, readability, and humanization |
| Module 03 | Technical SEO, crawlability, indexability, rendering, structured data, and accessibility |
| Module 04 | Local SEO and scaled-content safeguards |
| Module 05 | Content lifecycle, refresh, merge, redirect, noindex, and retirement decisions |
| Module 06 | AI-search visibility, GEO, source eligibility, freshness, proof, and citation readiness |
| Module 07 | Specialist QA, recovery, repair, and verdict support |
| Module 08 | Image-generation prompts, filenames, alt text, captions, and image handoff |

## Evidence states

The system uses explicit evidence labels:

- `SUPPLIED` — provided directly by the user or project
- `OBSERVED` — directly inspected or verified
- `CALCULATED` — derived from supplied or observed data
- `INFERRED` — reasonable interpretation that is not directly verified
- `NOT TESTED` — not verified or not yet inspected

The system must not present inferred, recommended, or untested information as verified fact.

## Default execution sequence

### Full workflow

1. Initialize the Full controller.
2. Load the canonical project context.
3. Load only the required task modules.
4. Produce the primary content or audit result.
5. Run Module 08 for publishable content when an image is relevant.
6. Run Module 07 QA and recovery.
7. Let the controller evaluate the result.
8. Return the final verdict and required registers.

### Lite workflow

1. Initialize the Lite controller.
2. Load the Lite canonical project context.
3. Load only the required task modules.
4. Produce the primary result.
5. Run Module 08 when an image is relevant.
6. Run Module 07 compact QA.
7. Let the Lite controller issue the final verdict.

Module 08 does not replace content QA. Module 07 does not override the controller.

## ChatGPT loading instructions

For Flat packages:

1. Open `START_HERE.md`.
2. Load the sole controller.
3. Load the canonical project context.
4. Use the route map to identify the required modules.
5. Load only those active modules.
6. Load optional reference files only when their documented trigger applies.
7. Do not load competing controllers, legacy governance files, or duplicate module copies.

### Example loading sets

**Content brief**

- Controller
- Canonical context
- Module 01
- Module 02
- Module 07

**Technical SEO audit**

- Controller
- Canonical context
- Module 03
- Module 07

**Local SEO page**

- Controller
- Canonical context
- Module 01
- Module 04
- Module 07

**AI-search visibility audit**

- Controller
- Canonical context
- Module 06
- Module 07

**Publishable article with image prompts**

- Controller
- Canonical context
- Module 02
- Module 08
- Module 07

## Reference files

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

## SEO, AEO, GEO, and humanization coverage

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

### Humanization

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
- concrete examples
- final human-editing pass

## Image-generation workflow

For publishable content, Module 08 runs after content output and before final QA.

Each image package may include:

- primary production-ready prompt
- two alternative prompts
- recommended aspect ratio
- SEO-friendly filename
- accessible alt text
- publication-ready caption
- evidence state
- usage or license note

The module avoids fabricated trademarks, logos, identifiable real people, unsupported locations, fake products, and misleading photographic claims.

## Governance safeguards

Do not load together:

- Full and Lite controllers
- Flat and Modular copies of the same system
- v6 and v7 controllers
- Elite v4 controllers and v7 controllers
- legacy orchestration prompts and the v7 controller
- duplicate copies of the same active module

Exactly one controller must be active in each run.

## Validation

The release includes:

- `RELEASE_VALIDATION_REPORT.md`
- `CHANGELOG.md`
- `SOURCE_MANIFEST_v7.md`
- package-specific migration reports
- detached `SHA256SUMS.txt`

The validation confirms:

- one controller per package
- exact filenames and route maps
- Full/Lite separation
- Flat/Modular equivalence
- preserved governance
- image-generation workflow order
- active SEO/AEO/GEO/humanization controls
- file-level traceability

## Verify downloads

Use the detached checksum file:

`SHA256SUMS.txt`

Example on macOS or Linux:

```bash
sha256sum -c SHA256SUMS.txt
```

On macOS systems without `sha256sum`:

```bash
shasum -a 256 SEO_Master_System_v7.zip
```

On Windows PowerShell:

```powershell
Get-FileHash .\SEO_Master_System_v7.zip -Algorithm SHA256
```

## Suggested repository structure

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
└── docs/
    ├── SOURCE_MANIFEST_v7.md
    ├── SEO_V7_MIGRATION_REPORT_FULL.md
    └── SEO_V7_MIGRATION_REPORT_LITE.md
```

## Release process

1. Update the package contents.
2. Run package validation.
3. Confirm controller and module metadata.
4. Rebuild all four ZIP files.
5. Generate detached SHA-256 hashes.
6. Update the changelog.
7. Publish the ZIP files and checksum file in a GitHub Release.
8. Tag the release using a version such as:

```text
v7.1.0
```

## License

This project is licensed under the MIT License.

You may use, copy, modify, merge, publish, distribute, sublicense, and reuse this project, including for commercial purposes, provided that the original copyright and license notice are retained.

Copyright (c) 2026 Reza DaliriRad (rdaliri)

See [LICENSE](LICENSE) for the full license terms.


## Contributing

Contributions should preserve:

- single-controller authority
- evidence-state definitions
- retry and stop rules
- QA thresholds
- Full/Lite separation
- Flat/Modular equivalence
- Module 08 image handoff
- task-only module boundaries

Changes to governance should include:

- rationale
- affected files
- migration notes
- validation updates
- new detached checksums

## Security and responsible use

This system does not replace professional legal, medical, financial, accessibility, privacy, or regulatory review.

Do not use it to:

- fabricate evidence
- invent experts or credentials
- create fake first-party proof
- misrepresent AI-search testing
- publish unsupported technical findings
- produce misleading local pages or doorway content

## Release notes

### v7.1

- Added deterministic AEO answer-first controls
- Added measurable humanization rules
- Added GEO freshness, attribution, first-party proof, and citation-readiness actions
- Added explicit QA acceptance checks
- Corrected task-module metadata
- Standardized release metadata and package documentation
- Preserved controller and governance behavior

---

**Recommended default:** Lite Flat v7.1 for daily ChatGPT work.  
**Recommended advanced edition:** Full Modular v7.1 for repositories and automation.
