# bunqueue

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/egeominotti/bunqueue, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/bunqueue

## Pinned environment

- Project commit: `13445488ab8abc70c7787a44268f1421c41a0a35`
- Test commit: `13445488ab8abc70c7787a44268f1421c41a0a35`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 36.7 to 51.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 36.7 | 0 | 0 | [run](https://argusic.com/run/51bdc038-7ba0-4f88-ba32-3690e77c3905) |
| 2 | pass | 100 | 3 | 51.1 | 2 | 2 | [run](https://argusic.com/run/b7374eef-8cc7-4e4c-b012-94e140406751) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Bun binary not found in PATH`
- 0.1 min: `sdk/typescript/dist/ directory missing (SDK client not built)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
