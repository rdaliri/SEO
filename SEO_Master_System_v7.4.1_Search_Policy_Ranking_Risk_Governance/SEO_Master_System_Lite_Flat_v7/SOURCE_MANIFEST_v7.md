<!--
File: SOURCE_MANIFEST_v7.md
Version: 7.4.1-search-policy-ranking-risk-governance
Classification: optional release/reference documentation
Authority: non-authoritative
Required or optional: Optional
Controller dependency: selected package controller
May override controller: No
Source provenance: v7.4.1 integrated release manifest
-->

# Source Manifest v7.4.1

## Release metadata

- Release: `7.4.1`
- Release date: `2026-08-07`
- Architecture: one authoritative controller per package; Full/Lite and Flat/Modular remain separate profiles.
- Module 09: active editorial humanization, batch-similarity, and optional detector-result governance.
- Module 10: active search-policy and ranking-risk governance.

## Active capability map

| Capability | Active owner | Authority status |
|---|---|---|
| Routing, evidence, severity, retries, verdict | Selected controller | authoritative |
| Intent architecture | Module 01 | task module |
| Content production | Module 02 | task module |
| Technical SEO / structured-data implementation | Module 03 | task module |
| Local and scaled-content defensibility | Module 04 | task module |
| Lifecycle, migration, redirect decisions | Module 05 | task module |
| AI-search / GEO / citation readiness | Module 06 | task module |
| Final specialist QA | Module 07 | task module |
| Image prompt package | Module 08 | task module |
| Humanization, batch similarity, detector governance | Module 09 | task module |
| Search-policy compliance and ranking-risk governance | Module 10 | task module |

## Module 09 integration

Module 09 supports:

- Mode A: direct single-asset editorial humanization audit;
- Mode B: related-batch similarity/originality audit;
- Mode C: governance of supplied external detector results, added only after the direct audit.

External detector scores are optional and cannot prove authorship or independently determine approval.

## Module 10 integration

Module 10 is automatically routed when publication/indexation or material search-policy/ranking risk applies. It coordinates spam-policy, people-first, structured-data, link, reputation, scaled-content, migration, security, ranking-drop, and recovery gates.

For publication/indexation work, Module 09 findings must reach Module 10 before final Module 07 QA when Module 10 triggers apply.

## Legacy provenance

The v7 system retains useful specialist concepts from earlier Full/Lite v6 and Elite v4 sources, but legacy controllers, orchestration prompts, alternate QA authorities, and mode-activation systems are excluded from active authority. Context/memory guidance remains in canonical project context and optional reference playbooks; it is unrelated to the current Module 09 humanization function.

## Release evidence

See the package validation report, release validation report, changelog, migration report, and checksums.
