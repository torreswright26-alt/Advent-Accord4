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
