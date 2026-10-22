# PiG

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MichaelKinsy/PiG, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/pig

## Pinned environment

- Project commit: `e63c61c338e2aaf0d130513db2c2e63fe2e7dafd`
- Test commit: `e63c61c338e2aaf0d130513db2c2e63fe2e7dafd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.4 to 34.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 34 | 34.4 | 4 | 4 | [run](https://argusic.com/run/bc57a0c6-e010-4641-a844-287fe9da142b) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Node.js v18.19.1 is below the required >=22.13; npm ci printed EBADENGINE warnings and some subprocess tests hung`
- `make test-prereqs requires cargo, rustc, and tmux (not installed, no root access)`
- `internal/nativeplatform clipboards tests fail: xclip not found`
- `make upstream-mirror required --force because .upstream/v1.0.3 existed but provenance marker was stale`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
