# Amphion

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/open-mmlab/Amphion, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/amphion

## Pinned environment

- Project commit: `26f6883110181f1dbfe95c70a7c7dbaf4de5f42a`
- Test commit: `26f6883110181f1dbfe95c70a7c7dbaf4de5f42a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.1 to 25.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 25.1 | 6 | 6 | [run](https://argusic.com/run/60fe3cb8-a6da-4543-b5fb-c091176947ad) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `pyworld, pysptk, pesq, webrtcvad failed to build from source: missing python3-dev (Python.h header). No root access to install it.`
- 1 min: `Multiple missing __init__.py files in modules/ subdirectories (modules/base, modules/diffusion/bidilconv, modules/diffusion/karras, modules/diffusion/unet, modules/flow, modules/naturalpseech2, modules/wenet_extractor/*)`
- 1 min: `fairseq missing version.txt - failed pip install from git`
- 1 min: `librosa 0.9.1 requires pkg_resources from setuptools; newer setuptools broke it`
- 1 min: `lhotse not installed (required by modules/general)`
- 1 min: `transformers 5.x missing soxr dependency for Wav2Vec2`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
