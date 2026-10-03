# MemOS

**Verdict: runs with mocks.** Argusic Score 98 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MemTensor/MemOS, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/memos

## Pinned environment

- Project commit: `a7367d07e55db61099f7b4e2c1108bc5831a24f3`
- Test commits: `02caf98c7bd038bd03dd7984cdfe51ec2652491e`, `a7367d07e55db61099f7b4e2c1108bc5831a24f3`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 4; wall time 5.1 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 24 | 24.8 | 3 | 3 | [run](https://argusic.com/run/2a836002-ca18-4c2b-9e54-21b4844a77cb) |
| 1 | pass with mocks | 92 | 8 | 5.1 | 2 | 2 | [run](https://argusic.com/run/a92789ba-3e9a-4bac-9225-2618fcffa7e5) |
| 2 | pass | 100 | 10.5 | 12.6 | 5 | 5 | [run](https://argusic.com/run/712432a9-1eeb-434c-a106-60c14c9e753e) |
| 3 | pass | 100 | 3 | 23.9 | 4 | 4 | [run](https://argusic.com/run/e4f1037e-f2e8-46b5-9276-e8dea43b7c6f) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Go runtime conflict: Go 1.27.1 tarball extracted over an earlier Go 1.22.5 extract, causing redeclaration errors in runtime/mbitmap_noallocheaders.go vs runtime/mbitmap.go`
- 2 min: `Test failure: TestDetectAttachmentMimeType/unknown_extension_falls_back_to_content_sniffing - system MIME database maps .xyz to chemical/x-xyz, so Go's mime.TypeByExtension returns a match before hitting the content-sniffing fallback`
- 2 min: `Node.js 18 is below minimum requirement (>=24)`

Attempt 1:

- 5 min: `API server (uvicorn) cannot start , init_server() eagerly connects to Qdrant on localhost:6333 which isn't running`
- `memos export_openapi fails , same eager init_server() call at module import`

Attempt 2:

- 1 min: `Go (1.27.0) not pre-installed`
- 1 min: `Node.js v24 not available (had v18)`
- 0.5 min: `pnpm not pre-installed`
- `Docker not available , store integration tests skipped (TestContainers requires Docker for MySQL/PostgreSQL)`
- `24 pre-existing frontend test failures (CSS class assertion mismatches in 2 test files)`

Attempt 3:

- 0.5 min: `Go not found in PATH`
- 0.5 min: `Node.js 18.19.1 too old for Vite 8, pnpm could not install globally`
- 0.3 min: `Server returned 'No embeddable frontend found' at /`
- 0.2 min: `pnpm not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
