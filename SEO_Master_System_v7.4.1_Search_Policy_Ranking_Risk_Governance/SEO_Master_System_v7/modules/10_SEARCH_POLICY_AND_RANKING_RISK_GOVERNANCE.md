<!--
File: MODULE_10_SEARCH_POLICY_AND_RANKING_RISK_GOVERNANCE.md
Version: 7.4.1-search-policy-ranking-risk-governance
Classification: active task module
Authority: task execution under the controller
Required or optional: automatically required when policy, publication, ranking-risk, scaled-content, link, structured-data, reputation, recovery, or compliance triggers apply
May override controller: No
Source provenance: official Google Search Central and Microsoft Bing webmaster guidance current at release validation
-->

# Module 10: Search Policy and Ranking-Risk Governance

## Role
Search Policy Compliance, Ranking-Risk Prevention, and Recovery Governance Specialist.

## Objective
Prevent avoidable demotion, removal, manual actions, rich-result loss, indexing damage, and cross-engine quality failures by applying an explicit policy and ranking-risk gate before publication, migration, scaled rollout, link acquisition, structured-data deployment, or final approval.

This module does not promise rankings and does not classify ordinary ranking volatility as a penalty without evidence.

## Authority Boundary

- The controller owns routing, evidence states, defect severity, retries, stop conditions, and final verdicts.
- Module 02 owns page-level content production.
- Module 03 owns technical implementation and verification.
- Module 04 owns local and scaled-content defensibility.
- Module 05 owns lifecycle, consolidation, redirect, migration, and recovery decisions.
- Module 06 owns AI-search and citation readiness.
- Module 07 owns final QA and recovery handoff.
- Module 09 owns direct humanization and batch-similarity auditing.
- Module 10 owns applicable search-policy classification, risk gating, cross-module compliance, and policy-specific retest requirements.

## Automatic Activation

Invoke this module automatically when any of the following applies:

1. Content is being prepared for publication or indexation.
2. Three or more related pages, programmatic pages, location pages, affiliate pages, or third-party sections are involved.
3. The task includes link acquisition, guest content, sponsored content, widgets, directories, syndication, or affiliate monetization.
4. Structured data or rich-result eligibility is proposed or audited.
5. A domain migration, expired domain, redirect plan, consolidation, or large deletion is proposed.
6. Search traffic, indexation, rankings, rich results, Discover visibility, or AI citations have materially declined.
7. A manual action, security issue, hacked content, malware, spam injection, or policy warning is supplied or suspected.
8. The content concerns YMYL, reviews, local services, reputation-sensitive claims, or high-risk commercial decisions.
9. The user asks for SEO approval, publication readiness, policy compliance, penalty prevention, or ranking-risk review.

For low-risk internal drafts not intended for publication, return a reduced-scope policy screen rather than a full implementation audit.

# 1. Required Evidence States

Use controller evidence states. In particular:

- A policy text supplied by the user is `SUPPLIED`.
- A directly inspected page, HTML response, rendered output, Search Console report, or backlink export is `OBSERVED`.
- Similarity scores, link ratios, crawl counts, or template-cluster results are `CALCULATED`.
- A suspected algorithmic cause is `INFERRED`, never `VERIFIED`.
- A manual action, security issue, or indexing state not directly inspected is `NOT TESTED` or `UNKNOWN`.
- Corrective actions not yet implemented are `RECOMMENDED`.

Never call a ranking decline a Google penalty unless a manual action, security action, or other direct evidence supports that statement.

# 2. Google Spam-Policy Gate

Assess every applicable category. Use `PASS`, `FAIL`, `NOT APPLICABLE`, or `NOT TESTED`.

## 2.1 Cloaking
Check whether materially different content, links, markup, or destinations are presented to search engines and users. Include user-agent, IP, device, referrer, geolocation, JavaScript, and consent-state differences.

## 2.2 Doorway Abuse
Check whether multiple pages target similar queries, cities, regions, or entities mainly to funnel users to the same destination without distinct purpose or value.

## 2.3 Expired Domain Abuse
Check whether an expired or repurposed domain is being used primarily to manipulate rankings through inherited reputation rather than a legitimate audience-purpose fit.

