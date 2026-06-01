# Prompt Orchestration Map

## Purpose
This file defines the exact order for using the prompts and modules in the framework.

Use this to prevent confusion about when and how each prompt should be used.

---

# Standard Full Workflow

## Step 0 — Master Controller
Use: `AI_WORKFLOW_KERNEL_MASTER_CONTROLLER.md`

Goal:
- Identify task type
- Select production mode
- Determine state
- Route next prompt

Output:
- Current State
- Mode
- Next Prompt
- Missing Inputs
- Approval Gate

---

## Step 1 — Discovery & Site Architecture
Use: Phase 1 prompt from `SEO_Content_System_Complete_Prompt_Kit.md`

Use when:
- Starting a new website
- Building full content strategy
- Creating site-wide SEO plan

Do not use when:
- User only needs one isolated article and already has keyword/brief

Output:
- Site structure
- Page types
- Navigation logic
- Topic hierarchy
- Internal link framework

Approval:
- Required

---

## Step 2 — Keyword Mapping & Content Hierarchy
Use: Phase 2 prompt from `SEO_Content_System_Complete_Prompt_Kit.md`

Enhance with:
- `SEARCH_INTENT_AND_ENTITY_SYSTEM.md`

Output:
- Primary keyword per page
- Secondary keywords
- Search intent
- Cannibalization warnings
- Entity requirements

Approval:
- Required

---

## Step 3 — Content-Type Selection
Use: `PRODUCTION_MODES_FRAMEWORK.md`

Classify content as:
- Landing page
- Local page
- Blog post
- Pillar page
- Category page
- Product/service page
- Comparison page
- Refresh/update

Output:
- Content type
- Mode
- Required structure
- QA depth

---

## Step 4 — Brief Validation
Use: Page or Blog generation prompt from `SEO_Content_System_Complete_Prompt_Kit.md`

Before writing, verify:
- Primary keyword
- Search intent
- Audience
- CTA
- Internal links
- Proof points
- Required claims
- Forbidden claims

If local:
Also use `LOCAL_SEO_ARCHITECTURE_MODULE.md`

If technical:
Also use `TECHNICAL_SEO_GOVERNANCE.md`

---

## Step 5 — Draft Generation
Use:
- Phase 3 for pages
- Phase 5 for blogs

Rules:
- Use approved brief only
- Do not change strategy
- Do not invent proof
- Do not keyword stuff
- Use semantic coverage instead of density

Output:
- Full draft
- Metadata draft
- Suggested FAQs
- Internal link suggestions
- CTA placement

---

## Step 6 — Anti-AI Humanization
Use: Phase 6 prompt from `SEO_Content_System_Complete_Prompt_Kit.md`

Goal:
- Remove robotic tone
- Remove filler phrases
- Improve sentence rhythm
- Increase human readability
- Preserve SEO structure

Output:
- Humanized version
- Notes on what changed

---

## Step 7 — Technical SEO Governance
Use: `TECHNICAL_SEO_GOVERNANCE.md`

Check:
- Title tag
- Meta description
- URL slug
- Schema
- Internal links
- Image ALT text
- Canonical
- Indexability
- Mobile readiness

Output:
- Technical QA checklist
- Pass/fail items
- Fixes required

---

## Step 8 — Final Audit
Use: Phase 4 prompt from `SEO_Content_System_Complete_Prompt_Kit.md`

Output:
- Editorial score
- SEO score
- Technical score
- Local SEO score if applicable
- Publish verdict

Approval:
- Required before publishing

---

# Local SEO Workflow

Use this route when the content targets a city, region, service area, or local pack intent.

1. Master Controller
2. Local SEO Architecture Module
3. Search Intent & Entity System
4. Keyword Mapping
5. Local Brief Validation
6. Draft Generation
7. Anti-AI Humanization
8. Technical SEO Governance
9. Local Duplicate Risk Audit
10. Final Audit

---

# Existing Content Refresh Workflow

Use this route when improving a published page.

1. Master Controller
2. Content Lifecycle Management
3. Search Intent & Entity System
4. Technical SEO Governance
5. Refresh Brief
6. Rewrite/Update
7. Humanization
8. Final Audit

---

# Bulk Production Workflow

Use this route for high-volume content.

1. Master Controller
2. Production Modes Framework
3. Batch Keyword Map
4. Batch Brief Template
5. Draft one sample page
6. Audit sample page
7. Approve template
8. Generate batch
9. Run batch QA
10. Human review

Bulk rule:
Never generate a full batch before one sample passes audit.
