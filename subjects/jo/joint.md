# joint

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/clientIO/joint, licensed MPL-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/joint

## Pinned environment

- Project commit: `881e49d8f5e4aea080875c653997260acea67870`
- Test commit: `881e49d8f5e4aea080875c653997260acea67870`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.8 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 7 | 8.8 | 2 | 0 | [run](https://argusic.com/run/cacb4760-64b4-424f-b4c5-96b190b0b4dd) |

## What was observed on a clean machine

Attempt 1:

- `Core test suite: util.breakText international character test fails due to Chrome font rendering differences in this container`
- `Node.js v18 cannot build @joint/layout-directed-graph due to 'import ... with' ESM syntax (requires Node 20+). Core library is unaffected.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
