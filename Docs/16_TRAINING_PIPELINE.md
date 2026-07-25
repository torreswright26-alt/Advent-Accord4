# Training Pipeline

## Separation of Concerns
Use separate systems where practical:
1. Render-style LoRA
2. Character LoRAs for true main cast
3. Environment LoRA
4. Future manifestation-specific solution only after diversity exists

## Current Foundation

- Local base: Z-Image Base BF16.
- Hardware target: RTX 4080 SUPER 16 GB / 64 GB system RAM.
- Training tool: Musubi Tuner.
- Renderer-only LoRA; do not mix character identity, location canon, or
  manifestation concepts into the style module.
- Cache latents and text-encoder outputs.
- Save intermediate checkpoints in one run and select by fixed-seed evaluation.

## Main-Cast LoRAs
Likely candidates:
- Adult Sol
- Child Sol if necessary
- Kael
- Vryn
- Auric

Minor characters should generally use reference packages rather than dedicated LoRAs.

## Experiment Rules
Every experiment records:
- experiment ID,
- parent experiment,
- hypothesis,
- changed variable,
- unchanged variables,
- dataset version,
- captions version,
- base model,
- resolution,
- rank,
- optimizer,
- learning rate,
- steps,
- seed suite,
- output checkpoints,
- evaluation result.

## One-Variable Rule
Do not change dataset, learning rate, rank, repeats, optimizer, and steps all at once.

When a run changes more than one tightly related variable, document the
combined correction hypothesis explicitly. Renderer R2 intentionally changes
weighting, shared caption language, and learning rate together because all
three address the same demonstrated over-polite/cartoon failure. R1 remains
preserved as the control.

## Evaluation
Use fixed prompts, fixed seeds, fixed resolutions, and fixed LoRA-weight sweeps.

Do not choose the final epoch automatically. Evaluate intermediate checkpoints
for style fidelity, prompt adherence, acting, anatomy, environment rendering,
palette range, and leakage.

## Current Experiments

### Renderer R1 — complete

- 20 equally repeated images.
- Rank/alpha 32/32.
- `5e-5`, AdamW8bit, BF16.
- Eight epochs / 960 steps.
- Epoch 6 selected from base/epoch-2/4/6/8 screening.
- Result: technically successful and attractive, but too polite, cartoony,
  cheerful-adventure-coded, outline-dependent, and narrow in mature color and
  emotional behavior.

### Renderer R2 — training launched

- Fresh from Z-Image Base.
- Same 20 images; no new generation.
- Core-weighted dataset described in `15_DATASET_POLICY.md`.
- Trigger: `aa_mature_renderer`.
- Rank/alpha 32/32.
- `3e-5`, AdamW8bit, BF16, eight epochs / 864 steps.
- Goal: mature painterly dimensionality, broader palette and mood, deeper
  colored shadows, richer material transitions, and reduced outline reliance.
- Status at documentation update: local training is active; all 40 cache files
  are present and no epoch checkpoint had been written at the last read-only
  check. Completion and checkpoint selection remain pending.
