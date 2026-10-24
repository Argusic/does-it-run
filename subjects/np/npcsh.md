# npcsh

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NPC-Worldwide/npcsh, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/npcsh

## Pinned environment

- Project commit: `e8d3cdd697d4bd10f8d2840ae7ee899d8a732fe8`
- Test commit: `e8d3cdd697d4bd10f8d2840ae7ee899d8a732fe8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 16.6 | 3 | 3 | [run](https://argusic.com/run/7fcbb7e4-dd98-4757-a745-29e31de0cf75) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing Rust toolchain (no cargo/rustc)`
- 2 min: `npcpy backend listens on port 5337 but npcsh expects 5237`
- 2 min: `Database migration fails because conversation_history table doesn't exist yet`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
