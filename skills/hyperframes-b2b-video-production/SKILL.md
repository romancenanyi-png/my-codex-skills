---
name: hyperframes-b2b-video-production
description: Implement approved B2B video scripts as deterministic HyperFrames compositions and verify layout, timing, animation, audio, render, and encoded output. Use after a brief, design, storyboard, and source manifest exist. When official HyperFrames skills are installed, read and follow them before implementation.
---

# HyperFrames B2B Video Production

Turn an approved storyboard into one reproducible composition; do not redesign the brief during rendering.

## Required artifacts

- `BRIEF.md`: goal, audience, duration, aspect ratio, approved flow, constraints, and review gate.
- `DESIGN.md`: palette, typography, spacing, caption style, and motion character.
- `STORYBOARD.md`: shot-by-shot timing, source asset/time range, text, transition, and audio.
- Asset manifest with local frozen paths and rights/claim notes.

## Production loop

1. Inspect the local HyperFrames CLI/version and official skill instructions; initialize the smallest valid composition.
2. Use framework timing attributes and seek-safe animation. Media playback must remain controlled by the rendering framework.
3. Preserve source aspect and focal points. Hide outgoing scenes after transitions; prevent decorative layers from polluting layout inspection.
4. Add captions with readable size, contrast, safe margins, and no overlap with key product/process areas.
5. Keep source audio unless the brief authorizes music, replacement, speed changes, or voiceover. Mix only after picture timing is stable.
6. Run lint and structural validation, inspect representative samples, open an interactive preview, and stop at the brief's review gate when required.
7. Render only the approved composition, then verify the actual output file.

## Delivery gates

- Exact expected duration, dimensions, frame rate, video/audio codecs, and nonzero file size.
- No black/blank frames, stale scene layers, clipping, overflow, broken assets, console errors, or caption collisions.
- Full decode succeeds; representative beginning/middle/end frames match the storyboard.
- Deliver project source, frozen assets or manifest, preview evidence, render log, and final media path.

Never copy third-party footage, watermarks, branding, or testimonials without permission.