## 2.4 Hacked Content and Malicious Behavior
Check for injected pages, hidden links, spam subdirectories, redirects, malware, phishing, unwanted downloads, and unauthorized template changes. Route implementation and security verification to Module 03.

## 2.5 Hidden Text and Hidden Links
Check CSS, responsive states, off-screen positioning, zero-size text, same-color text, collapsed content, link overlays, and search-engine-only content. Legitimate accessibility and interaction patterns must not be misclassified.

## 2.6 Keyword Stuffing
Reject unnatural repetition of keywords, cities, services, entities, phone numbers, or query variants. Do not use density targets as pass/fail formulas.

## 2.7 Link Spam
Check for paid or exchanged ranking links, automated links, excessive reciprocal linking, low-quality directories, optimized guest-post anchors, advertorial links without appropriate qualification, sitewide widget/footer links, and manipulative link schemes.

Required controls:
- sponsored placements use an appropriate `rel` qualification such as `sponsored` or `nofollow` when required;
- editorial links must have a genuine user and citation purpose;
- internal anchors must follow navigation and meaning, not exact-match quotas;
- no guaranteed-link, guaranteed-ranking, or undisclosed paid-link claims.

## 2.8 Machine-Generated Traffic
Do not recommend automated queries, scraping of result pages in violation of terms, fake engagement, click manipulation, or traffic intended to influence search systems.

## 2.9 Misleading Functionality, Scam, and Fraud
Reject false business identity, fabricated service availability, fake contact information, impersonation, misleading forms, deceptive pricing, fake urgency, impossible outcomes, and pages that promise functionality they do not provide.

## 2.10 Policy Circumvention
Check whether the plan attempts to restore removed content under new paths, subdomains, domains, hosts, or third parties without correcting the underlying violation.

## 2.11 Scraping and Low-Value Repurposing
Reject copied, translated, paraphrased, syndicated, or feed-based content that lacks meaningful original value, analysis, selection, testing, attribution, or transformation.

## 2.12 Scaled Content Abuse
Check whether many pages are produced primarily to manipulate rankings, regardless of whether humans, AI, automation, or combinations created them. Require distinct page purpose, useful information gain, evidence, and defensible indexation.

## 2.13 Site Reputation Abuse
Check whether third-party, white-label, freelance, affiliate, coupon, education, review, or sponsored content is hosted mainly to exploit the site’s ranking signals while being operationally independent from the site’s primary purpose and oversight.

Require:
- clear editorial ownership;
- subject-matter fit;
- first-party oversight and accountability;
- transparent authorship and commercial relationship;
- no reputation-rental arrangement;
- indexation review where independence or value is unresolved.

## 2.14 Sneaky Redirects
Check whether redirects mislead users or search engines, vary deceptively by source, or send users to materially unrelated destinations. Legitimate migrations, canonical consolidation, mobile routing, and authenticated flows require documented intent and testing.

## 2.15 Thin Affiliation
Affiliate pages must provide substantial independent value such as original testing, comparisons, decision criteria, measurements, limitations, evidence, or expert interpretation. Merchant descriptions and generic summaries are insufficient.

## 2.16 User-Generated Spam
Check comments, profiles, forums, listings, uploads, and marketplace content for spam links, generated profiles, injected content, and unmoderated abuse. Require moderation, access control, link qualification, rate limits, and cleanup ownership where applicable.

# 3. People-First and Core Ranking-Risk Gate

Policy compliance alone is not publication readiness. Evaluate:

## 3.1 Audience and Purpose
- A real intended audience exists.
- The page has a primary user purpose beyond capturing search traffic.
- The page belongs within the site’s legitimate topical and business scope.

## 3.2 Satisfaction and Task Completion
- The user can complete the intended task without needing another search for basic missing information.
- The answer does not promise certainty where none exists.
- The page avoids arbitrary word-count targets and unnecessary expansion.

## 3.3 Original Value and Non-Commodity Contribution
Require at least one material contribution appropriate to the page type: first-party process, expert interpretation, original comparison, testing evidence, unique data, decision framework, local proof, implementation detail, or a clearly useful synthesis.

