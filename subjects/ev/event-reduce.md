# event-reduce

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pubkey/event-reduce, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/event-reduce

## Pinned environment

- Project commit: `d25f28df0c5ef53b44fe582790d0c8a789ab1e74`
- Test commit: `d25f28df0c5ef53b44fe582790d0c8a789ab1e74`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.9 to 1.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 1.9 | 1 | 1 | [run](https://argusic.com/run/58c75f09-7246-4eb3-8e88-507716081938) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm test failed with SyntaxError: Unexpected token 'with' from mocha 12 on system Node 18.19.1 (needs Node >=20; repo .nvmrc pins 24)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
