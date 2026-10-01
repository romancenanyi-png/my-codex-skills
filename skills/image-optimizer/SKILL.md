---
name: image-optimizer
description: Analyze website images and recommend or implement compression, resizing, WebP/AVIF conversion, lazy loading, responsive image markup, alt text, and performance improvements.
metadata:
  source_status: "normalized-from-public-description"
  source_url: "https://openclawskills.best/skills/lxgicstudios/image-optimizer/"
  aliases: "image-performance, web-image-optimization"
  related_skills: "visual-qa, seo-expert"
---

# Image Optimizer

Use this skill to improve web performance and image quality for websites, landing pages, blogs, and B2B content libraries.

## When to use

Use when:

- Lighthouse flags oversized images, missing dimensions, poor LCP, or offscreen images.
- A website has heavy PNG/JPEG assets.
- The user needs WebP/AVIF conversion guidance.
- Responsive images, `srcset`, lazy loading, or CDN variants are needed.
- The user wants image SEO and alt-text improvements.

## Workflow

1. Inventory images by page or directory.
2. Record dimensions, file size, format, usage location, and whether the image is above the fold.
3. Identify oversized images and unnecessary PNGs.
4. Recommend target dimensions and formats.
5. Add responsive image markup where relevant.
6. Check accessibility: alt text, decorative images, and text-in-image issues.
7. Re-test performance.

## Output format

```markdown
# Image Optimization Report

## Summary
- Total images:
- Largest assets:
- Estimated savings:

## Priority Fixes
| Image | Current | Recommended | Expected impact |
|---|---|---|---|

## Implementation
- Format conversions:
- Resize targets:
- Lazy loading:
- Responsive markup:
- CDN/cache notes:

## Alt Text / SEO Notes
```

## Rules of thumb

- Hero/LCP images: preload carefully and avoid lazy loading above the fold.
- Below-the-fold images: lazy load.
- Use WebP or AVIF where supported.
- Set width and height to avoid layout shift.
- Use SVG for simple icons and logos where appropriate.
