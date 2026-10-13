# deja

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Giammarco-Ferranti/deja, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/deja

## Pinned environment

- Project commit: `97156840defebb476be0bbc97bbcca3b75934c66`
- Test commit: `97156840defebb476be0bbc97bbcca3b75934c66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.7 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 4.7 | 1 | 1 | [run](https://argusic.com/run/570a14a8-27e5-4870-854f-60c17ea103ae) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go: github.com/giammarcoferranti/deja@latest: git ls-remote -q https://github.com/giammarcoferranti/deja ... could not read Username for 'https://github.com': terminal prompts disabled (repo is private on GitHub)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
