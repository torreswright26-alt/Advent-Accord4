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
The render dataset should include at least 20 approved references in each:
- environment,
- mood,
- character,
- intimate location.

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
