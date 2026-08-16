# Frosted Object Poster Style Guide

## Priority Hierarchy

For detailed source-reference analysis, read `reference-analysis.md` before style-sensitive generation.

Match the reference mood before optimizing anything else:

1. **From-scratch redraw:** use the photo only to understand the object, then create a new poster illustration. Never apply a frosted-glass filter over the photo.
2. **Translucent frosted atmosphere:** milky transparent planes, blurred interior color, softened far-side contours, color bleeding through redesigned forms.
3. **Object recognition:** keep the main silhouette and a few iconic cues from the uploaded photo.
4. **Large-form simplification:** reduce tiny detail into broad soft masses.
5. **Locked poster layout:** fixed 3:4 canvas, pure white background, centered subject, top bilingual name, bottom creator/mood caption.
6. **Optional slight vector feel:** only clean up silhouettes and shape boundaries. Do not turn the subject into a flat icon.

If a style rule conflicts with the translucent frosted atmosphere, the atmosphere wins. If a style rule conflicts with the locked poster layout, the locked poster layout wins.

## Locked Production Rules

These rules are fixed and must not be changed while calibrating style:

- Output ratio: 3:4 vertical poster.
- Resolution target: 4K-quality, preferably 3072x4096 or equivalent.
- Background: pure white (#FFFFFF), with no paper texture, off-white tint, gradient, vignette, floor plane, tabletop, or scene.
- Subject: centered and appropriately sized.
- Top text: Chinese and English object name.
- Bottom text: creator name or short mood caption.
- Style calibration only affects the object rendering, not these layout/background/text rules.

## Calibration Boundary

When the user asks to calibrate the visual style, change only the object rendering language:

- Adjust material, translucency, matte grain, soft blur, opacity, color-block simplification, and overlap.
- Adjust the redraw process: force semantic extraction, shape redesign, and repainting from broad forms.
- Do not adjust output ratio, resolution target, pure white background, subject centering, top object name rule, or bottom caption rule.
- Do not copy the reference's subtle off-white texture into the poster background. The reference mood comes from pale object edges and frosted material; the production background remains #FFFFFF.

## What The References Actually Are

The references are not literal photos, not product renders, not photo filters, and not flat vector icons. They are redrawn soft editorial still-lifes with:

- a clear translucent container or outer form, such as a tote wall, cup wall, rim, handle, or shell;
- colorful inner objects or color fields blurred behind that frosted outer form;
- milky white opacity, soft internal blur, and matte grain;
- rounded softened edges, diffused highlights, and hazy overlap;
- large simplified forms rather than detailed realism;
- clean white or near-white surrounding field with generous negative space. For production output, still use pure white (#FFFFFF) because that rule is locked.
- invented clean shapes and poster composition, not preserved source-photo texture or perspective clutter.

The style can be slightly graphic, but it should still feel like an airy translucent object, not a logo mark or sticker.

## Core Visual Formula

Use this formula:

```text
semantic extraction from photo + pure white poster + newly redrawn translucent object forms + large blurred color masses + hazy matte grain on the object + sparse typography
```

Do not use this formula:

```text
original photo + blur/filter + frosted glass sheet on top + preserved photo details
pure vector icon + hard geometry + flat opaque blocks + zero atmospheric depth
```

## Avoid Overcorrection

These are failure modes from testing:

- **Too filter-like:** looks like the original photo viewed through frosted glass, with preserved source perspective, texture, and small details.
- **Too 3D:** looks like a product render, realistic food/photo, ceramic, plastic, or modeled object.
- **Too flat/iconic:** looks like a vector icon made of simple polygons and loses frosted depth.
- **Too detailed:** keeps crumbs, leaf veins, printed words, dirt, individual pebbles, wrinkles, scratches, or food texture.
- **Too background-heavy:** uses desk, lifestyle setting, gray gradient, floor plane, vignette, or visible shadow.
- **Too glossy:** transparent but polished; missing matte frosted haze.

Correct path: redraw the subject as a new object poster, then use soft translucent overlap and blurred inner color while simplifying details.

## Redraw Procedure

Before generating, turn the source photo into a design brief:

1. Name the object and choose the exact poster title.
2. Describe the simplified silhouette in one sentence.
3. Select 3-5 identity cues to preserve.
4. Select 3-6 large color masses; ignore small photographic detail.
5. Decide which real object parts become translucent planes. Use natural carriers first: bag, cup, box, wrapper, shell, vessel, petals, fruit skin, leaf layers, fabric, or casing.
6. If the object has no natural carrier, do not add a generic glass sheet. Redraw its own surface as milky matte color planes with soft overlaps.
7. Prompt the image as a new illustration/design, not an edit of the photo.

Use language like:

```text
redraw from scratch as a new minimalist poster illustration based on the uploaded object, not a photo filter, not an image with a frosted glass layer on top, redesigned simplified silhouette, invented soft translucent planes, broad color fields
```

## Flatness Target

The desired flatness is not "zero volume." It is:

- no realistic cast shadow;
- no hard 3D modeling;
- no literal photo texture;
- no small details;
- broad poster-like silhouettes;
- color blocks that are soft, blurred, and semi-transparent;
- just enough soft highlight and overlap to prove that one layer is in front of another.

The image should look like a soft frosted object poster made from large translucent color planes, not like a fully flat SVG icon.

## Canvas And Layout

- Use 3:4 vertical output. Prefer 3072x4096, 2160x2880, or the highest available 3:4 resolution.
- Background must be pure white (#FFFFFF). Do not import the reference image's subtle paper texture into the final poster background.
- Center the subject horizontally.
- Subject size:
  - Tall object: about 58-70% canvas height.
  - Wide object: about 50-64% canvas height and 62-78% canvas width.
  - Small/simple object: scale up enough to read, but leave generous white margins.
- Keep top and bottom text areas clear. Do not let text overlap the object.
- Use only a faint grounding haze if needed. Avoid obvious cast shadows and floor planes.

## Material Recipe

Use this recipe as the core prompt block:

```text
Redraw the object from scratch as a soft translucent frosted still-life on a pure white (#FFFFFF) poster background. Use a redesigned simplified silhouette, milky semi-transparent material planes, blurred internal color fields designed into the object, softened far-side contours, diffused color bleeding, hazy edges, broad matte highlights, and subtle frosted grain on the object only. Simplify details into large soft shapes, but keep the object's recognizable silhouette and key cues. Avoid photo filtering, frosted-glass overlay, hard 3D rendering, flat icon abstraction, realistic texture, hard shadows, sharp reflections, tiny details, and background texture.
```

Material cues:

- 35-65% opacity milky outer shell.
- Blurred warm/cool color masses behind the shell.
- Far-side contours softened and lower contrast.
- Frosted matte surface with fine soft grain.
- Broad diffused highlights, never sharp glossy hotspots.
- Rounded/hazy edges with gentle overlap.
- Slight volume only where it supports transparency.

Suggested opacity hierarchy:

- outer handles, far rims, and back walls: very pale, about 10-25% visual strength;
- main frosted wall/shell/lip/flap: milky, about 25-55% visual strength;
- inner color masses: strongest, but blurred through the shell, about 55-90% visual strength;
- tiny identity accents: only 1-2, slightly clearer than the rest.

## Shape Abstraction

Use large, soft, recognizable forms:

- Identify the object's top 3-5 visual cues.
- Redesign the big silhouette and one or two distinctive structural shapes as clean poster forms.
- Merge repeated small parts into larger color masses.
- Remove literal text, brand marks, small stains, crumbs, grit, veins, scratches, and tiny wrinkles.
- Let color blocks bleed and blur through translucent surfaces.
- Do not preserve original camera angle, exact folds, individual pieces, or source-photo lighting when they make the result feel filtered.

Do not over-flatten into pure geometry. If the result looks like a simple SVG icon, increase soft blur, color bleeding, frosted haze, and translucent overlap.

## Reference Matching Checklist

Before accepting an output, check:

- Does it have one dominant translucent shell/wall/skin that covers or wraps the colorful subject?
- Does it feel redrawn from scratch rather than like the source photo with blur or glass over it?
- Are the strongest colors behind or inside that shell, not sitting as separate opaque graphic blocks?
- Are internal colors blurred and blooming through the frosted layer?
- Are edges soft and hazy while the main silhouette remains readable?
- Is there a large clean white field around the subject?
- Is there only a faint sense of depth, enough to show overlap, but not product-render volume?
- Is the object simplified without becoming a sticker/icon?
- Are tiny real-life details removed?

## Color Handling

- Extract the object's dominant colors.
- Lift brightness and freshness.
- Use the object's characteristic colors as internal color fields.
- Keep the outer shell pale, milky, and semi-transparent.
- Let strong colors sit behind or inside translucent material, then blur outward.
- Preserve one small high-identity accent when present, such as a red tomato, black straw, fruit skin, handle, logo shape if allowed, or flower decoration.

## Typography

Top label:

- `[中文名] / [English Name]`
- Small clean sans serif, charcoal or soft gray.

Bottom label:

- Short creator name or mood copy.
- 2-6 Chinese characters plus 1-3 English words works well.
- Keep it delicate and separated from the subject.

If exact text generation is unreliable, generate the image with reserved white space and add type in a separate layout step.

## Negative Prompt

Use or adapt:

```text
watermark, QR code, fake app watermark, random logo, busy background, desk, cables, laptop, lifestyle scene, dark background, gray gradient, off-white background, paper texture background, obvious floor plane, cast shadow, strong contact shadow, original photo under frosted glass, photo filter, blurred source photo, trace-over-photo, photorealistic photo, product render, hard 3D model, opaque ceramic, opaque plastic, solid cardboard, sharp reflections, glossy glass, hard black outline, flat vector icon, sticker icon, logo mark, excessive geometric simplification, crumbs, grease stains, readable package text, printed words, tiny details, realistic texture, sharp leaf veins, realistic pebbles, dirt, scratches, noisy background
```

## Prompt Examples

### Mango Tote

```text
Redraw the uploaded mango tote photo from scratch as a 3:4 high-resolution minimalist frosted object poster on a pure white (#FFFFFF) background. Center the subject. Preserve the tote silhouette, soft handles, and mango shapes, but invent clean simplified poster forms instead of filtering the photo. Make the tote wall the main translucent milky frosted shell, with mango orange, coral, and golden color fields blurred behind and through it. Use hazy edges, diffused color bleeding, broad matte highlights, and subtle frosted grain on the object only. Simplify folds and fabric detail into large soft forms. Keep slight dimensional overlap only to show transparency. Top text: "芒果手提袋 / Mango Tote"; bottom text: "透明小事 / Soft Carry". No watermark, no desk, no hard shadow, no product render, no flat icon, no frosted-glass overlay on the original photo.
```

### Apricot Sparkling Water

```text
Redraw the uploaded drink photo from scratch as a 3:4 high-resolution minimalist frosted object poster on a pure white (#FFFFFF) background. Center a tall cup. Preserve the cup silhouette, rim, straw, and fruit identity, but redesign all shapes as clean poster forms. Make the cup wall a milky translucent frosted shell, with blurred apricot orange, lemon yellow, grapefruit red, and cream color fields visible inside. Soften far-side contours and internal details; use broad matte highlights, hazy rim glow, and subtle frosted grain on the object only. Keep the black straw as one crisp identity accent. Top text: "杏子气泡水 / Apricot Sparkling Water"; bottom text: "Fresh Pause". No watermark, no product render, no flat icon, no hard shadow, no photo filter.
```

### Fried Snack Box

```text
Redraw the uploaded fried snack box photo from scratch as a 3:4 high-resolution minimalist frosted object poster on a pure white (#FFFFFF) background. Center the open kraft snack box. Preserve the open box silhouette, raised back flap, side flaps, liner-paper feeling, warm fried-food center, and one red tomato accent, but do not preserve exact food pieces or source-photo perspective. Make the box and liner behave like translucent frosted parchment: milky tan outer flaps with honey yellow, apricot orange, caramel brown, and tomato red color fields softly blurred behind them. Simplify crumbs, grease, printed words, folds, and food texture into broad soft masses. Keep soft translucent overlap and hazy edges; allow slight dimensional overlap only to show the box opening and transparency. Top text: "炸物小食盒 / Fried Snack Box"; bottom text: "酥脆时刻 / Crispy Mood". No desk, no laptop, no realistic food photo, no hard shadow, no product render, no flat vector icon, no frosted-glass overlay.
```
