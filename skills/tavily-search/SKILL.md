---
name: tavily-search
description: Use Tavily-powered real-time web search for current, niche, competitive, technical, SEO, market, and research questions where normal model memory may be stale or incomplete.
metadata:
  source_status: "normalized-from-public-description"
  source_url: "https://clawbot.ai/skills/tavily-search.html"
  environment: "TAVILY_API_KEY"
  aliases: "web-research, realtime-search"
---

# Tavily Search

Use this skill when the agent needs current or niche web information. Tavily is especially useful for concise search results, competitor research, source discovery, and follow-up investigation.

## When to use

Use this skill when the user asks for:

- Latest or current information.
- Market, competitor, industry, pricing, legal, product, or policy research.
- SEO keyword, SERP, content, or backlink research.
- Verification of unfamiliar terms, tools, libraries, people, companies, or claims.
- Citations, source links, or evidence-backed answers.

## Inputs

- Query or research question.
- Region/language constraints.
- Recency requirements.
- Preferred source types: official docs, news, academic, product pages, forums, etc.

## Search workflow

1. Rewrite the user need into 2-4 precise search queries.
2. Run broad search first, then targeted searches against authoritative sources.
3. Prefer primary sources: official docs, original research, company pages, regulatory pages, or direct product pages.
4. For contested topics, collect multiple viewpoints.
5. Track publication dates and event dates separately.
6. Summarize with citations and confidence level.

## Output format

```markdown
# Search Findings

## Answer
Concise answer.

## Evidence
| Claim | Source | Date | Notes |
|---|---|---|---|

## Caveats
- What is uncertain or conflicting.

## Recommended next action
```

## Safety and quality notes

- Do not rely on low-quality scraped pages when primary sources are available.
- Treat product prices, schedules, laws, and public roles as volatile.
- For medical, legal, financial, or high-stakes topics, cite authoritative sources and avoid overclaiming.
