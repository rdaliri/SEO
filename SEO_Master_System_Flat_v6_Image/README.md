# SEO Master System Full v6 — Flat ChatGPT Edition

## Purpose
A flat, ChatGPT-friendly distribution of the Full v6 SEO system. It removes subfolder-routing dependency without changing controller authority, evidence states, missing-data behavior, retries, conflict escalation, defect definitions, QA thresholds, or verdict rules.

## Primary Controller
`SEO_MASTER_CONTROLLER_v6.md` is the sole authority. No module may override it.

## Required Files
Always load:
1. `START_HERE.md`
2. `SEO_MASTER_CONTROLLER_v6.md`
3. `CANONICAL_PROJECT_CONTEXT_v6.md`

Then load only the required task module(s). Use `MODULE_08_IMAGE_GENERATION.md` for publishable content, followed by `MODULE_07_QA_AND_RECOVERY.md` for final validation or repair.

## Active Task Modules
- `MODULE_01_INTENT_ARCHITECTURE.md`
- `MODULE_02_CONTENT_PRODUCTION.md`
- `MODULE_03_TECHNICAL_SEO.md`
- `MODULE_04_LOCAL_AND_SCALED_CONTENT.md`
- `MODULE_05_CONTENT_LIFECYCLE.md`
- `MODULE_06_AI_SEARCH_VISIBILITY.md`
- `MODULE_07_QA_AND_RECOVERY.md`

## Optional / Reference-Only Files
- `REFERENCE_SEO_SYSTEM_AUDIT_REPORT_v6.md` — design and audit history
- `REFERENCE_SOURCE_MANIFEST_v6.md` — provenance and file mapping

Do not load reference-only files for normal production runs.

## Flat ChatGPT-Friendly Usage
1. Upload the required files from this package.
2. Load the controller first, then project context, then the minimum task modules.
3. Provide the requested deliverable and source materials.
4. Require the controller's bounded execution loop and final verdict.
5. Update the project context and evidence register after approved work.

The flat package has no nested folders and no dependency on subfolder discovery.

## Modular File-Aware Usage
Use the original `SEO_Master_System_v6.zip` when the environment reliably discovers and routes files inside `/modules`. The modular version is the canonical organizational structure for repositories, agents, or file-aware workflows. Load order remains controller → context → minimum modules → QA module.

## Do Not Load Together
- Full v6 and Lite v6 controllers
- Flat and modular copies of the same controller in one run
- Any v4/v5 controller, orchestration, execution-guide, production-mode, context-governance, or separate QA-governance prompt

Duplicate task modules are also unnecessary. Choose either the flat package or the modular package for a run.

## System Choice
- **Full v6:** use for formal audits, complex multi-module work, detailed assumptions and verification registers, and higher audit-trail requirements.
- **Lite v6:** use for daily production, repeated page workflows, and lower formatting overhead while keeping the same safety thresholds and core governance.

## File Classification
- **Keep active:** controller, canonical context, task modules, QA module, `START_HERE.md`, and this README.
- **Flatten:** all active modules into root-level `MODULE_*.md` files.
- **Keep reference-only:** audit/refactor report and source manifest.
- **Archive:** prior v4/v5 systems and superseded v6 variants not used in the current run.
- **Delete from active workspace:** duplicate controllers and duplicate governance files. Preserve them elsewhere only when provenance is required.

## Image Generation Step
For publishable content, run image generation **after the content output and before final QA**:

1. Content module produces the draft, brief, or summary.
2. `modules/08_IMAGE_GENERATION.md` creates the image specification and metadata.
3. The QA module evaluates the combined content and image package.

Minimal publish assets:
- Hero image when a hero placement exists.
- Social preview image for public shareable content.
- Inline image only when needed for explanation, trust, comprehension, or conversion.

Optional assets: secondary inline visuals, decorative images, galleries, alternate crops, and extra social variants.

To regenerate, request a new image prompt or rendered variation and state which element may change: composition, viewpoint, style, lighting, palette, crop, or aspect ratio. Factual constraints, approved subject identity, and no-logo/no-real-person rules remain unchanged.

Record image work in the structured result or decision/control log:
- `SUPPLIED`: approved reference image or asset supplied by the user.
- `OBSERVED`: rendered image or reference directly inspected.
- `NOT TESTED`: prompt or proposed asset not yet rendered and inspected.
- `RECOMMENDED`: proposed prompt, filename, placement, alt text, caption, or structured-data entry.

### Image Policy
- Filename is descriptive and SEO-friendly.
- Format suits the publishing channel.
- Dimensions match the placement.
- Alt text is accurate and concise.
- Caption is short and useful when needed.
- License or usage note is recorded when relevant.
- Thumbnail or social-preview size is defined.
- Structured-data image entry is included when relevant and supported.

See `IMAGE_PIPELINE_DEVELOPER_NOTE.md` for automation wiring.
