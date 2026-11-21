# pint

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/cloudflare/pint, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/pint

## Pinned environment

- Project commit: `39ba145ee6b7c33050133dc572437e17931e0fde`
- Test commit: `39ba145ee6b7c33050133dc572437e17931e0fde`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.4 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.4 | 0 | 0 | [run](https://argusic.com/run/c296e43e-46b7-4997-b9da-e9e67a3b00c8) |
| 2 | pass | 100 | 0.5 | 9.8 | 0 | 0 | [run](https://argusic.com/run/796e6c7c-82c7-4e03-b064-2c87fed344fb) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
