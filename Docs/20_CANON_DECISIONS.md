# Canon Decisions

## Approved Visual References
- Adult Sol: latest approved multi-pose adult illustration.
- Vryn: latest approved reference with increased color variety.
- Auric: latest approved mentor reference.
- Kael: established white-hair, purple-eye reference.

## Render Style
- As of 2026-07-24, the three core aesthetic anchors are the primary renderer
  authority: koi-garden woman, original intricate dark-coat man, and seated
  pendant woman.
- Approval `002` remains useful composition and environment evidence but no
  longer outranks the three core anchors for renderer style.
- Approval `003` remains an approved wide environmental reference and does not
  replace the three core anchors.
- Painterly selective detail is preferred over hyperreal or highly textured rendering.
- Approved render references should collectively vary palette, location, weather, mood, environment, character age, body type, occupation, hair color, eye color, and manifestation medium where active.
- Mature painterly dimensionality must not collapse into polite cartoon,
  cheerful adventure, uniform youthfulness, narrow safe color, or dark-outline
  dependence.
- “Mature” must not be interpreted as universally grim, dark, desaturated,
  gritty, or photorealistic.

## Renderer Training Decisions

- Z-Image Base is the selected local renderer foundation.
- Renderer LoRAs remain style-only.
- Renderer R1 completed; epoch 6 was technically selected but the family is not
  accepted as final because it remains too polite and cartoony.
- Renderer R2 uses the same 20 images with stronger core weighting and revised
  mature rendering captions. More generated references are not currently
  required.
- Exact identity continuity remains a separate workflow problem and must not be
  solved by contaminating the renderer-style LoRA.

## Visual Evaluation Decisions

- As of 2026-07-26, visual comparisons must keep anatomy/pose, character
  design/maturity, dimensional rendering, environment density, color cohesion,
  shadow structure, and selective detail as separate evaluation axes.
- Anatomy, mature character specificity, and dimensional form are threshold
  requirements. Strong environment construction or color does not erase
  shortcomings in those areas, but those successful setting qualities should
  be preserved in the next iteration.
- Clothing and environmental detail are desirable when they communicate
  construction, material, culture, use, or story. This material detail must not
  be conflated with particulate effects, repetitive micro-marks, or uniform
  texture density.
- The target may be highly finished, but it must not collapse into uniformly
  polished promotional concept art. Selective resolution, painterly
  transitions, quiet surfaces, and lost-and-found edges remain required.

## Workflow
- Approved render images receive chronological IDs.
- Render manifest must remain updated.
- Generation commands: again, next, stop, approve/approved.

## Manifestation
- Sol's manifestation is smoke-dominant, red-orange with silver streaks.
- Manifestations preserve environment identity before full manifestation.
- Manifestations should vary by medium as a core identity, not merely by color or shape.
