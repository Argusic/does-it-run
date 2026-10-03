# MOSS-TTS

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenMOSS/MOSS-TTS, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/moss-tts

## Pinned environment

- Project commit: `934d6826b084c46a0d033402174d5f8ac4ed2519`
- Test commit: `934d6826b084c46a0d033402174d5f8ac4ed2519`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31.3 to 31.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 31.3 | 7 | 7 | [run](https://argusic.com/run/48f9ab83-aa0d-4f45-a542-8394a8b33cae) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `pyproject.toml [tool.setuptools] py-modules = [] prevented package discovery - CLI script and package imports failed`
- 2 min: `moss_tts_delay/__init__.py and moss_tts_realtime/__init__.py missing`
- 3 min: `torch==2.9.1+cu128 not installable on CPU-only machine`
- 1 min: `torchcodec==0.8.1 not available; installed 0.17.0`
- 5 min: `mossttsrealtime subpackage not discoverable through editable finder`
- 3 min: `moss_tts_local_v1.5 directory name with dot prevents Python package import`
- 2 min: `moss_soundeffect_v2 requires ftfy, audiotools, diffusers - not all installable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
