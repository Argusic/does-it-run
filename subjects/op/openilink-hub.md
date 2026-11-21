# openilink-hub

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/openilink/openilink-hub, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/openilink-hub

## Pinned environment

- Project commit: `1df2ebebb69a5099e94b3f254f069aca5e272eed`
- Test commit: `1df2ebebb69a5099e94b3f254f069aca5e272eed`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.4 to 14.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24.5 | 7.4 | 4 | 4 | [run](https://argusic.com/run/1f735d7b-6aed-46cc-af2f-79844fe2095e) |
| 2 | pass | 100 | 13 | 14.1 | 3 | 3 | [run](https://argusic.com/run/c4a0ccc9-00d8-4491-9eb0-862430471999) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go compiler not found in container`
- 2 min: `Node.js v18.19.1 too old for vite-plus build`
- 0.5 min: `vite-plus native binding @voidzero-dev/vite-plus-linux-x64-gnu not installed`
- 1 min: `Go embed failed: internal/web/embed.go expected all:dist but dist/ did not exist`

Attempt 2:

- 3 min: `Go binary not found in container`
- 2 min: `Node.js 18 too old for vite-plus native binding (requires Node >=22.12)`
- 1 min: `vite-plus Linux x64 native binding optional dependency not installed by pnpm`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
