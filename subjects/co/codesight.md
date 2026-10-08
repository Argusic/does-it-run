# codesight

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Houseofmvps/codesight, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/codesight

## Pinned environment

- Project commit: `f9a43d70f0a6538c845884242894d6c0c02f0950`
- Test commit: `f9a43d70f0a6538c845884242894d6c0c02f0950`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 3.9 | 2 | 2 | [run](https://argusic.com/run/4f650245-2b1c-4c71-af20-839c0cf54233) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `import.meta.dirname is undefined on Node.js 18 (requires Node.js 21+) in tests/terraform-plugin.test.ts`
- 1.5 min: `WASI.getImportObject() not available on Node.js 18 WASI API (requires Node.js 21+)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
