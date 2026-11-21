# Irodori-TTS

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Aratako/Irodori-TTS, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/irodori-tts

## Pinned environment

- Project commit: `89f9d8fbd4d51ea019867ee1197725ede1df13c5`
- Test commit: `89f9d8fbd4d51ea019867ee1197725ede1df13c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 7.8 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 7.8 | 0 | 0 | [run](https://argusic.com/run/575fd737-5f35-4c25-92b2-1e11f906843a) |
| 2 | pass with mocks | 92 | 5 | 18.7 | 3 | 3 | [run](https://argusic.com/run/4bbcdc7f-7a80-406e-bbd0-2a8a7e14149d) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `uv (package manager) not available in base environment`
- 1 min: `soundfile.LibsndfileError: Format not recognised when writing audio tensor with shape [1, N]`
- 3 min: `Full checkpoint (2.6GB) could not be downloaded - OOM killed (1.9GB RAM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
