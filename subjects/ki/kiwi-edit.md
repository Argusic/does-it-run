# Kiwi-Edit

**Verdict: could not verify.** Argusic Score 42.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/showlab/Kiwi-Edit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/kiwi-edit

## Pinned environment

- Project commit: `178f3f4f8221d7598fcc21875c847d6cf6323c4e`
- Test commit: `178f3f4f8221d7598fcc21875c847d6cf6323c4e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 6.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 40 | 4.5 | 8.4 | 4 | 2 | [run](https://argusic.com/run/8438e21f-41ee-4bf8-afcc-1e5dfbd8bbc4) |
| 2 | fail | 45 | 8 | 6.4 | 4 | 3 | [run](https://argusic.com/run/a6b5c838-1a83-44fa-a921-26a77cb78433) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Missing module deepspeed`
- 0.2 min: `Missing module wandb`
- `No CUDA GPU available , inference requires GPU`
- `Demo target videos (tgt_video) missing from repo (demo_data/video/target/ does not exist)`

Attempt 2:

- 1 min: `Python 3.12 vs required 3.10, no conda available`
- 2 min: `VideoData.__init__ crashed with TypeError: '<' not supported between instances of 'int' and 'NoneType'`
- `No CUDA GPU in container - cannot run model inference`
- 2 min: `huggingface-hub version conflict: transformers requires <1.0, datasets/diffusers require >=1.31.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
