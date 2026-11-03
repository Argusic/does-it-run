# colly

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gocolly/colly, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/colly

## Pinned environment

- Project commit: `cfd4fade0c702af04305b610c7744efff4edfc66`
- Test commit: `cfd4fade0c702af04305b610c7744efff4edfc66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.4 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 1.4 | 0 | 0 | [run](https://argusic.com/run/26116613-0f9d-4701-a9ed-9df35d05a2f8) |
| 2 | pass | 100 | 1 | 14.2 | 3 | 3 | [run](https://argusic.com/run/54b345f3-c09e-4acc-8ee3-459cb6bf5a39) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `go: not found in container`
- 10 min: `background mock server sometimes died after the exec command that launched it returned`
- 1 min: `message type mismatch for github.com/gocolly/colly/v2 errors-goquery ReadAll`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
