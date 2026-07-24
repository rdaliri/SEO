<!--
File: README.md
Version: 7.0-corrected-final
Classification: archive-only documentation
Authority: None
Required or optional: Optional
Controller dependency: None
May override controller: No
Source provenance: Legacy and provenance archive policy
-->

# Archive Policy

The release archive directory may contain only an index or README. Historical source packages are retained separately in controlled storage and are not required for normal v7 execution.

- Archived controllers must never be loaded with v7.
- This folder is provenance storage only.
- Archive contents are inactive and cannot override the active controller.
- No file in this directory is an execution dependency.
- Absence of legacy source files from this directory is intentional for the clean release.


This archive folder is not an execution dependency.
