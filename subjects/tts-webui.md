# TTS-WebUI

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rsxdalv/TTS-WebUI, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/tts-webui

## Pinned environment

- Project commit: `2e5701387c423307d73972a45496bfdcb6a7d8e1`
- Test commit: `2e5701387c423307d73972a45496bfdcb6a7d8e1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.2 | 5.9 | 2 | 2 | [run](https://argusic.com/run/30eb5dbc-1657-4b9b-9400-3f8f2903c059) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pyopenjtalk-prebuilt==0.3.0 fails to build on Python 3.12 (distutils removed, Cython compile error); depends on tts-webui-extension-vall-e-x -> tts-webui-valle-x. Skipped installing this package.`
- 1 min: `torchaudio C shared library (_torchaudio.abi3.so) fails to load: libcudart.so.13 not found. Causes errors in seamless_m4t and simple_remixer extensions at startup.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
