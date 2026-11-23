# opik-openclaw

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/comet-ml/opik-openclaw, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opik-openclaw

## Pinned environment

- Project commit: `0d65e6f4a5f277285d9bb7bb59179f0be304972d`
- Test commit: `0d65e6f4a5f277285d9bb7bb59179f0be304972d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 4.9 | 1 | 1 | [run](https://argusic.com/run/b8847b52-e741-49bc-b9a7-ffd15df36dcc) |
| 2 | pass with mocks | 92 | 0.25 | 2 | 1 | 1 | [run](https://argusic.com/run/81a664f0-9447-4667-8ca4-47b73e819514) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 is installed but the project requires >=22.12.0`

Attempt 2:

- 0.1 min: `Node.js v18.19.1 was installed, but the project requires >=22.12.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