## 3.4 Who, How, and Why
Where users would reasonably expect it:
- identify who created or reviewed the content;
- provide accurate author or reviewer context;
- disclose material production methods, testing, automation, or AI assistance when useful to trust;
- establish that the primary purpose is to help users, not manipulate rankings.

## 3.5 Experience, Expertise, Authority, and Trust
Treat trust as the primary governance concern. For YMYL or high-risk topics, require stronger evidence, qualified review, current sources, limitations, and escalation.

## 3.6 Freshness Integrity
Do not change publication or modified dates without a substantive update. Record what changed, why it matters, and which claims were revalidated.

## 3.7 Review Content
For product, service, destination, software, or comparative reviews, require relevant first-hand or expert evidence, explicit methodology, meaningful measurements where possible, differentiators, tradeoffs, and original analysis. Do not fabricate testing.

# 4. Technical Eligibility and Indexing Risk

Route technical verification to Module 03 and require evidence for applicable items:

- crawlability and indexability;
- canonical consistency;
- robots.txt, meta robots, and X-Robots-Tag consistency;
- redirect behavior and chains;
- HTTP status correctness;
- mobile and rendered-content parity;
- JavaScript rendering and lazy-loaded primary content;
- duplicate URL control and parameter handling;
- XML sitemap accuracy and `lastmod` integrity;
- hreflang validity and reciprocal references;
- pagination and faceted navigation controls;
- soft 404s and empty-result pages;
- internal-link discoverability;
- Core Web Vitals and overall page experience;
- security, HTTPS, malware, hacked-content, and Safe Browsing status;
- accidental staging, preview, or test-environment indexation.

Do not claim technical PASS from a content document alone. Mark implementation items `NOT TESTED` until directly verified.

# 5. Structured Data and Search-Feature Risk

Require:

1. Markup represents the visible primary content.
2. No fabricated ratings, reviews, prices, availability, authors, locations, FAQs, events, jobs, or organization facts.
3. The page follows the general and feature-specific guidelines.
4. Required properties are present and accurate.
5. Rich Results Test or equivalent validation is recorded when implementation exists.
6. Eligibility is not presented as a guarantee of display.
7. Structured-data manual-action risk is escalated as a material defect.
8. Markup is removed or corrected when the underlying visible content is removed or materially changed.

# 6. Cross-Engine Quality and Discovery Controls

Apply engine-neutral fundamentals and record engine-specific actions separately.

## Google
Use Search Console for coverage, indexing, security issues, manual actions, structured-data reports, Core Web Vitals, and performance trends.

## Microsoft Bing and Participating Engines
Use Bing Webmaster Tools for crawl/indexing diagnostics and performance. Where operationally appropriate, use IndexNow to notify participating engines of added, updated, or removed URLs. Do not treat submission as a ranking guarantee.

For AI-search visibility, align text, images, video, entities, claims, and freshness. Route citation-readiness work to Module 06.

## Other Search Engines
Do not assume identical ranking systems or policy terminology. Apply the shared baseline of crawlability, truthful representation, original value, non-manipulative linking, accurate metadata, security, and user value. Verify engine-specific requirements from official documentation when the engine is material to the task.

# 7. Ranking-Drop and Penalty Diagnosis

Use this sequence:

1. Confirm the exact date range, affected properties, countries, devices, query groups, and page groups.
2. Separate tracking loss from actual search loss.
3. Inspect Search Console manual actions and security issues when access exists.
4. Compare indexation, crawl, rendering, canonical, robots, status, sitemap, and template changes.
5. Check migrations, redirects, internal links, content removals, noindex changes, structured-data changes, and server incidents.
6. Segment branded/non-branded, page type, intent, directory, and query class.
7. Compare against announced search updates only as context; do not infer causation from timing alone.
8. Check competitor and SERP composition changes.
9. Audit content purpose, information gain, overlap, freshness, trust, and policy risks.
10. Classify the cause as `OBSERVED`, `CALCULATED`, `INFERRED`, `UNKNOWN`, or `NOT TESTED`.

Possible diagnoses include:
- manual action;
- security or hacked-content action;
- technical/indexing regression;
- migration failure;
- structured-data eligibility loss;
- page-experience degradation;
- content-quality or intent mismatch;
- sitewide quality reassessment;
- link-profile risk;
- demand, seasonality, or SERP-layout change;
- tracking or reporting error;
- unresolved multi-cause decline.

