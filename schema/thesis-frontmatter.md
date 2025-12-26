# Thesis Frontmatter Schema

Every thesis markdown file must include YAML frontmatter with the following fields:

## Required Fields

```yaml
---
slug: ai-knowledge-work          # URL-safe identifier (lowercase, hyphens)
title: "AI & Knowledge Work"     # Display title
status: active                   # active | evolving | challenged | archived
version: "2.4"                   # Semantic version (major.minor)
created: 2024-08-01              # ISO date of first publication
updated: 2024-12-26              # ISO date of last update
description: |                   # 1-3 sentence summary
  How AI transforms professional services, what it means for
  SMB owners doing $2-10M, and why the next 3 years will reshape
  how expertise is packaged and sold.
---
```

## Optional Fields

```yaml
---
connections:                     # Related thesis slugs
  - reshoring
  - demographics
tags:                            # Searchable tags
  - ai
  - professional-services
  - smb
key_claims:                      # Core falsifiable claims
  - "AI leverage ratios will matter more than talent density by 2027"
  - "SMBs at $2-10M will adopt fastest"
---
```

## Status Definitions

| Status | Meaning |
|--------|---------|
| `active` | Thesis is stable and being tracked |
| `evolving` | Significant new evidence is shifting the thesis |
| `challenged` | Strong counter-evidence has emerged |
| `archived` | Thesis has been retired (proven, disproven, or obsolete) |

## Version Guidelines

- **Minor version bump (2.3 → 2.4)**: New signals incorporated, minor refinements
- **Major version bump (2.4 → 3.0)**: Core argument restructured, key claims changed

## Example

```yaml
---
slug: reshoring
title: "Reshoring & Deglobalization"
status: active
version: "1.8"
created: 2024-06-15
updated: 2024-12-21
connections:
  - us-china
  - inflation
  - ai-knowledge-work
description: |
  Manufacturing returning home, supply chain rewiring, and what
  happens when 'made in America' becomes strategic necessity
  rather than marketing.
key_claims:
  - "30% of China-dependent supply chains will have US alternatives by 2028"
  - "Reshoring creates professional services demand for domestic expertise"
---

# Reshoring & Deglobalization

## The Core Argument

[Thesis content here...]
```
