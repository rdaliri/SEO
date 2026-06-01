# Mode Activation Rules

## Purpose
This file defines when to activate each production mode and how strict the AI should be.

---

# 1. Strict Mode

## Activate When
- High-value landing page
- Pillar page
- Main service page
- Homepage
- Core commercial page
- Legal/financial/medical/high-trust content

## Requirements
- Full intent classification
- Full entity mapping
- Full brief validation
- Approval gates required
- Technical QA required
- Final audit required

## Shortcuts Allowed
None unless user explicitly overrides.

---

# 2. Fast Production Mode

## Activate When
- User needs quick draft
- Low-risk supporting article
- Internal draft only
- User already has complete brief

## Requirements
- Intent classification
- Brief validation
- Draft
- Humanization
- Lightweight audit

## Shortcuts Allowed
- Combine brief + draft
- Combine humanization + audit

## Must Disclose
- Which checks were compressed
- What should be reviewed before publishing

---

# 3. Bulk Production Mode

## Activate When
- Multiple pages/articles are requested
- Programmatic or repeatable content set
- City/service/category expansion

## Requirements
- Batch architecture
- Template approval
- Sample output approval
- Duplicate risk control
- Batch QA

## Critical Rule
Do not generate a full batch before one approved sample exists.

---

# 4. Local SEO Mode

## Activate When
- Content targets local search
- City or region page
- Service-area page
- Local pack ranking goal
- Google Business Profile support content

## Requirements
- Geographic intent classification
- NAP consistency check
- Local entity reinforcement
- Duplicate local page prevention
- Local schema recommendation
- Unique local proof requirement

## Shortcut Risk
High. Local pages become duplicate quickly.

---

# 5. Authority Content Mode

## Activate When
- Thought leadership
- Expert guide
- Competitive SERP
- Content meant to build topical authority

## Requirements
- Entity map
- Competitor gaps
- original insights/proof requirements
- strong internal linking
- EEAT layer

---

# 6. Conversion-Focused Mode

## Activate When
- Lead generation page
- Product/service sales page
- Paid traffic landing page
- Quote/request page

## Requirements
- CTA strategy
- trust signals
- objection handling
- mobile CTA placement
- conversion section audit

---

# 7. Refresh Mode

## Activate When
- Existing content is outdated
- Rankings declined
- CTR declined
- Competitors improved
- Content is thin or duplicated

## Requirements
- Content decay review
- Update priority level
- Rewrite plan
- Technical QA
- Final audit
