# reelmimic

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/edenfunf/reelmimic, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/reelmimic

## Pinned environment

- Project commit: `782a3ba3cfa455663127348dbfcbcfafada05d52`
- Test commit: `782a3ba3cfa455663127348dbfcbcfafada05d52`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 6.9 to 11.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 6.9 | 3 | 3 | [run](https://argusic.com/run/b25b40f8-d23d-48c3-956d-d5da7bc5a2b3) |
| 2 | pass | 100 | 18 | 11.2 | 5 | 5 | [run](https://argusic.com/run/4a904d2b-6fa4-4869-8e6c-21ee761f7950) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18.19.1 is below the required v22.18+`
- 0.5 min: `Python externally-managed-environment blocks system pip install`
- 1 min: `Chrome/Chromium not found for headless rendering`

Attempt 2:

- 3 min: `Node v18.19.1 too old (needs 22.18+)`
- 2 min: `Python pip blocked by externally-managed-environment (PEP 668)`
- 3 min: `unzip missing for puppeteer Chrome download`
- 5 min: `Chrome/Chromium not found in system`
- `First test run showed 1 flaky failure (test order pollution)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
