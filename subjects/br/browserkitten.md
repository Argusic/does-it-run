# BrowserKitten

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Player-YN/BrowserKitten, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/browserkitten

## Pinned environment

- Project commit: `6ec7d9cc841189bb960621a60dd9ef031dc3a9f5`
- Test commit: `6ec7d9cc841189bb960621a60dd9ef031dc3a9f5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.7 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11.4 | 10.9 | 1 | 1 | [run](https://argusic.com/run/e346f48b-8d53-4b91-987b-1f108b204775) |
| 2 | pass | 100 | 15 | 4.7 | 1 | 1 | [run](https://argusic.com/run/186c6907-ca04-4cf5-a26e-657a18fcc099) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js 18.19.1 (default) lacks global crypto.randomUUID, Promise.withResolvers, and MockTimers object-format config required by this project. Tests fail with ESM import errors, crypto is not defined, and MockTimers API incompatibility.`

Attempt 2:

- 5 min: `System Node.js v18.19.1 cannot import ES module .js files , automatic ESM detection requires Node.js 22+`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
