# taste-skill

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Leonxlnx/taste-skill, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/taste-skill

## Pinned environment

- Project commit: `a60a36dc2bb3bb77ccf17f2f62041f5ca8a458b9`
- Test commit: `a60a36dc2bb3bb77ccf17f2f62041f5ca8a458b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.9 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 4.5 | 1 | 1 | [run](https://argusic.com/run/e9650d1e-a22d-49a7-b012-80e24d47f919) |
| 2 | pass | 100 | 1.5 | 2.9 | 2 | 2 | [run](https://argusic.com/run/539249d8-f70f-4314-8e30-69b2ff6f7b4e) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `inspect.mjs aborts with extracted Chrome: SUID chrome-sandbox not configured', so the inspector exited. The CDP client spawns Chrome without --no-sandbox.`

Attempt 2:

- `Node 18.19.1 is installed but inspect.mjs (browser inspector/screenshots) requires Node 22+`
- `No Chrome/Chromium binary is available, so inspect.mjs and assets.mjs cannot drive a real browser`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
