<!--
File: MODULE_06_AI_SEARCH_VISIBILITY.md
Version: 7.1-seo-aeo-geo-humanize
Classification: active task module
Authority: task execution under the controller
Required or optional: required when routed
Controller dependency: SEO_MASTER_CONTROLLER_LITE_v7.md
May override controller: No
Source provenance: v7 AI-search module with active GEO production actions
-->

# Module 06: AI Search Visibility

## Objective
Assess whether content is accessible, semantically clear, evidence-rich, and suitable for retrieval or citation without promising inclusion.

## Rules
1. Separate foundational SEO from platform-specific tests.
2. Platform results require platform, query, date, locale/account context, and direct observation.
3. Never infer inclusion, exclusion, citation, or ranking from general page quality.
4. Evaluate access controls, entity clarity, answer extractability, source quality, claim provenance, freshness, unique information, query fan-out, and ambiguity.
5. Frame improvements as citation-readiness recommendations, not outcome guarantees.

## Deliverable
Query/answer coverage; evidence and citation-readiness; technical access; observed platform results or untested status; priorities and retest plan.

## v7 Specialist Guidance
### Query Fan-Out
Map the primary query into relevant definition, comparison, cost, process, risk, proof, local, technical, objection, and use-case sub-queries. Include only sub-queries that support the page role.

### Source Eligibility
Evaluate, when evidence is available: crawlability, indexability, extractability, entity clarity, proof, freshness, internal authority, visible-content accessibility, and schema alignment. Unchecked items remain `NOT TESTED`.

### AI-Search Testing
For observed platform tests, record date, platform, exact query, mention/citation status, citation URL, competitor presence, accuracy, gap, and action. Do not simulate platform results or claim citation visibility without direct testing.

Detailed test templates are in `REFERENCE_QUERY_FANOUT_AND_SOURCE_ELIGIBILITY_v7.md`.

## GEO Production Actions

Apply these actions whenever AI-search visibility, citation-worthiness, recency, or credibility materially affects the deliverable.

### Freshness
- Add a visible “last reviewed,” “last updated,” or equivalent freshness note when the topic changes materially over time.
- Record the review date and the evidence used to support current claims.
- Do not imply freshness when the underlying evidence is old, incomplete, or `NOT TESTED`.
- For fast-changing topics, flag claims that require scheduled revalidation.

### Expertise and attribution
Recommend or include author, reviewer, or subject-matter expert attribution when credibility depends on professional expertise, firsthand experience, legal or medical review, technical authority, or local knowledge.

Attribution must reflect a real supplied or verified person or role. Do not fabricate experts, credentials, biographies, quotes, or review activity.

### First-party proof
When original evidence is missing:
1. Identify what first-party proof would materially strengthen the page.
2. Request or recommend collection of that proof, such as internal data, original photos, process documentation, customer evidence, test results, expert commentary, or local verification.
3. Until obtained, substitute only eligible third-party evidence and label remaining limitations.
4. Do not present substitute evidence as first-party proof.

### Citation-readiness
A claim is citation-ready only when:
- the claim is specific and clearly worded,
- the source directly supports the claim,
- the source is eligible and current enough for the topic,
- attribution is unambiguous,
- qualifiers and limitations are preserved,
- the claim is not overstated beyond the evidence.

### Recency and credibility handling
For topics where AI-search visibility depends on recency or authority:
- prioritize current eligible sources,
- identify stale or weak evidence,
- recommend an update, expert review, or first-party validation,
- label unresolved items `NOT TESTED` or as pending verification,
- do not claim AI-search readiness until the required credibility signals are present.
