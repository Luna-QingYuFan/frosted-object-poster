---
name: frosted-object-poster
description: Generate or edit 3:4 high-resolution posters from real object photos in a fresh translucent frosted-glass editorial still-life style, including 清新透明磨砂质感, 半透明磨砂物体海报, 柔雾透明色块, 大面积概括化物体图, and 小红书风格物体图. Use when the user wants an uploaded everyday object redrawn from scratch as a centered soft 4K poster, not filtered or blurred, with fixed 3:4 poster size, pure white background, translucent milky frosted outer forms, softly blurred internal color fields, simplified large shapes, bilingual object name at the top, and a short creator name or mood caption at the bottom.
---

# Frosted Object Poster

## Core Workflow

1. Inspect the uploaded object photo and identify the object's Chinese and English name, defining silhouette, original material cues, characteristic colors, and any details that must remain recognizable.
2. Read `references/style-guide.md` before generating or editing the final image. When calibrating style, debugging mismatch, or working from a new object photo, also read `references/reference-analysis.md`.
3. Convert the photo into a semantic design brief before prompting: list the object's silhouette, 3-5 identity cues, 3-6 broad color masses, and which parts become translucent planes. The photo is only source material; never use it as a base layer.
4. Generate a single 3:4 portrait image, preferably 3072x4096 or equivalent 4K-quality output, on a pure white (#FFFFFF) background. Do not change the poster size rule.
5. Keep the object centered, usually occupying about 52-68% of canvas height and 58-74% of canvas width, with generous pure white negative space. Never alter the 3:4 ratio, pure white background, top name text, or bottom caption rules while trying to improve style match.
6. Redraw the real object from scratch as a soft translucent frosted still-life. Preserve identity through a newly designed simplified silhouette, major translucent planes, dominant color fields, and 2-5 key visual cues. Do not filter, blur, trace, or re-render the original photo.
7. Simplify aggressively, but do not reduce the image to a flat icon. The target is a reference-like redrawn soft frosted still-life: broad semi-transparent planes, milky material, blurred color masses designed into the object, gentle overlap, and almost no conventional shadow. Keep only the slight softness/gradient needed to show translucent layering.
8. Add top typography with the object's Chinese and English name. Add bottom typography with either the creator's name or a short mood caption that fits the object. Do not change these text placement rules while calibrating the visual style.
9. Verify the output: correct 3:4 ratio, pure white background, readable top and bottom text, centered subject, no watermark, no unrelated props, no photorealism, no crowded layout, no hard shadow, and a strong reference-like translucent frosted feeling. If the output looks like a frosted-glass overlay on the source photo, a blurred copy of the source photo, or a flat vector icon, it failed.

## Style Contract

Use this visual language:

- Fresh, clean, quiet, airy, and editorial.
- Pure white background only: #FFFFFF. No lifestyle scene, tabletop clutter, dark backdrop, off-white paper background, gradient, texture, or floor plane.
- Redrawn from scratch: reinterpret the object as a new poster illustration using the uploaded photo only for recognition, not as a layer to be covered by blur or glass.
- The "watermelon" priority is translucent frosted atmosphere: milky transparent outer shell, blurred internal colors, softened far-side contours, and color bleeding through the surface.
- Large-form simplification: use broad soft masses and only a few key details, but keep the object feeling like a frosted still-life rather than a flat vector icon. The flatness should come from designing new simplified shapes, not from blurring the source photo or making opaque vector shapes.
- Subtle dimensionality is allowed only to support transparency: soft rim glow, diffused highlight, faint contact haze, and blurred overlap. Avoid hard product-render volume, cast shadows, bevels, realistic thickness, and shiny glass reflections.
- Heavy frosted softness: cloudy white veiling, soft grain, hazy edges, and diffused color fields.
- Colors derived from the object itself, shifted toward fresh fruit, candy glass, water gel, or pastel acrylic tones.
- Optional slight vector feeling only in the cleanliness of silhouettes and layout, never as the main style.
- Typography that feels like a minimal design poster: small upper label, larger or delicate lower caption depending on composition.
- Do not add a generic all-over translucent membrane unless the source object naturally has a carrier such as a cup, bag, box, wrapper, shell, vessel, or petals. For other objects, redraw the object's own surfaces as milky soft color planes.

Keep these rules separate:

- **Locked poster rules:** 3:4 poster, pure white (#FFFFFF) background, centered subject, top Chinese/English object name, bottom creator or mood caption.
- **Style calibration rules:** how the object is redrawn into translucent, frosted, simplified, soft, color-blocked forms.
- If style calibration seems to conflict with locked poster rules, keep the locked poster rules unchanged and adjust only the object rendering.

Avoid:

- Literal product photography, blurred-photo filters, frosted-glass overlays, trace-over-photo results, busy lifestyle scenes, dark backgrounds, neon cyberpunk lighting, strong metallic texture, thick outlines, cluttered props, heavy grain, illegible text, fake app watermarks, and random brand marks.

## Output Prompt Pattern

When using an image generation model, build the prompt from these parts:

```text
Transform the uploaded photo of [object] into a 3:4 portrait high-resolution 4K minimalist still-life poster.
Do not edit, filter, blur, trace, or cover the original photo. Redraw a new poster illustration from scratch based on the object's identity.
The object is centered and sized appropriately, occupying [size guidance].
Use a pure white (#FFFFFF) background with no clutter, no dark scene, no texture, no gradient, and no floor plane.
Render the object as a newly designed translucent milky frosted still-life with simplified soft planes and blurred internal color fields.
Preserve identity through a simplified redesigned silhouette, the key translucent material forms, and 2-5 key visual cues: [details].
Use large simplified color masses from the object: [palette].
Keep the image nearly shadowless and highly simplified, with only soft gradients, veils, and overlaps needed to show frosted transparency. Do not make it a flat opaque vector icon.
Top text: "[Chinese name] / [English name]" in clean minimal typography.
Bottom text: "[creator or mood caption]" in short delicate typography.
No watermark, no extra logos, no clutter, no photorealistic snapshot, no source-photo blur, no frosted-glass overlay on the source photo, no dark background, no off-white background, no paper texture background, no heavy 3D render, no flat icon, no strong shadow.
```

For detailed composition, typography, palette, and negative prompt guidance, use `references/style-guide.md`.
