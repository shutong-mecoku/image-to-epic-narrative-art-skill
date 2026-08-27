# Generation Specification

Use the available image-generation or editing capability. Build a concise production prompt with the following order.

## Prompt structure

```text
Use case: stylized-concept
Asset type: spatial-allegory illustration
Canvas: requested ratio, otherwise preserve the orientation needed by the source relationship; use vertical 3:4 only when vertical scale supports the proposition; no text

IMAGE ROLES
- Image 1: source/content anchor; list what must remain recognizable.
- Image 2: optional primary style reference; name only the transferable relationship and explicit no-copy items.
- Image 3: optional secondary reference, used only when Image 2 exists; limit it to one domain.

CENTRAL VISUAL PROPOSITION
One sentence specific to this source, carried by a visible or directly evidenced source form.

COMPOSITION
- dominant shape or subject
- viewpoint contradiction or scale relation
- active negative space
- small scale cue when justified
- deliberate crop and hierarchy

SOURCE INVARIANTS
- identity/pose/group relation/landmark/object interaction
- factual objects that must remain

STYLE, COLOR, MATERIAL
- large graphic masses and degree of simplification
- two to four functional colors
- clean ground; locally varied mineral or silkscreen texture

AVOID
- source-specific failure risks
- template motifs from the chosen references
- photo filter, generic concept art, uniform yellowing, malformed anatomy, text and watermark
```

## Role discipline

- Never call every input image an edit target.
- State exactly which image supplies content, composition logic, human treatment, palette, or material.
- List recognizable nouns and coordinates from style references under “do not copy.”
- Use the user's source as the only factual authority unless the user supplies a story or additional content reference.
- Do not add a long cast shadow, road, portal, crack, circle, fold, or giant crop unless the source visibly supports that carrier and it improves the preserved relationship.

## Recomposition strength

- For a single person, keep pose and bodily relationship prominent; transform the surrounding space or an organically connected element.
- For a group, simplify individuals while retaining the action hierarchy.
- For landscape and architecture, preserve relationships while allowing substantial camera and spatial reconstruction.
- For an object, maintain functional contact points so the result remains more than an arbitrary giant object.
- Do not force a factual object to become a bridge, doorway, altar, or other metaphor when that role conflicts with its source position or is unreadable without explanation.
- If foreground bodies or garments become spatial borders, preserve irregular human contours and visible joints/hands; do not extend them into two straight panels around a rectangular center.

## Visible text

Default to no visible text. Incidental subtitles, UI, ratings, and overlays from screenshots should not be reproduced in the new composition. When the user requests exact text, quote it verbatim and keep typography subordinate to the image.

## Iteration

After inspecting the result, revise one dominant failure at a time and repeat the source invariants. Do not rewrite the whole concept merely to add more effects.
