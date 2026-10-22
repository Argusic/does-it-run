# whirl

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/whirlchat/whirl, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/whirl

## Pinned environment

- Project commit: `1fb4754706c36ab4fe258720b770dbfa90addada`
- Test commit: `1fb4754706c36ab4fe258720b770dbfa90addada`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.3 to 23.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 6 | 23.3 | 6 | 6 | [run](https://argusic.com/run/c4fff68a-1904-4fa2-9ba7-f7175634c968) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `bun not found`
- 1 min: `unzip not found for bun installer`
- 1 min: `node 18 too old for next.js 16 (requires >=20.9.0)`
- `vitest's rolldown dep requires node:util.styleText (node 21+)`
- 1 min: `build failed: missing NEXT_PUBLIC_CONVEX_URL env var`
- 2 min: `clerk middleware rejects mock keys at server-side auth boundary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
