# werf

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/werf/werf, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/werf

## Pinned environment

- Project commit: `e6c37bd15ea829ea619929bd9ec4e35044955e00`
- Test commit: `e6c37bd15ea829ea619929bd9ec4e35044955e00`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 15.8 to 27.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 27.9 | 6 | 6 | [run](https://argusic.com/run/7d9aec18-62a8-45fd-8a11-552db09d540a) |
| 2 | pass with mocks | 92 | 12 | 15.8 | 5 | 5 | [run](https://argusic.com/run/e34aed82-1c5b-4b35-8d20-7c306d9c5d5b) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain not installed`
- 2 min: `Task runner not installed`
- 5 min: `CGO compilation failed: missing btrfs/version.h header (libbtrfs-dev not installed, no root)`
- `Remote taskfiles not enabled`
- 2 min: `Ginkgo CLI not installed (needed for test runner)`
- `git_repo unit tests failed: git user identity not configured`

Attempt 2:

- 1 min: `Go 1.26 not installed`
- 1 min: `Task runner not found`
- 5 min: `Default build uses CGo (needs libbtrfs-dev) which cannot be installed without root`
- 1 min: `Ginkgo test runner not installed`
- `git_repo tests fail because no git user config`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
