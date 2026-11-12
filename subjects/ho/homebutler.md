# homebutler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Higangssh/homebutler, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/homebutler

## Pinned environment

- Project commit: `546ff83e47e8f813925761a1cb189977634bf934`
- Test commit: `546ff83e47e8f813925761a1cb189977634bf934`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12 | 2 | 2 | [run](https://argusic.com/run/0fdfec80-5c7f-4907-a127-d9a86686f896) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Test suite relies on system.InContainer() which detected /.dockerenv marker, causing tests expecting external-container behavior to fail (3 server tests, 1 mcp test)`
- 3 min: `Web frontend build fails: Vite 8 requires Node.js >=20.19.0 but system has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
