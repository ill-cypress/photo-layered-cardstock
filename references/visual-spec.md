# Visual and Prompt Specification

Use this reference to turn the source analysis into a precise image-generation instruction and to diagnose weak results. The intended object is an **unframed stack of separate cardstock sheets**, not a conventional shadow box.

## 1. Build a depth map

Read the photograph as physical space before simplifying its appearance.

- Use occlusion first: an element covering another belongs in front of it.
- Use relative scale, atmospheric softness, horizon position, and overlap as supporting cues.
- Record the main subject and the silhouettes, negative spaces, landmarks, and spatial relationships required for recognition.
- Divide the scene only at meaningful depth changes. The usual categories are foreground, main subject, midground, background, and sky/farthest backdrop, but the source—not a fixed layer count—determines the final stack.
- A layer can contain several disconnected paper shapes if they share one depth. It cannot contain objects from different depths.
- When a continuous object spans depth, separate its visible depth components into different sheets while keeping the assembled silhouette coherent from the main viewing angle.

Write the plan as a front-to-back stack before generation. Mention the defining content of every sheet and avoid vague combined labels such as “foreground and background scenery.”

## 2. Convert planes into paper sheets

For each depth plane:

- Preserve its decisive outer contours, object placement, relative scale, and overlaps.
- Reduce texture and tonal modeling to broad, clean, source-derived color shapes.
- Retain only internal details that make the subject or place recognizable.
- Use a single physical z-position for the sheet. Any internal color pieces must remain visibly coplanar unless they represent another explicitly separated depth layer.
- Give the cardstock consistent, believable thickness and matte cut edges.

The assembled view must reconstruct the whole photograph. Simplification changes rendering detail, not the scene inventory or spatial logic.

## 3. Stage the construction

- Stack the sheets in correct front-to-back order with clearly visible, moderate air gaps.
- Use a slight three-quarter or oblique camera angle—typically enough to expose one side of the stack without changing the source composition substantially.
- Let some lateral sheet edges and cutout openings reveal the staggered planes behind them.
- Keep the construction cohesive. It should not become an exploded diagram with layers floating so far apart that the photograph stops reading as one scene.
- Crop around the paper sculpture itself. A plain studio environment may provide contrast, but it must not become a backing board, stand, frame, box, or decorative surround.

## 4. Material and lighting

- Use thick colored cardstock with matte faces, visible edge thickness, restrained fibers, and clean handcrafted cuts.
- Use soft directional studio lighting coherent across the entire stack.
- Add narrow contact shadows at close separations and soft cast shadows falling from front sheets onto the next sheets behind.
- Make shadows physically correspond to the real gaps. Avoid printed or painted drop shadows on a sheet, generic ambient occlusion, smooth gradient modeling, or translucent layer effects.
- Keep color elegant and source-derived. Depth legibility should come from physical separation and shadow, not decorative contrast alone.

## 5. Prompt assembly

Build the generation prompt in this order:

1. State that the supplied photo is the exact composition and subject reference.
2. Name the main subject and the front-to-back sheet stack.
3. State that every named depth plane is one separate physical cardstock sheet and that no sheet may mix depths.
4. Describe the clean simplification, source-derived palette, and details that must remain recognizable.
5. Specify the slight oblique view, visible thickness, exposed edges, air gaps, and physically coherent shadows.
6. End with the no-housing and anti-flatness constraints.

### Prompt skeleton

> Transform the supplied photograph into a clean, elegant layered-cardstock diorama while preserving its complete composition, main subject, major silhouettes, placement, scale relationships, overlaps, horizon, and recognizable scene structure. Build it from separate thick matte cardstock sheets in this exact front-to-back order: [LAYER STACK]. Each sheet represents one spatial depth plane only; never place foreground, subject, midground, background, or sky content from different depths on the same sheet. Simplify every plane into broad, clean paper-cut shapes and a restrained source-derived palette, preserving identity-defining structure while removing micro-detail. Physically stack the sheets with visible moderate air gaps. Render the assembled scene from a slight oblique side angle so the thickness of every sheet, exposed paper edges, staggered silhouettes, spacing, contact shadows, and soft cast shadows are clearly visible. The result must read as a freestanding physical paper sculpture made from multiple separate sheets, not a flat illustration. Show only the layered paper construction. No box, shadow-box housing, outer frame, border, mat, bezel, rim, window, wall, container, backing board, stand, or decorative surround. No flat front view, single-layer relief, mixed-depth sheet, intricate filigree, invented objects, text, or watermark.

Add source-specific descriptions after the layer stack, especially for the main subject, landmark contours, and important occlusions. Do not add style rules unsupported by the user's request.

## 6. Failure diagnosis

### Looks like a flat poster

Increase the camera offset slightly and explicitly expose the lateral edges of every sheet. Widen the air gaps, strengthen physically consistent inter-layer shadows, and repeat that the planes are separate slabs rather than printed bands on one surface.

### Looks like a framed shadow box

Remove all words that imply enclosure, display case, cabinet, frame, or backing board. Repeat that only the freestanding stack of shaped cardstock sheets may appear and crop tightly around it.

### Layers are decorative rather than spatial

Rebuild the depth map from occlusion. Give every sheet one z-position and move any element that belongs to another depth onto its own sheet. Remove ornamental edge layers that do not correspond to source space.

### Scene is no longer recognizable

Restore the source framing, subject count, major silhouettes, landmarks, relative scale, and overlaps. Simplify internal texture rather than deleting or relocating structural content.

### View is too oblique

Reduce the angle until the photograph's composition reads clearly while at least one side edge, the sheet thicknesses, and the gaps remain visible.
