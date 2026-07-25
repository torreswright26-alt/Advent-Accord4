# Generation Workflow

## Default Assumption
Ask what the image is for. It may be:

- renderer reference development,
- fixed-seed renderer evaluation,
- continuity testing,
- controlled correction,
- panel production,
- concept-only exploration.

Do not treat attractive generations as training data by default. Generated
images enter training only after explicit user approval.

## Commands
- `again`: incorporate critique and regenerate.
- `next`: resume the sequence.
- `stop`: stop generating.
- `approve` / `approved`: save current image as the next chronological approval.

## Approval Process
On approval:
1. Assign next ID.
2. Rename file using the fixed convention.
3. Add manifest entry.
4. Record category and metadata.
5. Flag as benchmark only when explicitly appropriate.
6. Preserve the original file.

## Categories
- Environment
- Mood
- Character
- Intimate location

## Scene Variation
Every generation should vary scene and composition unless the user asks for a controlled revision.

## Current Production Boundary

Renderer R1 text-to-image successfully holds broad design vocabulary, clothing
family, props, location features, and rendering grammar. It does not maintain
exact facial identity, mature age, scars, freckles, or fine garment
construction reliably across new seeds.

Low-denoise Z-Image img2img preserves composition, pose, clothing, prop,
location, light, and style well enough for local corrections, but it did not
solve structural age or exact identity.

Do not claim panel-ready continuity yet. The next workflow layer must benchmark
explicit identity/reference conditioning or a dedicated controlled editor.
