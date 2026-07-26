# AI Handoff Manual

## Purpose
Allow any competent AI system to begin work without requiring the user to restate the project.

## Startup Procedure
1. Read `README.md`.
2. Read `Docs/22_CURRENT_RENDERER_STATUS.md`.
3. Read the relevant files under `Docs/`.
4. For visual work, inspect approved references and manifest metadata.
5. For training work, inspect configs and experiment history.
6. Do not make canon claims from filenames alone.

## Visual Work
- Use approved benchmark images as the highest visual authority.
- The current renderer authority is the three-image core defined in
  `02_ART_DIRECTION.md`.
- Historical approval `002` remains a composition/environment reference but no
  longer outranks the core aesthetic.
- Maintain painterly selective detail.
- Avoid hyperrealism, overtexturing, particulate density, generic anime drift,
  polite cartoon drift, happy-adventure default, narrow palette behavior, and
  geometric clutter.
- Preserve composition variety.
- Evaluate anatomy, character design, dimensionality, environment, color, and
  detail as separate axes; do not collapse them into one preference score.
- Treat anatomy, mature character specificity, and modeled form as threshold
  requirements. Environment density or cohesive color cannot compensate for
  failures in those areas.
- Preserve useful lived-in environmental density while correcting a weak
  character. Do not flatten the room merely because its figure needs revision.
- Distinguish material detail from visual noise. Seams, layering, closures,
  wear, joinery, tools, and task-specific objects are valuable; particles,
  repetitive micro-marks, and evenly distributed texture are not.
- A polished concept-art finish can still be off-target. Favor selective
  resolution, connected shadow masses, quiet surfaces, lost-and-found edges,
  and painterly transitions.
- Preserve structural silhouette integrity. Painterly softness must not cause
  locations, architecture, terrain, foliage, or water boundaries to dissolve
  into ambiguous geometric fragments.
- "Cleaner shapes" means coherent large masses, readable overlaps, continuous
  identity-defining boundaries, and smoother connected planes—not universal
  outlines, sterile precision, photorealism, or increased micro-detail.
- Treat an otherwise successful atmospheric image with slightly undefined
  environmental shapes as a refinement candidate, not an automatic rejection.
  Preserve its composition, palette, mood, and painterly strengths while
  improving structural legibility.

## Dataset Work
- Never promote candidates automatically.
- Never use rejected assets.
- Keep holdout references outside training.
- Maintain manifest IDs chronologically.
- Do not ask for or generate more renderer references until current R2 results
  demonstrate a specific missing coverage category.

## Story Work
- Preserve opening canon.
- Preserve character appearance and personality.
- Respect pacing and panel rules.
- Do not add unrequested subchapters.

## Change Management
- Add new rules to the most relevant document.
- Add the decision to `20_CANON_DECISIONS.md`.
- Add the repository change to `21_CHANGELOG.md`.
- Do not repeatedly restructure the repository.

## Authority Order

When documents conflict:

1. the user's latest explicit decision;
2. `22_CURRENT_RENDERER_STATUS.md`;
3. dated decisions in `20_CANON_DECISIONS.md`;
4. other repository guidance;
5. historical experiments and filenames.

Do not revert to an older renderer, benchmark hierarchy, or broad dataset target
merely because it appears elsewhere in the repository.
