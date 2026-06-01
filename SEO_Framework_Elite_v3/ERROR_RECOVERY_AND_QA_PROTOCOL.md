# Error Recovery & QA Protocol

## Purpose
This file defines what the AI should do when a workflow breaks, information is missing, or content quality fails.

---

# Core Recovery Rule

Do not hide problems. Do not continue blindly.

When an issue appears:

1. Identify the failure
2. Explain the risk
3. Mark severity
4. Recommend correction
5. Continue only when safe

---

# Severity Levels

## Critical
Blocks publishing.

Examples:
- wrong search intent
- keyword cannibalization
- duplicate local page
- unsupported legal/medical/financial claim
- missing primary keyword
- missing page purpose
- no indexability confirmation for publish-ready content

## Major
Must fix before final approval.

Examples:
- weak CTA
- thin sections
- missing internal links
- poor metadata
- weak entity coverage
- generic AI tone

## Minor
Can fix during final polish.

Examples:
- formatting issue
- repetitive phrasing
- weak transition
- minor heading improvement

---

# Recovery Actions

| Problem | Action |
|---|---|
| Missing input | Ask only for missing input or propose assumptions clearly |
| Conflicting keyword intent | Split into separate pages or choose one intent |
| Cannibalization | Merge, split, redirect, or retarget |
| Generic AI tone | Run Anti-AI Humanization |
| Thin content | Add useful sections, proof, examples, FAQs |
| Local duplication | Require unique local details and proof |
| Weak technical SEO | Run Technical SEO Governance |
| Unsupported claim | Remove or mark proof required |
| Over-optimization | Rewrite with semantic variation |

---

# QA Output Format

```text
QA VERDICT
Status: Pass / Conditional Pass / Fail
Severity: Critical / Major / Minor
Issues Found:
Fixes Required:
Safe To Publish: Yes / No
Next Action:
```
