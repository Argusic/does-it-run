# mnemon

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mnemon-dev/mnemon, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/mnemon

## Pinned environment

- Project commit: `e9ce9945b12f879061a439d7174e014a3e93dfa7`
- Test commit: `e9ce9945b12f879061a439d7174e014a3e93dfa7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 4.6 | 2 | 2 | [run](https://argusic.com/run/820e1ec9-dc88-469d-9ee1-6f2de389636a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go compiler not found in container (no go binary)`
- 3 min: `umask 0002 causes tests to fail , project root / tmp dirs are group/other-writable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
