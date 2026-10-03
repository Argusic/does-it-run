# VoiceMem

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xzf-thu/VoiceMem, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/voicemem

## Pinned environment

- Project commit: `6cacb3c1e7fca2679f3bf95451f6b480efd9a783`
- Test commit: `6cacb3c1e7fca2679f3bf95451f6b480efd9a783`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.3 to 15.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 15.3 | 6 | 6 | [run](https://argusic.com/run/8854f5ba-4b64-457d-90f2-195ad8816ebf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `externally-managed-environment: system Python 3.12 blocks system-wide pip install (PEP 668)`
- 1 min: `BackendUnavailable: Cannot import 'setuptools.build_meta' (setuptools not in fresh venv)`
- 3 min: `torchvision 0.29.1 incompatible with torch 2.13.0 (RuntimeError: operator torchvision::nms does not exist)`
- 1 min: `sentence-transformers 6.1.0 requires transformers>=5.0.0, conflicting with pinned transformers==4.52.3`
- 2 min: `pip install funasr/modelscope hung (corrupted pip cache)`
- `sounddevice requires PortAudio system library (OSError: PortAudio library not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
