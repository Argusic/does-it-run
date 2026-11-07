# hass-xiaomi-miot

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/al-one/hass-xiaomi-miot, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/hass-xiaomi-miot

## Pinned environment

- Project commit: `919b7a49bb3215a22ad56cbb5b6eea026c391691`
- Test commit: `919b7a49bb3215a22ad56cbb5b6eea026c391691`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.3 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 4.3 | 1 | 1 | [run](https://argusic.com/run/56818b15-78c7-43e2-8d56-25afe9d49f77) |
| 2 | pass with mocks | 92 | 40 | 4.7 | 2 | 2 | [run](https://argusic.com/run/ad46e718-1b40-4d40-929c-c0ab702d6a4f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `netifaces failed to build (missing python3-dev headers, no root access in container)`

Attempt 2:

- 20 min: `pip install -r requirements_test.txt failed on host Python 3.12: netifaces 0.11.0 has no wheel and its build failed with 'Python.h: No such file or directory' (no python3-dev, no root)`
- 10 min: `Real Mi Cloud login needs live Xiaomi credentials, unavailable in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
