# nod

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/n8n-io/nod, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/nod

## Pinned environment

- Project commit: `079f534d951471029bbb25965fd9a52318179d13`
- Test commit: `079f534d951471029bbb25965fd9a52318179d13`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 32 to 33.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 0.5 | 32 | 5 | 5 | [run](https://argusic.com/run/1bd08d00-87a4-4723-8b56-94c81a55a92f) |
| 2 | pass with mocks | 92 | 2.1 | 33.3 | 3 | 3 | [run](https://argusic.com/run/69faa96b-a975-48e3-b5a7-4cc3bb524d71) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node.js v18 system install -- needs >=24.21`
- `Docker not installed -- cannot start app (docker compose for postgres/workspace/browser)`
- `sandbox.test.ts: 'connected CLIs run only their sealed install' test fails (exit code 126) -- needs Docker workspace container with Linux user namespaces`
- `pi.test.ts hangs indefinitely -- needs model provider connection and workspace container`
- `browser.test.ts hangs indefinitely -- needs browser container`

Attempt 2:

- 0.2 min: `Node.js 18 was installed, project requires >=24.21.0`
- 0.2 min: `3 browser tests failed: Chrome not found`
- 0.5 min: `sandbox test failed: 'connected CLIs run only their sealed install' - sealed check rejected group-writable dir (umask 0002 caused mkdir {recursive: true} to produce 0o775 instead of 0o755)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
