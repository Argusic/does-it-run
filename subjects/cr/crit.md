# crit

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tomasz-tomczyk/crit, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/crit

## Pinned environment

- Project commit: `2f9a883d138cf5d0dafd1eec70cf6c98893e3f12`
- Test commit: `2f9a883d138cf5d0dafd1eec70cf6c98893e3f12`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8 to 41.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 8 | 0 | 0 | [run](https://argusic.com/run/25a8bdd9-a4c5-4358-918d-f1494e41cca5) |
| 2 | pass | 93.33 | 41 | 41.9 | 3 | 2 | [run](https://argusic.com/run/b8e67c13-1fd1-456b-8330-01738b68b221) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go not found in container (required go1.26.8, system had none)`
- 2 min: `JS test: missing normalizeCommentMarkdown stub in mock (window.crit.commentHtml.normalizeCommentMarkdown is not a function)`
- `Pre-existing flaky Go test TestNewSessionFromGitLazyThreshold (expected 120 files, got 121) , global defaultBranchOverride state leaks between tests in the suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
