# chromedp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chromedp/chromedp, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/chromedp

## Pinned environment

- Project commit: `166af206b915d60dbe77ab32bb4ec74890ce077a`
- Test commit: `166af206b915d60dbe77ab32bb4ec74890ce077a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.3 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.5 | 10.3 | 1 | 1 | [run](https://argusic.com/run/894283de-7413-4724-bf30-f9e047fd4f4b) |

## What was observed on a clean machine

Attempt 1:

- `No Chrome browser or headless-shell available in container. Full test suite skipped.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
