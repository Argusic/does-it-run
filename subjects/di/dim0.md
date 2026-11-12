# dim0

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vcmf/dim0, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dim0

## Pinned environment

- Project commit: `de9d9523168eedbc4edbfb9111b863a8885a3335`
- Test commit: `de9d9523168eedbc4edbfb9111b863a8885a3335`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 12.3 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 17.5 | 0 | 0 | [run](https://argusic.com/run/c7ffd9f6-973e-4f12-a7ad-0f358a31f432) |
| 2 | pass with mocks | 92 | 13 | 12.3 | 6 | 6 | [run](https://argusic.com/run/95621767-8765-4a1f-859c-8f9ec6a24989) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Python 3.13 not available in container`
- 1 min: `uv not installed`
- 1 min: `mini-app-compiler node_modules missing (sucrase)`
- 1 min: `Node 18 cannot require ES Module from @exodus/bytes`
- 2 min: `undici 8.x crashes on Node 20 (createZstdDecompress missing)`
- 1 min: `jsdom 30 uses undici with webidl.markAsUncloneable not in Node 20`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
