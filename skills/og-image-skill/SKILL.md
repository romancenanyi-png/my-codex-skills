---
name: og-image-skill
description: Generate Open Graph, social share, blog thumbnail, landing page, or marketing preview images from text briefs and brand constraints.
metadata:
  source_status: "normalized-from-public-description"
  source_url: "https://tools.yiteai.com/en/openclaw-skills/og-image-skill"
  aliases: "og-image-generator, social-preview-image"
  related_skills: "b2b-visual-assets-generator, visual-qa"
---

# OG Image Skill

Use this skill to create or brief Open Graph and social preview images that support articles, landing pages, campaigns, and B2B website assets.

## When to use

Use when the user needs:

- OG images for blog posts, pages, or docs.
- Social share cards for LinkedIn, X/Twitter, Facebook, Slack, or Discord previews.
- Campaign thumbnails, lead magnet covers, or content preview graphics.
- Consistent branded visuals for generated pages.

## Inputs

- Page title or article headline.
- Subtitle or supporting claim.
- Brand colors, fonts, logo rules, and visual style.
- Target aspect ratio, usually `1200x630` for OG.
- Audience and desired tone.

## Workflow

1. Extract the core message from the page or brief.
2. Write a short image prompt with clear hierarchy: headline, supporting visual, brand tone.
3. Keep the layout simple enough to read at small preview size.
4. Avoid excessive text.
5. Generate or brief variants.
6. Run visual QA before publishing.

## Output format

```markdown
# OG Image Brief

## Asset
- Page:
- Size:
- Format:

## Text
- Headline:
- Subtitle:

## Visual Direction
- Style:
- Composition:
- Colors:
- Imagery:

## Prompt
Full generation prompt.

## QA Checklist
- [ ] Readable at thumbnail size
- [ ] Safe margins
- [ ] Brand aligned
- [ ] No misleading claims
- [ ] Exports as PNG/WebP
```
