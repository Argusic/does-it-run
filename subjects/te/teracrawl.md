# teracrawl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/BrowserCash/teracrawl, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/teracrawl

## Pinned environment

- Project commit: `eae1b0e4911928e398b583add50c2e2d4406a3c0`
- Test commit: `eae1b0e4911928e398b583add50c2e2d4406a3c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.3 to 15.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 15.3 | 2 | 2 | [run](https://argusic.com/run/1941d381-b088-4538-aaa0-4587e3596bee) |

## What was observed on a clean machine

Attempt 1:

- `npm install warns about unsupported Node.js v18 for find-my-way@9.3.0 (requires >=20). Node 18.19.1 is below the SDK's preferred 20+, but all packages install and the app runs fine.`
- `npx playwright install chromium fails because the npx version requires Node >=20, but the bundled playwright-core v1.57 ships its own CLI which works.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
