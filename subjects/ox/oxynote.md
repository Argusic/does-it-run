# oxynote

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oxynote/oxynote, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/oxynote

## Pinned environment

- Project commit: `a7dc0c8440b85ad990ef64801f1f48991ba30cd5`
- Test commit: `a7dc0c8440b85ad990ef64801f1f48991ba30cd5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 46.2 to 46.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 46.2 | 5 | 5 | [run](https://argusic.com/run/0d16b431-ab40-436f-87b7-499193e61baa) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.0 toolchain not available - had to download via go toolchain auto-resolution`
- 1 min: `Node.js 18 installed but needs 24+ - had to download Node 24 tarball`
- 1 min: `pnpm not installed - had to set up via corepack`
- `Docker not available - 4 Go test packages fail (db, datasource/processor, mariademo, pgdemo)`
- `Web test suite (vitest) crashes with SIGSEGV or hangs when running all 289 files together`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
