# prime-agent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PrimeIntellect-ai/prime-agent, licensed NOASSERTION, written in Rust.

Evidence and recordings: https://argusic.com/subject/prime-agent

## Pinned environment

- Project commit: `e260085dd8f742e0def3d871860c9a888b114851`
- Test commit: `e260085dd8f742e0def3d871860c9a888b114851`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 55.4 to 55.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 55.4 | 5 | 5 | [run](https://argusic.com/run/94b14b72-2fb5-4d17-ae75-0efc22cb5481) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 too old (requires >=22.8.0)`
- 1 min: `uv not installed - Python kernel bootstrap failed`
- 1 min: `catalog assets not generated (models.bundled.json missing)`
- 1 min: `packages/ai/test/stream.test.ts hangs when run with other ai tests due to parallel provider test contention`
- `coding-agent test suite hangs in large parallel batches (parallel test file contention from daemon socket/process tests)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
