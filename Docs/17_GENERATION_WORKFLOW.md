# Generation Workflow

## Default Assumption
Advent Accord image requests are for render-LoRA reference generation unless explicitly stated otherwise.

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
