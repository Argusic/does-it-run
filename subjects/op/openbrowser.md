# openbrowser

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ntegrals/openbrowser, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/openbrowser

## Pinned environment

- Project commit: `067fc45d649baa961750da8e2f4a75d87c5c75c8`
- Test commit: `067fc45d649baa961750da8e2f4a75d87c5c75c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.4 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 7.7 | 2 | 2 | [run](https://argusic.com/run/1857523d-abad-41b5-92bd-ebe54ff14262) |
| 2 | pass | 100 | 6 | 6.4 | 2 | 2 | [run](https://argusic.com/run/e5bc5004-b37c-48b8-91b4-af63afd5b3fe) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Bun not available in container; npm install -g bun failed (EACCES, can't write to /usr/local/lib)`
- 2 min: `Playwright browser not found at /home/runner/.cache/ms-playwright/chromium_headless_shell-1208`

Attempt 2:

- 2 min: `bun not available in container`
- 1 min: `Playwright browsers not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
