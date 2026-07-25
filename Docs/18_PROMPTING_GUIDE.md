# Prompting Guide

## Preferred Prompt Structure
1. Scene purpose
2. Location
3. Camera and composition
4. Lighting and weather
5. Character activity
6. Palette
7. Painterly style constraints
8. Explicit exclusions

## Style Constraints
Use language such as:
- painterly first,
- selective detail,
- medium-frequency detail,
- broad value groups,
- grouped foliage,
- simplified stone and fabric,
- restrained particulate density,
- controlled edge hierarchy,
- cinematic but not photorealistic.
- mature painterly-dimensional illustration,
- softly modeled dimensional facial planes,
- nuanced warm-cool transitions,
- deep readable colored shadows,
- rich material transitions,
- emotionally specific expression,
- minimal reliance on dark outlines,
- no automatic cheerful-adventure tone.

## Avoid
- generic keyword piles,
- "ultra detailed",
- "8k",
- "hyperrealistic",
- "photorealistic",
- "intricate texture everywhere",
- repeated gothic skyline defaults.
- “anime-influenced” as a universal style label,
- generic “beautiful fantasy character” wording,
- automatic friendly, heroic, or optimistic emotional framing,
- using darkness, grime, or texture as shorthand for maturity.

## Current R2 Trigger

Use `aa_mature_renderer` after an R2 checkpoint has been selected and installed.
Until then, treat it as training vocabulary rather than a production guarantee.

Put subject, action, and place first. Describe rendering behavior after scene
facts. Keep palette and mood scene-specific so the renderer does not learn one
universal color script.
