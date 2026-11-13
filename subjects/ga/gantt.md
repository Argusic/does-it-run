# gantt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DHTMLX/gantt, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/gantt

## Pinned environment

- Project commit: `67d4425db50009705fbe41538d75c8f5f5ac9276`
- Test commit: `67d4425db50009705fbe41538d75c8f5f5ac9276`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.25 | 6.1 | 1 | 1 | [run](https://argusic.com/run/172035cf-1e48-4cad-81a6-51626ca2742b) |
| 2 | pass | 100 | 1 | 3.1 | 1 | 1 | [run](https://argusic.com/run/1c38a6dc-8d09-4e5a-b4af-1ab3cc4a5e4f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm run test failed: Chrome requires --no-sandbox in this container (sandbox disabled by distro policy)`

Attempt 2:

- 1 min: `Puppeteer Chrome sandbox crash: container lacks user namespace support, Chrome fails to launch without --no-sandbox`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
