# bramble

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/movio/bramble, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/bramble

## Pinned environment

- Project commit: `3d878944f60a13ffc98442507aa74c6dc8c2b9fb`
- Test commit: `3d878944f60a13ffc98442507aa74c6dc8c2b9fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 7 | 3 | 3 | [run](https://argusic.com/run/86fee78c-2eeb-46ef-b0ac-e79d42644964) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Go toolchain present`
- 5 min: `gqlgen example pins fail to build on Go 1.23+ (x/tools v0.17.0 invalid array length)`
- 1 min: `gateway initial launch: listen tcp :8083: bind: address already in use (private port collision)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
