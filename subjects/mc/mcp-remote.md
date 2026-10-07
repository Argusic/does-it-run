# mcp-remote

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/punkpeye/mcp-remote, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mcp-remote

## Pinned environment

- Project commit: `6a06aca546a8fd3b7beb040f39761b364893198d`
- Test commit: `6a06aca546a8fd3b7beb040f39761b364893198d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 40.4 to 40.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 40.4 | 1 | 1 | [run](https://argusic.com/run/ca3f7fa2-5c4d-42e0-95ac-2551349d8418) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `undici@7.12.0 calls String.prototype.toWellFormed() which is only available in Node.js 20+, but the container has Node.js 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
