# Dataset Policy

## Render Dataset Folders
- `approved/`: approved images eligible for curation.
- `candidates/`: not yet approved.
- `rejected/`: excluded from training.
- `holdout/`: approved but withheld for evaluation.
- `benchmarks/`: represented through manifest flags; avoid duplicate authoritative files unless required by tooling.

## Training Admission
Only manually approved images may enter training.

## Balance

Do not pursue fixed category counts before renderer fidelity is established.
The first clean-slate renderer run uses a small, tightly governed 20-image pool.
Quality, aesthetic authority, caption clarity, and effective weighting outrank
round-number collection targets.

Add new images only when they fill a demonstrated gap. More images are not
automatically better.

## Variation Requirements
Balance:
- orientation,
- camera,
- lighting,
- weather,
- palette,
- interior/exterior,
- crowd density,
- scale,
- architecture,
- character distance,
- quiet/action scenes.

## Captioning
Captions should describe:
- content,
- composition,
- light,
- palette,
- material simplification,
- style-relevant properties.
Avoid encoding accidental defects.

Caption rendering properties directly. Do not rely on broad labels such as
“anime-influenced” when they can produce flat animation behavior. Describe:

- softly modeled dimensional facial planes;
- matte skin with nuanced warm-cool transitions;
- deep readable colored shadows;
- painterly material transitions;
- controlled intricacy;
- selective edges and minimal outline reliance;
- scene-specific mood and palette rather than a universal emotional tone.

## Weighting and Authority

Approval does not imply equal training weight.

- Core anchors may receive higher effective weight when they define the
  renderer aesthetic.
- Bridge references support transfer and breadth.
- Harder or stylistically peripheral references may receive reduced weight or
  remain holdouts.
- Weighting must be documented as part of the experiment.

The current Renderer R2 plan uses the same 20 admitted images:

- three core anchors ×14 repeats;
- sixteen bridge references ×4 repeats;
- one harder coastal edge case ×2 repeats.

This produces 108 effective samples per epoch and 38.9% core-anchor influence.
