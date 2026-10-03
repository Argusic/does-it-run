# opensrc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vercel-labs/opensrc, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/opensrc

## Pinned environment

- Project commit: `f96078ac0a7ce3fb7d058d73ce65ff4b6606d765`
- Test commit: `f96078ac0a7ce3fb7d058d73ce65ff4b6606d765`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.9 to 12.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 12.9 | 3 | 3 | [run](https://argusic.com/run/728c2a9f-3f02-4924-bf3f-102af887fc7f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18 present but project requires >=24; pnpm not available`
- 1 min: `Rust toolchain missing: 'cargo test' failed in opensrc#test`
- `GitHub API rate limit exceeded when fetching vercel/next.js`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
