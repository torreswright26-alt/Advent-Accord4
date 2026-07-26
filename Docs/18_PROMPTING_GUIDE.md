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

## Prompt Priorities for New Characters

For a new character, specify design before decorative finish:

1. age and mature facial structure;
2. body build, weight, posture, and balance;
3. role, temperament, and immediate intention;
4. silhouette, grooming, and culturally authored wardrobe;
5. garment construction, material weight, and a few meaningful details;
6. hand placement and contact with relevant objects;
7. relationship to the setting and its light.

For environments, describe why the place exists and how it is used. Name
purposeful evidence of work, storage, maintenance, habitation, ceremony, or
weather rather than requesting generic "high detail" or "clutter."

Useful phrasing:

- selective garment detail following seams, layers, closures, and material;
- lived-in room with purposeful tools, storage, wear, and circulation;
- character and setting unified by one cohesive light and palette;
- deep shaped shadows with readable interior color;
- resolved face and hands, quieter secondary surfaces;
- painterly transitions and lost edges outside the focal area.
- clean readable large silhouettes without heavy outlines;
- coherent rooflines, structural masses, and negative spaces;
- smooth connected planes with selective painterly breakup;
- atmospheric softness that preserves location identity;
- recognizable architecture and terrain before surface detail;
- selective crisp edges at form-defining corners, overlaps, and openings.

Use `aa_mature_renderer` after an R2 checkpoint has been selected and installed.
Until then, treat it as training vocabulary rather than a production guarantee.

Put subject, action, and place first. Describe rendering behavior after scene
facts. Keep palette and mood scene-specific so the renderer does not learn one
universal color script.
