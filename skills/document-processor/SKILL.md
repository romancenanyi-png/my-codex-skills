---
name: document-processor
description: Process PDFs, DOCX files, slides, scans, screenshots, tables, and mixed-format documents into structured Markdown, summaries, extracted fields, and reusable knowledge.
metadata:
  source_status: "custom-gap-fill"
  aliases: "pdf-processor, document-parser, document-ocr"
---

# Document Processor

Use this skill to turn documents into usable structured information for agents, websites, research, sales enablement, SEO, and data extraction.

## When to use

Use for:

- PDF, DOCX, PPTX, spreadsheet, scanned, or image-heavy documents.
- Contracts, white papers, pitch decks, brochures, manuals, reports, and research papers.
- Extracting tables, headings, summaries, quotes, entities, dates, and action items.
- Converting documents into clean Markdown for knowledge bases or website content.
- Comparing multiple documents or versions.

## Workflow

1. **Identify document type**
   - Text-native PDF, scanned PDF, DOCX, slide deck, spreadsheet, image set, or mixed.

2. **Extract structure**
   - Title, headings, page numbers, sections, tables, figures, captions, footnotes, references.

3. **Extract content**
   - Preserve original order.
   - Keep tables as Markdown tables or CSV blocks.
   - Label uncertain OCR text.

4. **Normalize**
   - Remove repeated headers/footers.
   - Fix broken line wraps.
   - Preserve citations and page references.

5. **Summarize and index**
   - Executive summary.
   - Key facts.
   - Entities and definitions.
   - Open questions.

## Output format

```markdown
# Document Processing Report

## File Overview
- File name:
- Type:
- Page count:
- OCR needed: yes/no

## Executive Summary

## Structured Outline

## Extracted Tables

## Key Facts
| Fact | Page/Section | Confidence |
|---|---|---|

## Action Items

## Clean Markdown Export
```

## Quality rules

- Preserve page references for claims.
- Do not invent missing text.
- Mark unreadable sections clearly.
- For legal, financial, medical, or compliance documents, summarize cautiously and recommend expert review for decisions.
