# Codync

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leepokai/Codync, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/codync

## Pinned environment

- Project commit: `013ec4c4023f58c8061293f09bb9922cbe57725c`
- Test commit: `013ec4c4023f58c8061293f09bb9922cbe57725c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.2 to 22.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 22 | 22.2 | 4 | 3 | [run](https://argusic.com/run/b6ba3f83-2eee-4c68-87c3-a9843247ee73) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js 18 lacks --experimental-strip-types and registerHooks needed by desktop & cloud tests`
- `7 desktop tests (ssh-command.test.ts) fail: /usr/bin/ssh not installed and openssh-client cannot be installed without root`
- 2 min: `Cloud tests failed with rolldown WASM binding from stale Node 18 node_modules`
- `E2E tests failed with host didn't start due to port contention in parallel test runner`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
