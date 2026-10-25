# agent-fetch

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/teng-lin/agent-fetch, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agent-fetch

## Pinned environment

- Project commit: `7632d139d5df1d8a19d23fdb2f5ae2619f151be4`
- Test commit: `7632d139d5df1d8a19d23fdb2f5ae2619f151be4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.3 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 6.8 | 0 | 0 | [run](https://argusic.com/run/4759164b-c0c4-434d-ab1b-7ec5c4d5589b) |
| 2 | pass | 100 | 3.5 | 6.3 | 1 | 1 | [run](https://argusic.com/run/4dfafb43-5182-4314-aacc-f3a2d904792d) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Node.js v18 in container incompatible with project engine requirement (>=20). npm install warned EBADENGINE for vitest; 13 test files failed with ReferenceError (File, DOMMatrix not defined).`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
