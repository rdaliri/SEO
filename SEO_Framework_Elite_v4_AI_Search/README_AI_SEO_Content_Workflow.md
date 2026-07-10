# README — AI SEO Content Workflow

This document explains the required execution order, decision points, approvals, and operational rules for using the SEO Content System in an AI-driven WordPress project.

The workflow is intentionally strict. It exists to prevent bad site structure, weak keyword targeting, keyword cannibalization, generic AI writing, and premature publishing.

---

## Purpose

This system is designed for a WordPress website where content production is AI-driven but final publishing authority remains with the SEO Lead.

The workflow ensures that every page or article is created in the correct sequence:

1. Structure first
2. Keywords second
3. Drafting third
4. Humanization fourth
5. Final audit fifth
6. SEO Lead approval before publishing

No content should skip steps.

---

## Roles

| Role | Responsibility |
|------|----------------|
| Content Team | Supplies business inputs, niche facts, page requirements, internal link targets, competitor context |
| AI System | Runs the prompts, validates missing inputs, drafts content, rewrites content, audits quality |
| SEO Lead | Approves site architecture, keyword map, final page/article draft, and publishing readiness |

---

## Core Rule

Nothing gets published unless all of the following are true:

- The site architecture was approved.
- The keyword map was approved.
- The content was drafted from a complete brief.
- The Anti-AI rewrite was applied.
- The final audit passed.
- The SEO Lead approved the final version.

If one step is missing, the content is not publish-ready.

---

## Execution Order

| Order | Phase | Mandatory? | Trigger | Output | Approval Required |
|------:|------|------------|---------|--------|-------------------|
| 1 | Phase 1 — Discovery & Site Architecture | Yes | Start of project | Site tree, page types, structure, internal link framework | SEO Lead |
| 2 | Phase 2 — Keyword Mapping & Content Hierarchy | Yes | After Phase 1 approval | Keyword map, page intent, cannibalization resolution | SEO Lead |
| 3 | Phase 3 — Page Content Generation | Yes for non-blog pages | Per page | Service page / landing / pillar / support page draft | SEO Lead later |
| 4 | Phase 5 — Blog Post Generation | Yes for blog pages | Per article | Blog brief validation + article draft | SEO Lead later |
| 5 | Phase 6 — Anti-AI Humanization Rewrite | Yes | After any draft | Rewritten expert-style draft | SEO Lead later |
| 6 | Phase 4 — Pre-Publish Quality Check | Yes | After rewrite | Final audit verdict | SEO Lead |
| 7 | Publish to WordPress | Yes | Only after approval | Live content | SEO Lead final go-ahead |

Important: Phase 4 happens after Phase 6, not before it.

---

## Priority Logic

The AI system must follow this priority order when deciding what to do next:

### Priority 1 — Missing prerequisites
If site structure or keyword mapping is not approved, stop everything. Do not allow drafting.

### Priority 2 — Missing required inputs
If a page or article brief is incomplete, challenge the team and collect the missing information before writing.

### Priority 3 — Structural conflicts
If keyword overlap or page-purpose conflict exists, stop and resolve cannibalization before content creation.

### Priority 4 — Draft generation
Only draft after intent, page type, target keyword, reader profile, and conversion goal are clear.

### Priority 5 — Humanization
Every draft must go through Anti-AI Humanization Rewrite before final audit.

### Priority 6 — Final audit and approval
Only audited and approved content can move to publishing.

---

## Decision Tree

Use this logic for every request inside the project:

### If the project has not started yet
Run:
- Phase 1

### If Phase 1 is approved but keyword mapping is not approved
Run:
- Phase 2

### If the keyword map is approved and the page is not a blog post
Run:
- Phase 3
- Then Phase 6
- Then Phase 4
- Then SEO Lead review

### If the keyword map is approved and the page is a blog post
Run:
- Phase 5
- Then Phase 6
- Then Phase 4
- Then SEO Lead review

### If the draft already exists but sounds generic or AI-written
Run:
- Phase 6 only
- Then Phase 4 again
- Then SEO Lead review

### If the audit fails
Do not publish.
Return to the relevant earlier phase:
- Brief problem → go back to Phase 3 or Phase 5 inputs
- Tone/human-likeness problem → go back to Phase 6
- Structural/keyword problem → go back to Phase 2

---

## Phase-by-Phase Guidance

## Phase 1 — Discovery & Site Architecture
Use at the beginning of the project only.

Objective:
- Understand the business, market, audience, competitors, goals, geography, and content scope.
- Build the site tree before any content is written.

Do not proceed to keyword mapping until the SEO Lead approves the structure.

Failure risks if skipped:
- Wrong site hierarchy
- Weak URL strategy
- Duplicate topic coverage
- Internal linking confusion later

---

## Phase 2 — Keyword Mapping & Content Hierarchy
Use after site structure approval.

Objective:
- Assign one primary keyword per page.
- Define page intent.
- Prevent keyword cannibalization.
- Establish internal linking relationships between pillar and cluster pages.

Do not move to content drafting without approval.

Failure risks if skipped:
- Multiple pages targeting the same query
- Wrong page type for the keyword
- Weak search intent alignment
- Blog and service page overlap

---

## Phase 3 — Standard Page Drafting
Use for:
- Homepage sections if needed
- Service pages
- Landing pages
- Category pages
- Pillar pages
- Support pages

Use only after Phase 2 approval.

