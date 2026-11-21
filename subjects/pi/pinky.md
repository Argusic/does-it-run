# pinky

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DIYgod/pinky, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/pinky

## Pinned environment

- Project commit: `aa2a5c52ab6f6573a2c4aec065af8d75a638b7cf`
- Test commit: `aa2a5c52ab6f6573a2c4aec065af8d75a638b7cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 13.3 to 13.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.5 | 13.3 | 1 | 1 | [run](https://argusic.com/run/089cd609-cf0f-4e0c-82cb-eddc437ff353) |
| 2 | pass with mocks | 92 | 13 | 13.3 | 1 | 1 | [run](https://argusic.com/run/977cfd1e-f81f-4188-9abd-20224eef72f7) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go 1.27.3 not installed on the system`

Attempt 2:

- 2 min: `Go 1.27.3 was not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
