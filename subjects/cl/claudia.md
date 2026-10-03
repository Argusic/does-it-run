# claudia

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/claudiajs/claudia, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/claudia

## Pinned environment

- Project commit: `9d68ed4c62e123279b14b31b7dfbc34710f40689`
- Test commit: `9d68ed4c62e123279b14b31b7dfbc34710f40689`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 41.2 to 41.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0 | 41.2 | 3 | 3 | [run](https://argusic.com/run/67ae2181-d3bb-4114-8fec-f70422070994) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `fs.mkdtempSync(os.tmpdir()) in spec/fs-promise-spec.js fails with EACCES on Node 18 because the template lacks 'XXXXXX' suffix`
- 10 min: `unzip binary is not installed in the container, causing zipdir spec to fail with ENOENT`
- 5 min: `npm 9 generates lockfileVersion 3 (packages key) but collect-files-spec expected lockfileVersion 1 (dependencies key)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
