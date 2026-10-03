# whisper-asr-webservice

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ahmetoner/whisper-asr-webservice, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/whisper-asr-webservice

## Pinned environment

- Project commit: `ec32cd50b508412e0b8ebe81c26cd7a7dc900b7a`
- Test commit: `ec32cd50b508412e0b8ebe81c26cd7a7dc900b7a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.8 to 13.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 13.8 | 1 | 1 | [run](https://argusic.com/run/9df60faf-0ba6-4874-a15c-c0e5fd424511) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Poetry not pre-installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
