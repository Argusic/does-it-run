# APIPark

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/APIParkLab/APIPark, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/apipark

## Pinned environment

- Project commit: `b6b58db20bfb8903a5bd623a0272dda16388dbb5`
- Test commit: `b6b58db20bfb8903a5bd623a0272dda16388dbb5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 56.8 to 56.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14.5 | 56.8 | 6 | 6 | [run](https://argusic.com/run/4d97bdd7-58f8-409d-b65d-777a7c789d62) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go not found in container`
- 1 min: `Frontend dist/ directory missing (required by go:embed directive)`
- 2 min: `libaio.so.1 not found - MySQL 8.0.37 required library missing`
- 5 min: `MySQL 8.0 gets OOM-killed on 2GB RAM (requires ~400MB RSS)`
- `log-driver/loki/loki_test.go: NewDriver returns 3 values but test expects 2`
- `ai-provider/local/executor_test.go: TestPullModel times out after 60s (starts HTTP server)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
