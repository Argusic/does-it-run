# easy-agent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ConardLi/easy-agent, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/easy-agent

## Pinned environment

- Project commit: `893e0dd34b7b2bd4ab713804572ea97eae5a1a8b`
- Test commit: `893e0dd34b7b2bd4ab713804572ea97eae5a1a8b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 6 | 1 | 1 | [run](https://argusic.com/run/3e557cd1-8bd1-4ddb-aabf-a022be96355f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node.js v18 was installed but project requires >=22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
