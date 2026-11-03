# prime-agent

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PrimeIntellect-ai/prime-agent, licensed NOASSERTION, written in Rust.

Evidence and recordings: https://argusic.com/subject/prime-agent

## Pinned environment

- Project commit: `e260085dd8f742e0def3d871860c9a888b114851`
- Test commit: `e260085dd8f742e0def3d871860c9a888b114851`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 55.4 to 64.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 55.4 | 5 | 5 | [run](https://argusic.com/run/94b14b72-2fb5-4d17-ae75-0efc22cb5481) |
| 2 | pass | 100 | 18 | 64.9 | 7 | 7 | [run](https://argusic.com/run/4553a224-a4a5-45d3-b5ff-568dc2bd42fd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js 18.19.1 too old (requires >=22.8.0)`
- 1 min: `uv not installed - Python kernel bootstrap failed`
- 1 min: `catalog assets not generated (models.bundled.json missing)`
- 1 min: `packages/ai/test/stream.test.ts hangs when run with other ai tests due to parallel provider test contention`
- `coding-agent test suite hangs in large parallel batches (parallel test file contention from daemon socket/process tests)`

Attempt 2:

- 4 min: `System Node was v18.19.1 but the project requires >=22.8.0`
- 25 min: `Extension loader aliased pi packages to unbuilt dist/ paths, breaking extension import and 10 tests`
- 30 min: `lsof missing on host (container has no ss either), breaking a shutdown --force regression`
- 6 min: `uv missing, required for the Python kernel bootstrap`
- 6 min: `No prime-agent-catalog checkout; tests need generated bundled assets`
- 5 min: `npm run check fails at check:test-policy with pre-existing prime-agent-runtime Python test violations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
