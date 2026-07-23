# Training Pipeline

## Separation of Concerns
Use separate systems where practical:
1. Render-style LoRA
2. Character LoRAs for true main cast
3. Environment LoRA
4. Future manifestation-specific solution only after diversity exists

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

## Evaluation
Use fixed prompts, fixed seeds, fixed resolutions, and fixed LoRA-weight sweeps.
