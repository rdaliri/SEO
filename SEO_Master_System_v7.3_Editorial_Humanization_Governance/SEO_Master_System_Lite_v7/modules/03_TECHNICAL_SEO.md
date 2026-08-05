<!--
File: 03_TECHNICAL_SEO.md
Version: 7.1-seo-aeo-geo-humanize
Classification: active task module
Authority: task execution under the controller
Required or optional: required when routed
Controller dependency: SEO_MASTER_CONTROLLER_LITE_v7.md
May override controller: No
Source provenance: v7 active task module derived from v6 with selected Elite v4 specialist guidance
-->

# Module 03: Technical SEO

## Objective
Verify or specify crawlability, indexability, canonicalization, rendering, metadata, links, structured data, images, and performance requirements.

## Rules
1. Check only what available access supports.
2. Do not infer code-level implementation from copy, mockups, screenshots, or briefs.
3. Separate observed defects from recommendations.
4. Treat structured-data eligibility and validity as separate checks.
5. Prioritize discovery, indexation, rendering, duplication, and critical UX blockers.
6. Include evidence and a retest method for each failed, recommended, or untested check.

## Deliverable
Audit table with check, status, evidence, impact, fix, owner, retest; blockers; implementation specifications; validation checklist.

## v7 Specialist Guidance
Check technical accessibility where relevant:
- crawlability, indexability, canonical status, rendered main content, and HTTP response
- content availability without login, blocked tabs, or unsupported client-side dependencies
- heading hierarchy, keyboard/accessibility implications, descriptive links, image alternatives, and visible-content/schema alignment
- snippet or extraction controls when AI-search visibility is an objective
Mark every unchecked item `NOT TESTED`; never claim implementation or validation without observation.
