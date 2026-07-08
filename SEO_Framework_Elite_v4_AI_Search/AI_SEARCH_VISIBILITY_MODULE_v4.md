# AI Search Visibility Module v4

## Purpose

This module upgrades the SEO framework for the new search environment where visibility is distributed across classic search engines, AI overviews, answer engines, and conversational search systems.

The main shift is from ranking alone to source eligibility.

A page must be:

- Crawlable
- Indexable
- Snippet-eligible
- Text-accessible
- Entity-clear
- Evidence-backed
- Internally connected
- Useful for humans
- Structured enough for AI extraction

---

## Core Principle

AI search systems do not only match keywords. They retrieve, compare, summarize, and cite sources based on relevance, clarity, trust, freshness, and accessibility.

Treat every important page as a possible source document for an AI-generated answer.

---

## AI Search Optimization Layers

| Layer | Question To Ask | Required Action |
|---|---|---|
| Crawlability | Can bots access the page? | Check robots.txt, server status, sitemap, canonical |
| Indexability | Can the page appear in search systems? | Check index tags, canonicalization, duplicate content |
| Extractability | Can AI understand the answer quickly? | Use BLUF summaries, headings, lists, tables, FAQs |
| Entity Clarity | Can AI understand who/what the page is about? | Use consistent brand, service, location, and audience terms |
| Trust | Would AI and humans trust this page? | Add proof, author credentials, sources, case studies |
| Fan-Out Coverage | Does the page answer related AI sub-queries? | Map and answer definition, comparison, cost, process, proof, objections |
| Freshness | Is the content current? | Add meaningful update notes and refresh outdated sections |
| Internal Authority | Does the site support the topic? | Link to related service, case study, FAQ, location, and comparison pages |

---

## Query Fan-Out Workflow

For every important topic, map the primary query into supporting sub-queries.

Example:

Primary query:

```text
best web agency for custom development and high-end animations
```

Possible fan-out queries:

```text
custom web development agency
GSAP animation agency
high-performance WordPress development
web agency portfolio examples
web agency case studies
web development pricing
secure WordPress architecture
conversion-focused web design
best agency for premium websites
```

The page or topic cluster should answer these sub-queries directly.

---

## AI Search Query Bank

Use this query bank for recurring visibility tests.

```markdown
| Category | Query Template | Goal |
|---|---|---|
| Branded | Is [Brand] good for [service]? | Check brand understanding and sentiment |
| Category | Best [service] agencies for [audience] | Check recommendation visibility |
| Local | Best [service] company in [location] | Check location visibility |
| Technical | Who can build [technical requirement]? | Check capability visibility |
| Comparison | [Brand] vs [Competitor] | Check competitive positioning |
| Cost | How much does [service] cost? | Check pricing/cost factor coverage |
| Trust | Is [Brand] reputable? | Check proof and authority visibility |
| Use Case | Best [service] for [industry/use case] | Check niche relevance |
```

---

## AI Visibility Testing Table

```markdown
| Date | Platform | Query | Brand Mentioned? | Brand Cited? | Citation URL | Competitors Mentioned | Accuracy | Gap | Action |
|---|---|---|---|---|---|---|---|---|---|
|  | Google |  |  |  |  |  |  |  |  |
|  | ChatGPT Search |  |  |  |  |  |  |  |  |
|  | Bing/Copilot |  |  |  |  |  |  |  |  |
|  | Perplexity |  |  |  |  |  |  |  |  |
|  | Gemini |  |  |  |  |  |  |  |  |
```

---

## Content Gap Actions

If the brand is absent:

- Create or improve a service page with direct entity statements.
- Add proof, portfolio examples, case studies, or testimonials.
- Improve internal links from related pages.
- Create comparison, FAQ, or use-case pages.
- Make sure the page is crawlable and indexable.

If the brand is mentioned but inaccurate:

- Clarify entity statements on homepage, about page, service pages, and schema.
- Add consistent descriptions across the site.
- Update outdated claims.
- Strengthen author and organization signals.

If competitors are cited instead:

- Compare their cited pages against your page.
- Identify missing sections, proof, schema, freshness, or internal links.
- Build stronger topic clusters and supporting assets.

---

## Source Eligibility Checklist

```markdown
- [ ] Page returns 200 status
- [ ] Page is not blocked in robots.txt
- [ ] Page is indexable
- [ ] Canonical points to the correct URL
- [ ] Main content appears in rendered HTML
- [ ] Content is not hidden behind tabs, login walls, or heavy JavaScript
- [ ] Snippet controls do not block answer extraction unless intentional
- [ ] Page has clear H1/H2/H3 hierarchy
- [ ] First 100 words answer the main intent
- [ ] Page includes structured sections for fan-out questions
- [ ] Brand/entity/service/location relationships are clear
- [ ] Claims are supported by proof
- [ ] Internal links support the topic cluster
- [ ] Schema matches visible content
- [ ] Last updated date reflects real changes
- [ ] OAI-SearchBot is allowed if ChatGPT Search visibility is desired
- [ ] Googlebot and Bingbot are allowed
```

---

## Required AI Search Report Format

```markdown
# AI Search Visibility Report

## 1. Target Topic

## 2. Target Page

## 3. Primary Query

## 4. Fan-Out Query Map

## 5. Platform Test Results

## 6. Brand Accuracy Review

## 7. Competitor Citation Review

## 8. Content Gaps

## 9. Technical Access Issues

## 10. Recommended Actions

## 11. Priority

High / Medium / Low
```