Required inputs:
- URL slug
- Primary keyword
- Page type
- Search intent
- Reader problem
- Conversion goal
- Required business facts
- Word count range
- Competitor context
- Internal links

After drafting, do not publish. Move to Phase 6.

---

## Phase 5 — Blog Drafting
Use only for blog/resource articles.

Objective:
- Support a pillar or category page.
- Match TOFU, MOFU, or BOFU-support intent.
- Answer a specific user query without colliding with commercial pages.

This phase includes its own validation step before drafting. That validation is mandatory.

After drafting, move to Phase 6.

---

## Phase 6 — Anti-AI Humanization Rewrite
Use after any draft from Phase 3 or Phase 5.

Objective:
- Remove machine-sounding language
- Remove filler phrases
- Break repetitive rhythm
- Prefer clear subjects and strong action verbs
- Keep one primary idea per sentence where practical
- Shorten sentences only when meaning, evidence, and nuance remain intact
- Add expert-level specificity
- Preserve SEO integrity while making the content read like a real specialist wrote it

This phase is mandatory for every final draft.

Failure risks if skipped:
- Content sounds synthetic
- Generic transitions remain
- Paragraph rhythm feels automated
- Expertise signals remain weak
- Final copy feels “correct” but not credible

---

## Phase 4 — Final Pre-Publish Audit
Use after Phase 6.

Objective:
- Validate technical SEO elements
- Check keyword placement and density
- Confirm internal links
- Confirm FAQ and schema
- Evaluate sentence quality and human-likeness
- Issue an approval, conditional approval, or rejection

Only after this phase may the SEO Lead sign off.

---

## Approval Gates

The following approval gates are non-negotiable:

| Gate | Required Before Next Step |
|------|----------------------------|
| Gate 1 | SEO Lead approval of Phase 1 before Phase 2 |
| Gate 2 | SEO Lead approval of Phase 2 before Phase 3 or Phase 5 |
| Gate 3 | Completion of Phase 6 before Phase 4 |
| Gate 4 | SEO Lead approval after Phase 4 before publishing |

If any gate is missing, the workflow is broken.

---

## Operational Rules for the AI Project

The AI running this system must obey these rules:

1. Never draft content before architecture and keyword approvals exist.
2. Never accept vague business descriptions without challenge.
3. Never accept duplicate or overlapping target keywords without flagging the problem.
4. Never generate content from missing or invented facts.
5. Never allow a draft to go to publication without humanization rewrite.
6. Never publish based only on draft completion.
7. Always return failed content to the correct earlier phase.
8. Always preserve Canadian English spelling.
9. Always treat the SEO Lead as the final authority.
10. Always assume WordPress is the publishing environment.
11. Use direct, verb-led sentences, but never sacrifice context, proof, nuance, or accuracy for brevity.
12. Vary sentence length and structure so the final copy reads naturally.

---

## Recommended Folder / Prompt Management Logic

For easier AI project handling, prompts should be stored and called in this logical order:

| File / Prompt | Purpose | When to Call |
|--------------|---------|--------------|
| Phase_1_Discovery_Architecture | Project setup | First |
| Phase_2_Keyword_Mapping | Keyword assignment and intent mapping | After architecture approval |
| Phase_3_Page_Generation | Standard pages | Per non-blog page |
| Phase_5_Blog_Generation | Blog articles | Per article |
| Phase_6_Anti_AI_Humanization | Rewrite and humanize draft | After every draft |
| Phase_4_Pre_Publish_Audit | Final audit | After rewrite |
| Master_Prompt_Kit | Reference only | Always available |
| README_AI_SEO_Content_Workflow | Process controller | Always available |

---

## Minimal Workflow Examples

### Example A — Service Page
1. Phase 1 approved
2. Phase 2 approved
3. Run Phase 3 for the service page
4. Run Phase 6 on the generated draft
5. Run Phase 4 on the rewritten draft
6. SEO Lead approves
7. Publish in WordPress

### Example B — Blog Article
1. Phase 1 approved
2. Phase 2 approved
3. Run Phase 5 for the article
4. Run Phase 6 on the generated article
5. Run Phase 4 on the rewritten version
6. SEO Lead approves
7. Publish in WordPress

### Example C — Failed Audit
1. Draft created
2. Rewrite completed
3. Audit says keyword intent is wrong
4. Return to Phase 3 or Phase 5 brief stage
5. Redraft
6. Rerun Phase 6
7. Rerun Phase 4
8. SEO Lead reviews again

---

## Final Publishing Checklist

Before any page or article goes live, confirm all items below:

- [ ] Site architecture approved
- [ ] Keyword mapping approved
- [ ] Correct phase used for this content type
- [ ] Full brief collected
- [ ] Draft generated
- [ ] Anti-AI rewrite completed
- [ ] Final audit completed
- [ ] SEO Lead approval recorded
- [ ] WordPress metadata ready (title, meta, slug, schema, internal links)
- [ ] Most sentences have a clear subject and a strong action verb
- [ ] Long sentences were split where clarity improved
- [ ] Sentence length varies naturally
- [ ] Concision did not remove evidence, context, or necessary qualifications

---

## Final Rule

This system is not a writing shortcut.
It is a quality-control workflow.

If speed conflicts with structure, structure wins.
If convenience conflicts with search intent, search intent wins.
If a draft looks finished but has not passed the workflow, it is not finished.

