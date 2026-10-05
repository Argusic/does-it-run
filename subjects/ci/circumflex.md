# circumflex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bensadeh/circumflex, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/circumflex

## Pinned environment

- Project commit: `ce26e6d5535452959bc87eb5f77d2046280fac0f`
- Test commit: `ce26e6d5535452959bc87eb5f77d2046280fac0f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6 | 1 | 1 | [run](https://argusic.com/run/30ee5cb6-d654-4597-8135-1dc76e548c92) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go compiler not installed in container; the deb package's 'go' binary tried to auto-download go1.27 toolchain but failed (download URL returned 404)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
