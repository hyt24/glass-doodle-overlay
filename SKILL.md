---
name: glass-doodle-overlay
description: "Turn each uploaded photo into its own fixed-ratio 3:4 vertical two-panel art poster: retain the real photograph in the upper half and place a cute thick white glass-window doodle reinterpretation of the same scene in the lower half. Use when the user asks for 上下拼图, 固定比例海报, 玻璃涂鸦海报, ‘像什么就画什么’, 玻璃涂鸦, 窗户涂鸦, or a photographic doodle edit that must keep the original photo intact."
---

# Glass Doodle Overlay Poster

Use the image generation/editing tool to turn every supplied photo into one finished poster. Process multiple uploads independently: output one poster per source photo and never combine different photos into a collage.

## Fixed poster system

- Use an exact 3:4 vertical canvas.
- Split the canvas into two equal-height panels: upper 50% and lower 50%. Keep the panel boundary clean and straight; do not introduce a third panel, frame, caption, or separator text.
- Use the same source photo in both panels. The upper panel is a restrained photographic treatment; the lower panel is the original Glass Doodle Overlay treatment.
- Extend only compatible sky, ground, wall, water, or environmental background when needed to fit the panel. Never stretch, warp, crop away, redraw, or alter the main subject.

## Workflow

1. Inspect one source photo. Identify its subject, silhouette, placement, scale, natural lighting, and the requested imagined form.
2. Read [references/style-guide.md](references/style-guide.md) and use [references/prompt-template.md](references/prompt-template.md).
3. Build the upper half from the real source photo. Preserve its subject structure, realistic texture, natural light, and original color mood. Apply only subtle premium editorial color grading: art magazine, independent publication, or exhibition photography—not a filter, illustration, or scene replacement.
4. Build the lower half from the same scene. Preserve the subject, perspective, composition, lighting, and background, then add extremely thick, playful white glass-marker doodles on a near-side transparent window pane so the subject reads as the imagined form.
5. Add 1–5 tiny, strongly related white pictograms near the lower-panel subject by default. Omit them only when the user explicitly asks for no icons.
6. Inspect the poster. Regenerate once if the proportions are not exactly 1:1, separate uploaded photos were combined, the upper panel is no longer photographic, the lower panel changes the subject, the glass looks fogged, or the doodle is thin, intricate, overfilled, or text-bearing.

## Lower-panel rules

- Retain the real-world subject rather than turning it into a complete animal, creature, or object.
- Establish three clear depth layers: foreground glass doodle → real subject outdoors → original background.
- Make the white drawing look physically on the glass closest to the camera. Allow only a slight natural reflection; keep the pane clear and distinct from the outdoor subject.
- Draw only decisive identifying features of the imagined form, such as ears, horns, eyes, wings, a fin, paws, antennae, or a tail. Follow the real silhouette rather than enclosing it with a generic icon.
- Use very thick, simple, deliberately hand-drawn white marker, crayon, or glass-pen lines. Avoid fine linework, fills, shading, or polished vector geometry.
- Keep all text, letters, numbers, signatures, watermarks, interface elements, and decorative frames out.

## Delivery

Show every finished poster separately. Briefly state the identified subject and imagined form for each output, plus the saved path when available.
