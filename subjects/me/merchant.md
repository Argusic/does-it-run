# merchant

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ygwyg/merchant, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/merchant

## Pinned environment

- Project commit: `1b42cbb7f5c8efaa943f68153cf6922ef6d1903b`
- Test commit: `1b42cbb7f5c8efaa943f68153cf6922ef6d1903b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 6.6 | 1 | 1 | [run](https://argusic.com/run/50b26c46-72f7-412b-945d-15c6c7e6cc61) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18 too old for wrangler (requires >=20)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
