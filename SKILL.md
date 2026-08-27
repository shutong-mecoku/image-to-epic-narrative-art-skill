---
name: image-to-epic-narrative-art
description: Transform a user-supplied photograph or film frame into an original spatial-allegory illustration using impossible perspective, extreme scale, active negative space, graphic simplification, restrained color, and mineral-print texture; optionally invent a short story that shapes and accompanies the image. Use when the user asks to convert an uploaded image into this established visual language. Do not use for ordinary retouching, simple color grading, or exact reconstruction of another artist's work.
---

# Image to Epic Narrative Art

Turn the source image into a newly composed visual allegory. Do not merely apply a filter, repaint the existing camera view, or force every subject into the same surreal device.

## Required input and default behavior

- Require one source image. Treat additional images as references only when the user labels them or their role is unambiguous.
- Default to **pure visual transformation**. Enable **narrative enhancement** only when the user explicitly asks to invent, write, or attach a story/backstory, or explicitly says `叙事增强`. Requests for mood, symbolism, or a more narrative-looking image change the visual direction but do not by themselves authorize story text.
- Choose the canvas from the preservation anchor and proposition. Preserve the source orientation and approximate ratio when a confrontation, procession, architecture, horizon, or group relationship depends on width or height. Use vertical 3:4 only when the user requests it or when vertical scale is itself part of the concept.
- Do not block on minor aesthetic choices. Infer them from the source, the selected visual metaphor, and the restrained series language.

## Read the relevant guidance

1. Always read [references/visual-language.md](references/visual-language.md).
2. Classify the source and read [references/scene-routing.md](references/scene-routing.md) before selecting references.
3. Read [references/narrative-mode.md](references/narrative-mode.md) only when narrative enhancement is active.
4. Read [references/generation-spec.md](references/generation-spec.md) before calling an image generator.
5. Read [references/quality-gates.md](references/quality-gates.md) before delivering the result.

## Workflow

### 1. Find the preservation anchor

Identify what must survive the transformation:

- single person: identity when relevant, pose, gesture, gaze, and bodily rhythm;
- group: primary relationship, action, hierarchy, and count when it matters;
- landscape or architecture: landmark relationships, path, horizon, and recognizable structural rhythm;
- object: silhouette, function, interaction, and one defining material cue.

Preserve the anchor, not the original camera layout. Remove incidental UI, subtitles, ratings, and overlays from the newly composed artwork unless the user asks to retain exact text. Do not present the operation as erasing ownership marks from an otherwise unchanged image.

### 2. State one visual proposition

Reduce the concept to one sentence, such as “the garment becomes the space it occupies” or “the two banks line a water-shaped rupture.” The proposition must arise from the source subject, action, and a form that is visibly present or directly evidenced by the source. Do not invent long shadows, roads, portals, discs, cracks, or folds merely because they are convenient metaphors.

Choose one dominant mechanism and, at most, one supporting mechanism:

- incompatible viewpoints;
- extreme near/far or large/small scale;
- subject becoming landscape or architecture;
- active negative-space cut;
- repeated modules changing state;
- meaningful crop or directional compression.

Do not stack mechanisms merely to look experimental.

### 3. Select references by function

- First lock the proposition, then decide whether a bundled reference actually helps it.
- Use the source image plus **zero or one primary style reference**. Add one secondary style/material reference only when a primary reference is already justified.
- Keep the total image inputs at three whenever possible. When no primary reference fits, use no bundled references; zero is preferable to a misleading one.
- Select references through `scene-routing.md`; never load every bundled image and never let a scene-category label dictate the composition.
- Borrow relationships—scale, space, hierarchy, reduction, material—not nouns, coordinates, colors, or recognizable layouts.

### 4. Generate a new composition

Use the available image-generation or image-editing capability. Label every input image's role explicitly. Preserve the source anchor, but allow substantial recomposition elsewhere.

The finished image should have:

- one dominant silhouette or spatial proposition readable at thumbnail size;
- an active field of light or dark negative space;
- a small scale cue when it strengthens the idea;
- two to four functional colors, not a default black-and-beige formula;
- clean major contours with locally varied mineral, dry-pigment, or silkscreen texture; leave some large surfaces nearly untextured;
- no visible text by default.

### 5. Inspect and revise

Inspect the actual output. If it fails a quality gate, revise only the highest-impact defect first. Typical priorities are: restore the concept, restore the source anchor, simplify the composition, repair anatomy, neutralize the palette, then reduce texture.

Do not deliver malformed people, accidental object fusion, fake text, a generic portal, a uniformly yellow image, or an attractive illustration that lacks a specific spatial idea.

## Output

- Return the finished image first.
- Briefly name the central spatial idea and what source relationship was preserved.
- In pure visual mode, do not add an unsolicited story.
- In narrative mode, place the short fictional story after the image; never render it inside the artwork unless the user explicitly requests visible typography.
