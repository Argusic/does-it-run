# OpenWorldLib

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenDCAI/OpenWorldLib, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/openworldlib

## Pinned environment

- Project commit: `32f7553566cc2081c78639a297962e1f86fc4808`
- Test commit: `32f7553566cc2081c78639a297962e1f86fc4808`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.5 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.5 | 4 | 4 | [run](https://argusic.com/run/0b36f5aa-7a41-4aa0-8277-1df4764c4269) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `pycuda failed to build (missing pyconfig.h / python3-dev headers, no root access)`
- 3 min: `torchaudio 2.11.0 incompatible with torch 2.5.1 (aoti_torch_abi_version symbol)`
- 1 min: `numpy 2.x incompatible with compiled pyarrow/pandas modules`
- 0.5 min: `plyfile module missing for VGGT pipeline`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
