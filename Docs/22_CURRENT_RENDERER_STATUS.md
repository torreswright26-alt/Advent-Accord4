# Current Renderer Status

Updated: 2026-07-25  
Purpose: concise cross-chat handoff for current Advent Accord visual work.

## Current Goal

Build a repeatable local image-to-panel production system. The immediate gate
is a renderer that reproduces the user's mature painterly-dimensional art
direction from text-to-image before character systems, panel assembly, or
lettering are scaled.

## Current Aesthetic Authority

The three primary renderer anchors are:

1. beautiful seated woman beside a koi pond;
2. original intricate dark-coat full-body man;
3. original seated pendant woman.

They define:

- softly modeled dimensional faces;
- stylized but anatomically grounded construction;
- mature, specific expression;
- shaped light and readable colored shadows;
- soft rich material transitions;
- intriguing clothing and controlled intricacy;
- beauty and atmosphere without photographic/PBR treatment;
- minimal dependence on heavy outlines.

Do not copy their people, clothing, koi garden, dark room, window pose, palette,
or architecture by default.

## User Correction

Renderer R1 art is attractive but too polite and cartoony. It suggests happy
adventure, loses color variety and maturity, and relies too much on clean
animation-like outlines and simplified surfaces.

The correction is not “make everything darker or grittier.” Preserve beauty,
romance, leisure, ceremony, color, humor, and wonder while adding dimensional
modeling, mature emotional range, deeper colored shadows, authored materials,
and wider palette behavior.

## Local Foundation

- Base: Z-Image Base BF16.
- Training: Musubi Tuner, renderer-only LoRA.
- Hardware: RTX 4080 SUPER 16 GB, 64 GB RAM.
- Local source of operational truth:
  `C:/AI/ComfyUI_windows_portable/advent_accord_lora/PROJECT_MEMORY.md`.

## Renderer R1

- Same 20 admitted images at equal repeat weight.
- Rank/alpha 32/32, BF16, AdamW8bit, `5e-5`.
- Eight epochs / 960 steps.
- Epoch 6 selected through fixed-seed base/epoch-2/4/6/8 screening and broader
  finalist tests.
- Result: meaningful improvement over base, but not accepted as final because
  it remains too polite, cartoony, cheerful-adventure-coded, and narrow in
  mature color/emotional behavior.

R1 must remain preserved as a control.

## Renderer R2

Status at this update: local training has been launched. All 20 latent caches
and all 20 text-encoder caches are present. No epoch checkpoint had been written
at the last read-only check, so completion is not yet recorded here.

- Fresh from Z-Image Base.
- Same 20 explicitly admitted images; no new generation.
- Three core anchors ×14 repeats.
- Sixteen bridges ×4 repeats.
- One harder coastal edge case ×2 repeats.
- 108 samples/epoch; 38.9% core-anchor influence.
- Trigger: `aa_mature_renderer`.
- Rank/alpha 32/32, BF16, AdamW8bit, `3e-5`.
- Eight epochs / 864 steps.

Caption correction removes broad `anime-influenced` language and directly
teaches mature dimensional faces, nuanced expression, painterly material
transitions, deep colored shadows, wide palette behavior, controlled
intricacy, and minimal outline reliance.

Do not generate more training references until R2 reveals a concrete missing
coverage category.

## Production Workflow Findings

R1 text-to-image can preserve:

- broad character design vocabulary;
- clothing family and palette;
- props;
- location features;
- rendering grammar.

It does not reliably preserve:

- exact face;
- mature age;
- scars or freckles;
- fine garment construction across new seeds.

A 0.35-denoise Z-Image img2img test preserved composition, pose, outfit, prop,
room, light, and renderer style and added minor facial details. It did not
convincingly change structural age.

Conclusion: exact identity continuity needs a separate reference/identity or
controlled-edit layer. Do not retrain or contaminate the renderer-style LoRA to
solve that problem.

## Immediate Resume Action

1. Determine whether the active Renderer R2 training has completed locally.
2. If complete, inventory and convert all checkpoints for ComfyUI.
3. Run a compact fixed-seed screen against R1 and Z-Image Base.
4. Select intermediate checkpoints by reference fidelity, maturity, palette,
   prompt adherence, anatomy, and leakage—not by final epoch number.
5. Only after renderer progress is accepted, resume identity-continuity tooling.

## Efficiency Rule

Prefer experiments that answer one demonstrated question. Do not spend usage on
broad generation, new training references, character LoRAs, panel tooling, or
large workflow systems before the renderer gate is meaningfully improved.
