# remirror

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/remirror/remirror, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/remirror

## Pinned environment

- Project commit: `61d27d389e90333adab7a42a3b6d282342793655`
- Test commit: `61d27d389e90333adab7a42a3b6d282342793655`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.2 to 13.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 13.2 | 1 | 1 | [run](https://argusic.com/run/f2fd2a2d-434e-427f-b8bb-2a3635c85091) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Rollup configs use 'import ... with { type: 'json' }' (ES2024 import attributes) unsupported by Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
