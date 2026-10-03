# playwright-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/playwright-mcp, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/playwright-mcp

## Pinned environment

- Project commit: `4c1fb03bad3bae379b0ae0e3d81d2660de56bd91`
- Test commit: `4c1fb03bad3bae379b0ae0e3d81d2660de56bd91`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 6.1 to 20.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 20.7 | 20.9 | 5 | 5 | [run](https://argusic.com/run/40b2153d-7858-4452-9128-4063f79e85e2) |
| 2 | pass | 100 | 2 | 6.3 | 2 | 2 | [run](https://argusic.com/run/df3dd1b5-6811-439a-8152-daefcb9b041d) |
| 3 | pass | 100 | 1 | 6.1 | 2 | 2 | [run](https://argusic.com/run/518ea071-f911-4833-9353-e9705e6a1ef2) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18 (system) is too old; package requires >=20`
- 2 min: `Chromium browsers not installed`
- 1 min: `playwright.config.ts defaulted to mcpBrowser='chrome' but only chromium (Playwright bundled) is available, not system Google Chrome`
- 12 min: `Missing system libraries (libglib, libnss, libx11, etc.) required by Playwright's Chromium`
- 1 min: `core.spec.ts test expected [ref=e1] in snapshot but newer Playwright accessibility tree format omits ref labels`

Attempt 2:

- 1 min: `Node.js v18.19.1 does not meet Playwright's requirement of Node >=20`
- 0.5 min: `Test failures: 'Chromium distribution chrome is not found at /opt/google/chrome/chrome' , default mcpBrowser was 'chrome' (system Chrome)`

Attempt 3:

- 0.5 min: `Node.js 18 lacks required version >=20 for Playwright dependencies`
- 0.5 min: `Test mcpBrowser defaulted to 'chrome' (Google Chrome) which was not installed; only open-source Chromium was available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
