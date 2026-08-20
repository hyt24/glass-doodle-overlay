---
name: glass-doodle-overlay
description: "Turn an uploaded photo into a glass-window doodle overlay: preserve the real scene and subject, then align a few very thick white hand-drawn marks on the near glass so the subject reads as a requested imagined character or object. Use when the user asks for ‘像什么就画什么’, 玻璃涂鸦, 窗户涂鸦, 白色马克笔叠画, or a cute photographic doodle edit that must keep the original photo intact."
---

# Glass Doodle Overlay

Edit one supplied photo with the image generation/editing tool. Do not recreate, vectorize, filter, or replace the photo.

## Workflow

1. Inspect the supplied photo. Identify the requested subject, its silhouette, position, scale, and the direction in which it can plausibly suggest the requested imagined form.
2. Read [references/style-guide.md](references/style-guide.md). Keep the source scene, perspective, composition, lighting, and subject recognizably unchanged.
3. Add only a small number of extremely thick, playful white glass-marker strokes on the near-side window pane. Make them align with the real subject so the doodle reads as a spontaneous visual association, not a replacement or an illustration pasted over the image.
4. Generate at 4:5 by default. Preserve a different source aspect ratio only if the user explicitly requests it.
5. Inspect the result. Regenerate once when the scene, subject, light, or composition changed; the glass reads as fogged; or the doodle is thin, intricate, overfilled, or text-bearing.

## Prompt construction

Collect or infer these two variables:

- **Subject:** the real object, person, animal, or scene element to trace.
- **Imagined form:** what the subject should resemble.

Use the template in [references/prompt-template.md](references/prompt-template.md). State the variables explicitly, including the subject location when it removes ambiguity. If the subject cannot be reliably identified, ask the user to point it out rather than guessing.

## Non-negotiable visual rules

- Retain the original real-world subject rather than turning it into a full animal, creature, or object.
- Establish three clear depth layers: glass-surface doodle → real subject outdoors → original background.
- Make the white drawing look physically on the glass closest to the camera: slight natural reflection is acceptable, but keep it sharp and distinct from the outdoor subject.
- Draw only decisive identifying features of the imagined form: for example ears, horns, eyes, wings, a fin, paws, antennae, or a tail. Follow the real silhouette rather than enclosing it with a generic icon.
- Use very thick, simple, deliberately hand-drawn white marker, crayon, or glass-pen lines. Avoid fine linework, fills, shading, or polished vector geometry.
- Optionally add one or two tiny, related pictograms only if they clarify the association without crowding the image.
- Keep all text, letters, numbers, signatures, watermarks, interface elements, and decorative frames out.

## Delivery

Show the finished image. Briefly state the identified subject and imagined form, plus the saved path when available.
