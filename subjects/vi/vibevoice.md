# VibeVoice

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/VibeVoice, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vibevoice

## Pinned environment

- Project commit: `16fb2cb1217c9934a886e1948ffb06120caa2df5`
- Test commit: `16fb2cb1217c9934a886e1948ffb06120caa2df5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.3 to 17.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 17.3 | 3 | 3 | [run](https://argusic.com/run/689470ae-83af-4123-b0ab-231d32bc4d9d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install -e . refused on system Python: externally-managed-environment (PEP 668)`
- 4 min: `Gradio launch produced empty log and exited when started from a non-interactive shell (first attempt)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
