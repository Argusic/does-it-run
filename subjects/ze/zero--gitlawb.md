# zero

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Gitlawb/zero, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/cd553535-ed67-4bc1-8e87-50b55f4694f9

## Pinned environment

- Project commit: `99721c762f37cd43ac511007a5f51d1846df959e`
- Test commit: `99721c762f37cd43ac511007a5f51d1846df959e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.9 to 9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 8.9 | 0 | 0 | [run](https://argusic.com/run/cd553535-ed67-4bc1-8e87-50b55f4694f9) |
| 2 | pass | 100 | 7 | 9 | 3 | 3 | [run](https://argusic.com/run/3b9feb1b-5d9d-47f3-9e5d-a0f055b62b29) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go 1.26.6+ not found in PATH; required to build from source`
- `GOPATH and GOROOT were the same directory after extraction, causing Go warning`
- 1 min: `npm global install (npm install -g @gitlawb/zero) failed with EACCES on /usr/local/lib/node_modules`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
