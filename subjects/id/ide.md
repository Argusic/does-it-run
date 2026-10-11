# ide

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/judge0/ide, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ide

## Pinned environment

- Project commit: `4e0e7a4bfe3217e07f4a88967bc7d4837b8e38c0`
- Test commit: `4e0e7a4bfe3217e07f4a88967bc7d4837b8e38c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.4 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6.4 | 2 | 2 | [run](https://argusic.com/run/86e671b3-63ec-4d34-b63e-346f05c9b622) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npx puppeteer browsers install chrome failed with SyntaxError: Invalid regular expression flags (Node v18 lacks /v regex support required by puppeteer's cliui/string-width deps)`
- 1 min: `python3 -m http.server in background terminated shortly after launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
