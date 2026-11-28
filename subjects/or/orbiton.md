# orbiton

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xyproto/orbiton, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/orbiton

## Pinned environment

- Project commit: `5adb97c4e577b328a04b039f33d495ea28cb70c6`
- Test commit: `5adb97c4e577b328a04b039f33d495ea28cb70c6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 6.5 | 3 | 3 | [run](https://argusic.com/run/0201c027-d129-4fee-8839-ea005653611f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container`
- 5 min: `Syntax highlighting test expectations mismatched the vendored library output values`
- 2 min: `Man page highlighting tests failed due to NO_COLOR=1 env var suppressing color output`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
