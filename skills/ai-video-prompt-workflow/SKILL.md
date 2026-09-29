---
name: ai-video-prompt-workflow
description: Reverse-engineer a visual concept and design consistent generative-video prompts with character, product, scene, camera, action, continuity, negative constraints, and post-production plans. Use for shot-based AI video, image-to-video, product transformations, or narrative continuity repair. Do not imitate protected footage or present generated scenes as documentary evidence.
---

# AI Video Prompt Workflow

Generate short shots separately, then edit them into a verified story. Consistency and causal continuity outrank prompt length.

## Build the continuity bible

Define before prompting:

- Character: age range, appearance, clothing, accessories, handedness, and stable reference images.
- Product: exact structure, dimensions/proportions, material, color, handles, pockets, logo rules, and reference angles.
- World: location, time, lighting, palette, weather, and realism level.
- Camera: aspect ratio, lens language, framing, movement, and frame rate feel.

## Story and prompt workflow

1. Break the idea into causal beats. Every shot must begin from the previous shot's resulting state.
2. Write each prompt as subject + stable attributes + action + environment + camera + light/style + duration + continuity anchor.
3. Add negative constraints for duplicate limbs/products, changing colors/logos, unreadable text, warped structure, teleporting objects, and unintended watermarks.
4. Generate 3–6 second shots independently with at least two variants for important beats.
5. Select by structural accuracy and transition compatibility, not only beauty.
6. Add dialogue, precise typography, brand marks, and complex captions in post unless the model reliably supports them.
7. Assemble, check causal order, and regenerate only the minimum broken shot when possible.

## Causal integrity example

For a growth transformation, the initial object must fully disappear before a sprout appears; the plant grows before buds; buds precede product-like fruit; harvesting happens only after fruit exists. If the original object remains at the roots, the transformation logic is broken even if the frame looks attractive.

## Output

Return concept boundary, continuity bible, numbered shot list, per-shot prompt and negative prompt, input reference plan, duration, transition state, generation variants, rejection reasons, post-production notes, disclosure requirement, and final QA checklist.
