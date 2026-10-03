# leon

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/leon-ai/leon, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/leon

## Pinned environment

- Project commit: `a8f2052fb6d9e7ffac50b115f976709afa22d390`
- Test commit: `a8f2052fb6d9e7ffac50b115f976709afa22d390`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.5 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 6.5 | 3 | 3 | [run](https://argusic.com/run/748a9b05-ef70-4d5b-ac6d-8521b248a1b8) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `System Node.js version was v18.19.1, but Leon requires Node.js >=24.0.0. pnpm refused to install.`
- 3 min: `Setup failed at setupNinja: 'spawnSync unzip ENOENT' -- unzip is not in the container.`
- `2 integration tests failed: document-reader.spec.ts - Missing managed OCR resource: PaddleOCR-v6-small-det/inference.onnx`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
