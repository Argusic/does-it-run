# ccpm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/automazeio/ccpm, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/ccpm

## Pinned environment

- Project commit: `7d7e4623bc6d4c0c9ba66ca6bfecd7e5261dc697`
- Test commit: `7d7e4623bc6d4c0c9ba66ca6bfecd7e5261dc697`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.7 | 4.3 | 2 | 2 | [run](https://argusic.com/run/2e8735a8-ae55-41ef-b565-3eb96bb5d984) |

## What was observed on a clean machine

Attempt 1:

- 1.2 min: `GitHub CLI (gh) not in PATH at start; sudo not available for apt-get install`
- `GitHub authentication unavailable non-interactively in sandbox`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
