# wtp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/satococoa/wtp, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/wtp

## Pinned environment

- Project commit: `842920d489e96c67798c6b2689f48dc885e42094`
- Test commit: `842920d489e96c67798c6b2689f48dc885e42094`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.7 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 5.4 | 2 | 2 | [run](https://argusic.com/run/29995106-e90d-4f47-825c-dca6b52b3fe3) |
| 2 | pass | 100 | 2 | 1.7 | 1 | 1 | [run](https://argusic.com/run/2951426d-43e4-41b4-b8f7-b2b63347b57d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go toolchain missing in container (go: not found)`
- 5 min: `Default .wtp.yml hook runs 'wtp list', which exits 127 when wtp is not on PATH`

Attempt 2:

- 1 min: `Go 1.24.4 not found in the container , neither in PATH nor as a system package`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
