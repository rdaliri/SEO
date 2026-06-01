# AI Context & Memory Rules

## Purpose
This file tells the AI what information must be preserved, summarized, or discarded during long SEO workflows.

---

# 1. Persistent Context

The AI must preserve these items exactly unless the user changes them:

- Target country/language
- Business/site category
- Audience
- Brand voice
- Primary keyword
- Secondary keywords
- Search intent
- Content type
- Production mode
- Approved page purpose
- Approved keyword map
- Approved site architecture
- Internal link targets
- CTA objective
- Required proof points
- Forbidden phrases
- Forbidden claims
- Compliance limitations

---

# 2. Compressible Context

The AI may summarize:

- Competitor observations
- Draft history
- optional examples
- alternate headings
- rejected variations
- previous audit notes after fixes are applied

---

# 3. Disposable Context

The AI may discard:

- abandoned wording
- failed title options
- temporary brainstorms
- unused content angles
- duplicate FAQ ideas

---

# 4. Context Carry-Forward Format

At the end of every major phase, the AI should produce this compact memory block:

```text
SEO CONTEXT SNAPSHOT
Project/Content Type:
Production Mode:
Target Country/Language:
Audience:
Primary Intent:
Primary Keyword:
Secondary Keywords:
Required Entities:
Approved Page Purpose:
CTA Objective:
Internal Links:
Proof Required:
Constraints:
Next Step:
```

Use this snapshot as the input for the next phase.

---

# 5. Drift Prevention Rules

The AI must not:

- change the primary keyword without approval
- change the search intent without approval
- change the page type without approval
- add unsupported claims
- remove required proof points
- change target language/country
- invent business facts

If drift is detected, stop and restore from the latest SEO Context Snapshot.
