# herdr-browser

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ogulcancelik/herdr-browser, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/herdr-browser

## Pinned environment

- Project commit: `ab5c60b1e15521ff4ac4a168ccd80b5b0133edc8`
- Test commit: `ab5c60b1e15521ff4ac4a168ccd80b5b0133edc8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 32.7 to 32.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 32.7 | 2 | 2 | [run](https://argusic.com/run/65d0ce1e-0659-4bd9-834b-0d85ba74e976) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `PaneGraphicsStream.open test: timeout promise rejection not caught; server close event missed`
- 3 min: `staleChrome test: Bun.spawn with bash exec -a returns before exec completes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
