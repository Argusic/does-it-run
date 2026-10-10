# gentle-shell

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Gentleman-Programming/gentle-shell, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/gentle-shell

## Pinned environment

- Project commit: `b27bd328b95e83967ffc23f62b76e77901b91130`
- Test commit: `b27bd328b95e83967ffc23f62b76e77901b91130`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 42.2 to 42.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 42.2 | 3 | 3 | [run](https://argusic.com/run/c59f7a2c-0bb8-4fea-93c2-139fe94be9b2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 is too old for pnpm 11 (needs >=22.13)`
- 1 min: `pnpm not globally installed`
- 30 min: `AbortSignal.timeout() in Node 22 emits process.exit which node:test treats as a process exit (cancelledByParent)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
