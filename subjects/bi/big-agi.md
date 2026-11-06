# big-AGI

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/enricoros/big-AGI, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/big-agi

## Pinned environment

- Project commit: `00715049819786dc66bb6961a5795dd538e79f29`
- Test commit: `00715049819786dc66bb6961a5795dd538e79f29`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 0.2 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 8.9 | 0 | 0 | [run](https://argusic.com/run/11d0871e-ec47-453a-ae41-011554c9495a) |
| 2 | fail | 20 | n/a | 0.2 | 0 | 0 | [run](https://argusic.com/run/217b28ee-3c0b-43ff-aa99-6649093f64c4) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
