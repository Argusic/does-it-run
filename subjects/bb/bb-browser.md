# bb-browser

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/epiral/bb-browser, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/bb-browser

## Pinned environment

- Project commit: `7975dc74b3f637d54906228e52f2ba9454874105`
- Test commit: `7975dc74b3f637d54906228e52f2ba9454874105`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.9 to 21.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 21.9 | 3 | 3 | [run](https://argusic.com/run/c811c7ea-44af-497d-9464-4a3c04150f0e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18 lacks import.meta.dirname (added in Node 20) - CLI daemon-startup tests crash`
- 2 min: `unzip not installed in container - Chrome auto-download fails to extract`
- 2 min: `Chrome 149 crashpad_handler segfault - Chrome fails to start (Permission denied on spawn)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
