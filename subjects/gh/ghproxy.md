# ghproxy

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/WJQSERVER-STUDIO/ghproxy, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ghproxy

## Pinned environment

- Project commit: `4c555ed50c5574163dd33c945a2d7092faa3932b`
- Test commit: `4c555ed50c5574163dd33c945a2d7092faa3932b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.6 | 3 | 3 | [run](https://argusic.com/run/bbdb556c-c38c-4b5f-8792-e8940520bbc5) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed in container`
- 1 min: `go build failed: pages/* directory missing for embed directive`
- 1 min: `TestExtractParts_Compatibility/Empty_path_segments failed: extractParts returned '/' instead of '' for empty first path segment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
