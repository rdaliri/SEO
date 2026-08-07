<!--
File: IMAGE_PIPELINE_DEVELOPER_NOTE.md
Version: 7.4.1-search-policy-ranking-risk-governance
Classification: optional reference playbook
Authority: Operational documentation; non-authoritative
Required or optional: Optional
Controller dependency: Sole package controller
May override controller: No
Source provenance: v7 release documentation
-->

# Image Pipeline Developer Note

## Handoff
Trigger image production after the content module returns its approved draft or brief and before the controller invokes final QA. Pass the page type, content summary, audience, factual constraints, approved references, placement, and channel to Module 08.

## Variant Creation
Generate one primary prompt from the dominant content purpose. Create two alternatives by changing composition/viewpoint and style/crop without changing approved facts, subject identity, or commercial claims.

## Aspect Ratio Selection
Select from the placement requirement: typically 16:9 or 3:2 for hero/editorial, 1.91:1 or platform-required dimensions for social preview, 4:3 for explanatory inline visuals, and 1:1 only when the channel requires a square asset. Record exact pixel dimensions at implementation time.

## Storage
Store final files in the project's approved image or media directory using the recommended filename. Keep source files, final web assets, and social crops separate when the workflow supports them. Record the final URL or asset ID in the project evidence register after inspection.

## Fallback Metadata
When no image is rendered, generate proposed alt text and caption from the approved prompt and content purpose, label both `RECOMMENDED`, and mark the image `NOT TESTED`. After rendering, inspect the actual image and revise alt text or caption so they describe the final asset rather than the prompt.
