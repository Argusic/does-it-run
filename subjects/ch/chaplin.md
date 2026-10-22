# chaplin

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amanvirparhar/chaplin, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/chaplin

## Pinned environment

- Project commit: `7aee1f8fca776ce4f63690063310b53573b7d804`
- Test commit: `7aee1f8fca776ce4f63690063310b53573b7d804`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1 to 23.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1 | 0 | 0 | [run](https://argusic.com/run/b077165b-6a18-4a5e-9043-ebb2da2e1053) |
| 2 | pass | 100 | 48 | 23.3 | 10 | 10 | [run](https://argusic.com/run/6267a702-04d5-4944-b3f9-463f1bc78841) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `pip install failed due to externally-managed-environment`
- 1 min: `evdev build failed - missing Python.h (system python3-dev not installed, no root)`
- 3 min: `mediapipe 1.1.0 removed mp.solutions API, breaking detector`
- 3 min: `mediapipe 0.10.20 requires numpy<2, conflicting with opencv-python 5.x`
- 8 min: `torchvision.io.read_video not available in torchvision 0.29`
- 2 min: `espnet.nets.pytorch_backend.e2e_asr.to_device not found (missing module)`
- 8 min: `Chaplin class hangs on __init__ due to async event loop init race condition`
- 2 min: `hydra.main got unexpected keyword argument version_base (hydra-core 0.11 vs 1.3)`
- 5 min: `wget not installed, setup.sh failed`
- 1 min: `No /dev/video0 (no webcam in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
