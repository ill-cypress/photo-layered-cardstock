---
name: photo-layered-cardstock
description: Transform a source photograph into a clean, unframed layered-cardstock diorama made from separate paper sheets at distinct depths, shown from a slight oblique angle with visible edges, spacing, and cast shadows. Use for photo-to-image requests that require a recognizable scene rebuilt as a physical stacked-paper sculpture; do not use for framed shadow boxes, flat papercut posters, generic paper-texture filters, or fabrication-ready cutting templates.
---

# Photo Layered Cardstock Diorama

Rebuild the supplied photograph as a **layered cardstock diorama composition**. The finished image must show only the freestanding paper construction—never a box, frame, housing, or container.

The governing rule is:

**ONE SPATIAL DEPTH PLANE = ONE SEPARATE PHYSICAL CARDSTOCK SHEET**

Multiple elements may share a sheet only when they occupy the same depth plane in the source. Never combine foreground, subject, midground, background, or sky content on one sheet merely to simplify generation.

## Input and output

- Require a source photograph. If it is missing or inaccessible, ask the user to attach it.
- Use an image editing or generation tool with the photograph supplied as the visual reference. Do not simulate the transformation with code, filters, or a text-only description.
- Preserve the source aspect ratio unless the user requests another format.
- Produce one polished image unless the user asks for variants or isolated layers.
- Treat the complete photograph as the composition reference. Preserve the main subject, recognizable scene structure, placement, scale relationships, overlaps, horizon, and major silhouettes.

## Process

1. **Identify the subject and depth planes.** Inspect occlusion, scale, overlap, atmospheric distance, and frame position. Find the foreground, main subject, midground, background, and sky or farthest backdrop that actually exist in the photo.
2. **Group strictly by spatial depth.** Place only elements occupying the same depth on the same plane. If one object visibly spans different depths, split its visible parts across the appropriate planes.
3. **Convert each depth plane into one separate cardstock sheet.** Simplify photographic detail into clean, broad paper-cut shapes while preserving each plane's decisive contours and content.
4. **Stack the sheets from front to back.** Keep their order physically correct and use visible air gaps; front sheets must occlude the sheets behind them as the source scene requires.
5. **Render from a slight oblique angle.** Keep the scene recognizable while clearly exposing sheet thickness, lateral paper edges, staggered silhouettes, and spacing between planes.
6. **Light the physical construction.** Use coherent contact shadows and soft cast shadows from each sheet onto the sheet behind it to make the depth unmistakable.

Before generation, state the inferred front-to-back stack in one compact line, for example: `near foliage → people → building → hills → sky`. Adapt the number of layers to the source; do not force empty or artificial planes.

## Visual direction

- Make the result read as several **thick colored cardstock sheets suspended and stacked in space**, not as one decorated surface.
- Use matte, opaque cardstock with visible paper thickness, crisp edge definition, restrained paper tooth, and clean handcrafted cut contours.
- Favor broad shapes and an elegant reduction of detail. Retain details that establish identity; remove fussy texture and micro-detail that do not affect recognition.
- Derive the palette from the source photograph, simplifying tonal variation into a small set of coherent paper colors.
- Keep the source composition dominant. The oblique view should reveal depth without turning the scene into a dramatically distorted perspective or an exploded technical diagram.
- Let gaps and shadows describe the construction. Do not fake depth with printed drop shadows, gradients, translucent photo slices, or several depth bands illustrated on one flat sheet.

## Hard constraints

- **No box, shadow-box housing, outer frame, border, mat, bezel, rim, window, enclosing wall, container, card outline, or decorative surround.**
- No flat poster-like papercut illustration.
- No single-layer composition or shallow embossed relief pretending to be multiple sheets.
- No straight-on front view that hides thickness and spacing.
- No sheet containing more than one spatial depth plane.
- No overly intricate cutwork, tiny decorative fragments, or surface detail that competes with depth layering.
- No invented objects, deleted primary subjects, arbitrary rearrangement, or major silhouette changes that reduce recognition.
- No glossy plastic, clay, wood, origami folds, miniature figurines, photographic cutout collage, text, captions, labels, or watermark.

The priority order is: **source recognizability → correct depth separation → visible physical construction → clean paper simplification → decorative finish**.

Read [references/visual-spec.md](references/visual-spec.md) when preparing the image-generation instruction or checking a result.

## Quality gate

Inspect the generated image before delivery. Refine or regenerate it if any answer is no:

1. Is the original subject and scene immediately recognizable?
2. Does every visible sheet represent one and only one spatial depth plane?
3. Can the viewer clearly see several separate sheets, their thickness, exposed edges, air gaps, and cast shadows?
4. Is the camera slightly oblique rather than flat front-facing or excessively angled?
5. Is the construction completely unframed and free of any box or housing?
6. Are the shapes clean and simplified without losing essential structure?
7. Is the layer order physically plausible, with no impossible intersections or reversed occlusions?

Present the finished image and briefly name the front-to-back layer order.