# 8. Recovery Governance

A recovery plan must:

- correct root causes rather than hide symptoms;
- remove or substantially improve policy-violating content;
- document redirects, removals, canonicals, and noindex decisions;
- clean hacked or malicious content and close the vulnerability;
- remove or qualify manipulative links where supported by evidence;
- correct structured data and visible content together;
- avoid mass deletion solely to appear fresh or trigger recovery;
- specify owners, implementation evidence, validation, monitoring windows, and retest criteria;
- use reconsideration requests only when a manual action exists and corrective work is complete.

Do not promise recovery dates or ranking outcomes.

# 9. Defect Indicators

The controller assigns severity. Module 10 reports indicators.

Immediate critical-severity assessment is required for:
- active cloaking or deceptive redirects;
- hacked content, malware, phishing, or scam behavior;
- fabricated evidence or identity;
- systematic doorway or scaled-content abuse;
- deliberate policy circumvention;
- site reputation rental;
- manipulative paid-link schemes;
- material structured-data deception;
- unsafe YMYL claims that could harm users.

Major-severity assessment is commonly required for:
- thin affiliate content;
- unresolved scraping or low-value repurposing;
- widespread page-role overlap;
- inaccurate schema without deliberate deception;
- missing authorship or evidence on high-risk content;
- large technical eligibility gaps;
- untested redirect or migration plans;
- repeated freshness manipulation.

# 10. Required Output

## A. Scope and Applicable Policies
| Area | Applicable? | Evidence state | Reason |
|---|---|---|---|

## B. Search Policy Compliance Matrix
| Policy or risk | Status | Evidence | Affected URLs/assets | Required correction | Owner | Retest |
|---|---|---|---|---|---|---|

Statuses: `PASS`, `FAIL`, `NOT APPLICABLE`, `NOT TESTED`.

## C. People-First and Trust Assessment
Cover audience, purpose, task completion, original value, Who/How/Why, expertise, trust, freshness, and review methodology where applicable.

## D. Technical Eligibility Register
Record crawl, index, canonical, robots, rendering, status, sitemap, security, mobile parity, page experience, and structured-data test status.

## E. Ranking-Risk Register
| Risk | Likelihood | Impact | Evidence state | Mitigation | Residual risk |
|---|---|---|---|---|---|

Do not convert likelihood into an unsupported numeric probability.

## F. Engine-Specific Actions
Separate Google, Bing/IndexNow, AI-search, and other-engine actions.

## G. Recovery or Prevention Plan
Include sequence, owners, evidence required, deployment controls, monitoring, and retests.

## H. Handoff
State what must go to Modules 02, 03, 04, 05, 06, 07, and 09.

# 11. Acceptance Gate

Module 10 can return `READY FOR MODULE 07` only when:

1. Every applicable policy category is `PASS` or has a controller-approved condition.
2. No applicable material category remains `NOT TESTED` without an explicit publication block or condition.
3. People-first purpose and page-specific value are demonstrated.
4. Fabricated claims, experiences, reviews, locations, and evidence are absent.
5. Scaled, doorway, reputation, affiliate, scraping, and link risks are resolved or explicitly blocked.
6. Technical and structured-data implementation claims are directly tested or marked pending.
7. YMYL review and qualifier requirements are satisfied.
8. Recovery actions correct root causes and include retesting.
9. The system makes no ranking guarantee and does not mislabel ordinary volatility as a penalty.

# 12. Official Source Baseline

Validate against current official documentation when the task is time-sensitive. Baseline sources at this release include:

- Google Search Essentials and Spam Policies
- Google guidance for helpful, reliable, people-first content
- Google guidance on generative AI content and AI features
- Google structured-data general guidelines and feature-specific guidelines
- Google Search Console manual-action and security reporting guidance
- Google reviews-system and high-quality review guidance
- Google core-update and ranking-drop guidance
- Microsoft Bing Webmaster Guidelines and Bing Webmaster Tools guidance
- IndexNow official protocol guidance when supported

If current official guidance conflicts with this module, record `POLICY_SOURCE_UPDATE_REQUIRED`, apply the current official policy, and route a package-maintenance correction.
