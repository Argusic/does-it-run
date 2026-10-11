# best-claude-hud

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GaoSSR/best-claude-hud, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/best-claude-hud

## Pinned environment

- Project commit: `0dd174e30eaa6f4a54661a9a4aadb37facdc9f7e`
- Test commit: `0dd174e30eaa6f4a54661a9a4aadb37facdc9f7e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.5 to 3.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.5 | 2 | 2 | [run](https://argusic.com/run/bc1eb873-5638-4d82-ae62-ab665982c47a) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `npm global install failed with EACCES (no root in container)`
- 8 min: `Rust toolchain not present in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
