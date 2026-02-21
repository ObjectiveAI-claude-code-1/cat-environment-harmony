# cat-environment-harmony

Scores how harmoniously a cat and its environment coexist in a photograph. Evaluates whether the light's mood matches the setting, the color palette accommodates the cat's coloring, and the cat looks like it belongs in the space — producing a unified visual world rather than a fragmented composite.

## Input

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `image` | `image` | Yes | A photograph of a cat within its surrounding environment. The image should capture the complete visual field — the cat, the space around it, the light falling across both, and the colors, textures, and shapes that populate the frame. |

The function considers the image as a whole, evaluating the relationship between the cat and its environment rather than any element in isolation. The breed of the cat and the category of environment are irrelevant — what matters is whether the visual elements of the scene speak the same language.

## Output

A scalar score between **0** and **1**.

- **High scores (near 1.0):** The photograph feels settled and harmonious. Light, environment, and cat exist as one coherent visual world. The viewer's eye rests comfortably — nothing feels out of place, contradictory, or assembled.
- **Mid scores (near 0.5):** The photograph shows partial harmony. Some elements agree while others introduce mild inconsistency. The image doesn't feel fractured, but it doesn't feel fully unified either.
- **Low scores (near 0.0):** The visual elements feel at odds. The photograph produces a fragmented or uneasy impression — the cat and its surroundings seem to belong to different images, as though assembled rather than observed.

## What It Evaluates

The function assesses three interconnected qualities. All three must be present for true harmony to emerge.

### 1. Tonal Cohesion

Does the emotional mood of the lighting agree with the emotional mood of the setting?

Every photograph carries an emotional temperature. Warm, diffused light suggests comfort; cool, sharp light suggests austerity. A cluttered, lived-in room speaks of domesticity; a stark landscape speaks of solitude. Tonal cohesion measures whether these registers agree — whether the light and the environment are telling the same story.

**High tonal cohesion:** Soft golden light in a cozy room. Cool, even light in a stark industrial space. The atmosphere is singular and settled.

**Low tonal cohesion:** Harsh, clinical light falling across a warm, intimate setting. The light tells one story while the space tells another, and the image fractures along that fault line.

### 2. Chromatic Sympathy

Does the environment's color palette work with the cat's natural coloring, or against it?

Chromatic sympathy evaluates whether the colors in the scene accommodate the cat gracefully — through harmonious echoes, gentle contrasts, or complementary relationships — rather than overwhelming or orphaning it. A ginger cat among autumn leaves achieves this effortlessly. A pale cat against an aggressively saturated background of competing primaries does not.

**High chromatic sympathy:** The cat's coloring finds quiet echoes or pleasing contrasts in its surroundings. The palette feels coherent. The cat is held by its environment.

**Low chromatic sympathy:** The surrounding colors are so disjointed or overpowering that the cat's appearance is diminished. The cat looks like a chromatic orphan — lost in a color argument that has nothing to do with it.

### 3. Spatial Belonging

Does the cat look like it was discovered in this place, or placed into it?

Spatial belonging evaluates whether the cat and its environment feel like they are part of the same photograph — the same moment, the same world. It considers consistency of depth, scale, texture, and visual weight across the frame. When spatial belonging is strong, the viewer accepts the scene without question. The cat is in its place.

**High spatial belonging:** The cat inhabits the space completely. Depth, texture, and scale are consistent. The space feels made to hold this cat.

**Low spatial belonging:** The photograph takes on a composite quality. The cat appears to float in front of its background. Scale or texture feels inconsistent, creating a sense of collage rather than a captured moment.

## Use Cases

- **Portfolio curation:** Identify which cat photographs achieve visual ease and unity — the images where the viewer's eye rests comfortably rather than searching for resolution.
- **Content selection:** Find photographs that feel polished and intentional for publications or social media, where the cat appears discovered within its setting rather than dropped into it.
- **Photographic diagnostics:** When a photograph feels wrong but the individual elements seem fine, this function can articulate what the photographer senses but struggles to name — the elements are not working together.
- **Environment design:** Score photographs across many settings to reveal which kinds of spaces, palettes, and lighting conditions tend to produce unity, guiding decisions about where and how to photograph cats.
- **Batch filtering:** Automatically rank or filter large collections of cat photographs by visual harmony, surfacing the most cohesive images.