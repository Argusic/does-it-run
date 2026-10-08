# vibeyard

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elirantutia/vibeyard, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/vibeyard

## Pinned environment

- Project commit: `19bc19f0fac04f11e7d9e5cf68ed75ac7d291566`
- Test commit: `19bc19f0fac04f11e7d9e5cf68ed75ac7d291566`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5 | 3 | 3 | [run](https://argusic.com/run/da1f8cd5-b7f4-47c0-b6dd-6edd61b99e8d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm install with Node 18 failed on native deps (node-pty rebuild)`
- `Node 18 too old for vitest 4.x (requires ^20||^22||>=24)`
- `Electron requires --no-sandbox flag in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
