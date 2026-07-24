# START HERE — Full v6 Flat

## Use This Package in ChatGPT
Load files in this order:

1. `SEO_MASTER_CONTROLLER_v6.md` — sole authority
2. `CANONICAL_PROJECT_CONTEXT_v6.md` — approved project facts and current task
3. Only the task module(s) needed from the list below
4. `MODULE_07_QA_AND_RECOVERY.md` for final QA, verdict, or defect repair

## Task Modules
- `MODULE_01_INTENT_ARCHITECTURE.md`
- `MODULE_02_CONTENT_PRODUCTION.md`
- `MODULE_03_TECHNICAL_SEO.md`
- `MODULE_04_LOCAL_AND_SCALED_CONTENT.md`
- `MODULE_05_CONTENT_LIFECYCLE.md`
- `MODULE_06_AI_SEARCH_VISIBILITY.md`
- `MODULE_07_QA_AND_RECOVERY.md`
- `MODULE_08_IMAGE_GENERATION.md`

## Execution Instruction
After loading the files, give ChatGPT the task and state: **Use the controller as the sole authority, select the minimum required modules, execute the bounded QA loop, and return the required verdict output.**

## Do Not Load Together
- Do not load another controller, orchestration prompt, execution guide, production-mode prompt, or QA-governance prompt.
- Do not load the Full and Lite controllers together.
- Do not load v4 or v5 controller files with this package.
- Reference files are not required for execution.

## Flat vs Modular
This flat edition contains the same active logic as the modular package, but every executable file is at the package root. The original modular package remains preferable for file-aware systems that reliably discover subfolders.

## Image Production
For content deliverables, also load `MODULE_08_IMAGE_GENERATION.md`. It runs after the content output and before `MODULE_07_*` final QA. Skip it only when the task has no publishable image requirement, and record the reason.
