# restic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/restic/restic, licensed BSD-2-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/restic

## Pinned environment

- Project commit: `6adedec6b48ae9ff0ffbc37bd675ccebd02c728f`
- Test commit: `6adedec6b48ae9ff0ffbc37bd675ccebd02c728f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.3 to 8.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.5 | 8.6 | 3 | 3 | [run](https://argusic.com/run/a22dae10-729a-4d39-80a3-24aaec1588a7) |
| 2 | pass | 100 | 6 | 7.3 | 3 | 3 | [run](https://argusic.com/run/0920ee75-c73f-4f29-952e-4992961dd333) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go compiler not found in container`
- 0.2 min: `python (not python3) required by TestStdinFromCommand tests`
- 0.3 min: `fusermount binary missing; mount tests cannot run`

Attempt 2:

- 1 min: `Go compiler not found in container`
- 1 min: `python not found in PATH`
- 1 min: `fusermount not found for FUSE mount tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
