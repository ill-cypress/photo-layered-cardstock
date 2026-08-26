---
name: photo-depth-shadowbox
description: Selectively reinterpret a photograph as a front-facing, handcrafted 4–6-layer paper shadow box with cartoon-like hand-drawn abstraction, broad matte shapes, faceless people, visible paper edges, and cast shadows. Use for photo-to-image requests that need depth decomposition without literal scene tracing; do not use for generic paper filters, sticker-card layouts, or fabrication-ready cutting templates.
---

# Photo Depth Shadow Box

Transform the supplied photograph into one finished image whose structure visibly follows:

**DEPTH ANALYSIS → SUBJECT EDITING → LAYER SELECTION → SILHOUETTE → PAPER DIORAMA**

The defining idea is: **Decompose a photograph by visual depth and rebuild it as a handcrafted multi-layer paper shadow box.** Treat the photograph as source memory, not a layout to trace literally.

## Input and output

- Require a source photograph. If none is available, ask the user to attach one.
- Use an image-editing/generation tool with the photograph as the source reference; do not recreate the result with code or filters.
- Produce one polished shadow-box artwork unless the user requests variants or separate planes.
- Preserve recognizability through one compact **identification anchor**: the main person, landmark, vehicle, object, or distinctive spatial relationship.
- Preserve the source aspect ratio unless the user requests another format.

## Workflow

1. Inspect the photograph and identify its emotional center, identification anchor, dominant spatial gesture, foreground, subject plane, background, and any broad quiet field such as sky, water, ground, wall, or road.
2. **Edit the scene before layering.** Decide what the memory is about, then omit unrelated people, vehicles, signs, clutter, repeated architecture, foliage detail, and other descriptive noise. Do not trace every visible source element.
3. Select **4–6 physical paper planes**, ordered front to back. Start from `foreground → main subject → middle ground → distant ground → sky/backdrop`, then merge or split only when it improves recognition or overlap.
4. Recompose the selected content into 3–6 oversized, blunt visual masses with quiet negative space. Mild naive changes in scale, spacing, proportion, or placement are welcome when they strengthen the subject.
5. Translate each plane into cartoon-like, hand-drawn cut-paper forms: chunky silhouettes, simplified geometry, slightly awkward contours, flat matte colors, and minimal internal detail.
6. Rebuild the scene as a real paper shadow box viewed **straight on from the front**. Use paper-edge shadows, contact shadows, and narrow layer separation to reveal depth; do not rotate the box to expose its side.

Before generation, state one compact line containing both the layer stack and the main omissions, for example: `railing → one couple → fountain → simplified buildings → dusk sky; omit the remaining crowd and cars`. Provide only this user-verifiable plan, not hidden reasoning.

## Selective abstraction

- Make the first read the identification anchor, 3–6 large shapes, and one calm field—not photographic detail.
- Preserve the anchor through silhouette, signature color, relative placement, and relationship to one or two supporting forms. Exact geometry and complete object inventory are not required.
- Rebuild the scene from **5–8 broad, low-saturation matte color families** sampled from the source, with no more than one or two stronger accents.
- Compress vegetation into 1–3 lumpy tonal masses; reduce buildings, terrain, water, and roads to decisive planes; suppress masonry, leaves, windows, grooves, machinery, fabric folds, and repeated linework.
- Prefer deliberate omission over descriptive completeness. Expand a source-supported sky, water, ground, wall, snow, sand, or road area to create breathing room.
- Allow a gently naive, editorial, lightly nostalgic mood. The result should feel illustrated by hand before being cut from paper, not mechanically segmented from a photograph.

## People and crowds

- Remove incidental background people by default. Retain only the smallest number needed for the story, scale, or emotional center—usually zero, one figure, one pair, or at most two compact pairs/groups.
- In a crowded source, choose representative figures rather than reproducing the crowd. For a fountain scene, for example, keep the fountain and one or two central pairs; omit the surrounding spectators unless a specific group is the subject.
- Render all people as compact, simplified paper characters or silhouettes with broad pose and clothing-color cues only.
- **Never draw facial features.** No eyes, pupils, eyebrows, nose, nostrils, mouth, lips, teeth, facial shading, or realistic skin detail, even on the main subject or a large foreground figure. Use a blank face shape, profile block, hair mass, hat, or fully faceless silhouette.
- Avoid detailed anatomy, fingers, fabric folds, or individualized background portraits.

## Non-negotiable visual constraints

- Exactly 4–6 visually distinct depth planes.
- Strict front elevation: camera centered and parallel to the artwork; straight-on composition with no three-quarter turn, visible box side, receding frame edge, or perspective skew.
- Depth remains legible through narrow physical spacing, exposed cut edges around silhouettes, consistent contact shadows, and soft cast shadows falling onto the planes behind.
- Bold, slightly rough hand-cut or torn-cut contours with subtle hand-drawn waviness; never smooth vector-perfect paths.
- Matte fibrous cardstock with opaque gouache, cut-paper, risograph, or screen-print-like color character; subtle uniform paper tooth and slight pigment-density variation are welcome.
- Flat color relationships rather than photorealistic modeling. Keep near-black sparse and avoid smooth gradients.
- One coherent handcrafted object with a restrained frontal frame if useful; the frame must not dominate.

Avoid literal tracing, flat posterization, stacked translucent photo masks, photographic cutout collage, glossy plastic, clay, wood, origami folds, miniature figurines, detailed faces, polished vector art, anime, watercolor blooms, visible marker bands, intricate texture, decorative filler, labels, captions, or watermarks.

## Composition decisions

- Give the identification anchor its own layer whenever this materially improves recognition.
- Use only source-supported foreground forms such as foliage, railings, rocks, doorways, or street furniture, and simplify them aggressively.
- Merge adjacent depth regions when their silhouettes compete; split a region only when the extra plane creates a clear overlap or useful spatial cue.
- When no sky is visible, use the farthest wall, landscape, darkness, or backdrop instead of inventing sky.
- Preserve culturally or geographically important landmark contours, but reduce secondary structures to supporting masses.

Read [references/visual-spec.md](references/visual-spec.md) when composing the image-generation instruction, pruning a crowded scene, or resolving an ambiguous layer stack.

## Quality check

Inspect the result before delivery. Regenerate or refine it if any of these fail:

- The camera is not squarely front-facing or any side wall of the box is visible.
- The scene reads first as detailed source transcription rather than a few broad shapes and quiet space.
- Unrelated people, vehicles, buildings, or foliage remain prominent.
- Any person has visible facial features.
- A viewer cannot distinguish 4–6 depth planes through edges and shadows.
- The identification anchor is no longer recognizable.
- The result looks photographic, mechanically vectorized, or merely covered with paper texture.
- Important layers intersect in physically impossible order.

Present the final image and briefly name the identification anchor, retained figures, omissions, and front-to-back layer order.
