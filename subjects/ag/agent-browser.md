# agent-browser

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/agent-browser, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/agent-browser

## Pinned environment

- Project commit: `5ee8691339a5a002e4d7454eec95250253bc7419`
- Test commit: `5ee8691339a5a002e4d7454eec95250253bc7419`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.6 to 18.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 18.6 | 3 | 3 | [run](https://argusic.com/run/5084027b-e339-48b7-8129-f7b2ed9cef9a) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 too old (requires 24+), pnpm not installed, Rust not installed, npm --prefix needed due to EACCES in /usr/local`
- 1 min: `e2e tests: e2e_material_checkbox_check_uncheck stack overflow under concurrent test runner`
- `e2e tests: 2 Obscura E2E tests fail , OBSCURA_BIN env var not set (expected, documented behavior)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
