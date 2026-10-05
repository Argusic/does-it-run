# corteza

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cortezaproject/corteza, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/corteza

## Pinned environment

- Project commit: `3835dfc4ac8bd89381753f09042ad147a4502576`
- Test commit: `3835dfc4ac8bd89381753f09042ad147a4502576`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 62.6 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/970a202c-78e2-4ec6-bdb2-261561d7187e) |
| 2 | pass | 100 | 18 | 62.6 | 3 | 3 | [run](https://argusic.com/run/f76b5a27-fc7b-41e2-97dd-6ff2195bba2e) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go compiler not installed in container`
- 1 min: `Build OOM-killed due to parallel compilation on 2GB RAM`
- 1 min: `Locale unit test failed: could not find en in loaded languages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
