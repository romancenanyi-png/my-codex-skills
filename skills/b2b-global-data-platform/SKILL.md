---
name: b2b-global-data-platform
description: Design and manage a structured B2B data layer for global markets, including company profiles, industries, countries, contacts, segments, intent signals, source reliability, compliance fields, and content/lead-generation usage.
metadata:
  source_status: "custom-gap-fill"
  related_skills: "b2b-lead-generation, b2b-content-marketing, seo-expert"
---

# B2B Global Data Platform

Use this skill to create the data foundation behind B2B websites, market entry, lead generation, international SEO, segmentation, and sales operations.

## When to use

Use when the user needs to:

- Build a company/contact/account database.
- Segment prospects by country, industry, size, role, revenue, language, or intent.
- Create global B2B landing pages from structured data.
- Support multi-region SEO and GTM planning.
- Normalize data from CRM, spreadsheets, web research, enrichment tools, and forms.
- Track source quality, consent, and compliance constraints.

## Core schema

```text
Account
├── company_name
├── domain
├── country / region / city
├── industry / sub_industry
├── employee_range / revenue_range
├── product_fit
├── use_cases
├── intent_signals
├── source_url
├── source_confidence
├── consent_status
└── last_verified_at

Contact
├── name
├── role / seniority / department
├── email / linkedin / phone
├── account_id
├── region
├── language
├── consent_status
└── last_verified_at
```

## Workflow

1. Define data use cases and legal constraints.
2. Design account, contact, market, keyword, and content schemas.
3. Define canonical fields and allowed values.
4. Map sources and confidence scoring.
5. Deduplicate and normalize entities.
6. Segment by ICP, region, industry, intent, and lifecycle stage.
7. Define update cadence and stale-data rules.
8. Generate outputs for website pages, sales lists, content maps, and reports.

## Output format

```markdown
# B2B Global Data Platform Plan

## Use Cases

## Data Model
| Entity | Fields | Required? | Notes |
|---|---|---|---|

## Source Map
| Source | Fields | Refresh cadence | Risk |
|---|---|---|---|

## Segmentation Rules

## Compliance / Consent Fields

## Quality Checks

## Example Exports
```
