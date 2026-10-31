# compose-action

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hoverkraft-tech/compose-action, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/compose-action

## Pinned environment

- Project commit: `4596b50939ca2354bdbed9c71f1f68a5ccbf22f9`
- Test commit: `4596b50939ca2354bdbed9c71f1f68a5ccbf22f9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 2.2 | 2 | 2 | [run](https://argusic.com/run/7de7997a-e6f8-402b-97b7-d21098a96b34) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node 18 insufficient; project requires >=24`
- 0.5 min: `Stale node_modules_bak polluted vitest discovery (23 false test failures)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
