# Scene Routing and Reference Selection

Lock the preservation anchor and central proposition before selecting references. Select zero or one primary reference for composition logic. Add at most one secondary reference for space, material, or human treatment only when a primary is already justified. The uploaded source remains the content anchor. If every bundled image introduces a stronger template than it solves, use no bundled reference.

All paths are relative to the skill root.

## Bundled references

| Reference | Best used for | Transferable relationship | Do not copy |
|---|---|---|---|
| `assets/references/folded-field.jpg` | everyday landscape, lone figure, road, field | a familiar environment becomes one dominant impossible space; tiny scale cues remain calm | rectangular wall, child, bicycle, utility poles, green palette |
| `assets/references/water-town-rift.jpg` | architecture, street, canal, village | overhead spatial field coexists with upright side-view structures; bold curved negative mass | river, bridge, white houses, S-curve |
| `assets/references/fashion-garment-space.jpg` | portrait, fashion, dancer, expressive pose | preserve bodily rhythm while clothing or gesture organically expands into extreme perspective | model identity, black gown, diagonal runway, hat pose |
| `assets/references/classroom-pages.jpg` | group, interior, repeated objects | overhead repeated modules change state while upright people preserve group hierarchy | students, books, classroom, exact large-right figure |
| `assets/references/mythic-city-invasion.jpg` | city, procession, historical or epic narrative | city scale overwhelms figures; one dark path carries action and fate | ancient city, warrior, black road, exact aerial layout |
| `assets/references/underworld-void.jpg` | sparse psychological scene, grief, memory, ritual | huge clean emptiness, dissolving crowd boundary, tiny emotional anchor | underworld, semicircular crowd, kneeling warrior, blood mark |

## Routing by source type

### Mixed-scene arbitration

Classify by the relationship that must survive, not by the largest object in the frame.

| Primary preservation anchor | Route | Tie-break rule |
|---|---|---|
| identity, pose, gaze, bodily rhythm | single person | use environmental scale only as a secondary mechanism |
| who faces, follows, opposes, isolates, or elevates whom | group | preserve orientation/aspect ratio when lateral placement carries the relation |
| path, horizon, facade, bank, room, or landmark structure | landscape / architecture / interior | choose viewpoint conflict for spatial contradiction; choose monumental depth only for scale hierarchy |
| silhouette, function, grip, support, or contact point | object | choose subject-becomes-space only when its function supports it; otherwise use active cut or sparse scale |

For a lone person inside a vast landscape, choose **single person** when pose or identity drives the image and **landscape** when distance or terrain drives it. For a group in a large environment, choose **group** whenever the human relation is the narrative anchor; the environment may support but must not overwrite it. For an empty interior, route as architecture/interior.

### Landscape or lone figure in an environment

- Preserve: horizon/path relation, subject placement, one factual object.
- Prefer: `folded-field.jpg`.
- Optional secondary: `underworld-void.jpg` for silence or `mythic-city-invasion.jpg` for epic scale.
- Risks: copying the folded rectangle; shrinking every subject into the same lower-corner position.

### Architecture, street, village, or city

- Preserve: landmark hierarchy, circulation path, facade/ground relationship.
- Prefer: `water-town-rift.jpg` for viewpoint conflict or `mythic-city-invasion.jpg` for monumental depth.
- Optional secondary: `underworld-void.jpg` for sparse atmosphere.
- Risks: tourism illustration, literal portal, dense architectural detail, repeated staircases.

### Single person, fashion, dance, or close portrait

- Preserve: identity when needed, pose, gaze, silhouette, hands, and bodily rhythm.
- Prefer: `fashion-garment-space.jpg`.
- Optional secondary: `folded-field.jpg` for environmental scale or `underworld-void.jpg` for psychological emptiness.
- Risks: ordinary fashion illustration, photoreal retouch, over-geometric body, malformed hands, garment turning into a generic road.

### Group, classroom, meeting, performance, or crowd

- Preserve: primary action, who is elevated or isolated, directional attention, and a meaningful count range.
- Prefer: `classroom-pages.jpg`.
- Optional secondary: `underworld-void.jpg` for crowd-as-boundary or `fashion-garment-space.jpg` for organic figure treatment.
- Risks: copied faces, literal repeated props, decorative grid, too many equal focal points.
- Do not introduce long cast shadows unless they are already visible and structurally important in the source.

### Object, vehicle, food, product, or close-up

- Preserve: silhouette, function, contact points, and one material cue.
- Choose the reference whose relationship fits the concept rather than the subject noun: subject-becomes-space (`folded-field`), active cut (`water-town-rift`), or sparse scale (`underworld-void`).
- Risks: glossy product render, random surreal hybrid, giant object without a meaningful scale relation.

## Selection limits

- Normally use the source plus zero or one primary reference.
- Add a secondary reference only for one missing domain.
- Never use more than two bundled style references in one generation.
- If two references visibly compete, remove the secondary rather than blending harder.
