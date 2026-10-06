# MeiGen-AI-Design-MCP

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jau123/MeiGen-AI-Design-MCP, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/meigen-ai-design-mcp

## Pinned environment

- Project commit: `788d7c5f0f8b1b242e2e0ba9ba41347b2951f569`
- Test commit: `788d7c5f0f8b1b242e2e0ba9ba41347b2951f569`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 55.9 to 55.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 55.9 | 4 | 4 | [run](https://argusic.com/run/3813dc80-6186-422b-b87a-8228feee4fb3) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `mock.timers.enable() uses Node 20+ object form { apis, now } but runtime is Node 18`
- 0.1 min: `mock.timers.enable() doesn't support 'Date' in Node 18, causing Retry-After test to fail`
- 0.2 min: `Node 18 mock.timers.reset() causes cancelledByParent on global mock timers`
- `scripts/ci/release.test.mjs fails , requires pnpm and node:child_process (Node 22+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
