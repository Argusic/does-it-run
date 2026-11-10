# dnote

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dnote/dnote, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/dnote

## Pinned environment

- Project commit: `a07a751f9827ff0875233e05317b90de7b29fd55`
- Test commit: `a07a751f9827ff0875233e05317b90de7b29fd55`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.1 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 12.2 | 0 | 0 | [run](https://argusic.com/run/b73c3bf7-d62b-4867-a95f-5e5c3d105a91) |
| 2 | pass | 100 | 5 | 5.1 | 1 | 1 | [run](https://argusic.com/run/e126bb8d-a363-4d1e-9373-05d3044b31c5) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `FTS5 module not loaded - go-sqlite3 needs -tags fts5 build tag`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
