# mozaik-network

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jigjoy-ai/mozaik-network, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mozaik-network

## Pinned environment

- Project commit: `32666f9c2b0be029a23e492e913846a1efdc1ca0`
- Test commit: `32666f9c2b0be029a23e492e913846a1efdc1ca0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.1 | 3 | 1 | 1 | [run](https://argusic.com/run/4337bf78-435b-4450-bba5-5c45e373aa6e) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node 18.19.1 is too old for @rstest/core (requires >=20)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
