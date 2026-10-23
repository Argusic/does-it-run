# mulmoclaude

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/receptron/mulmoclaude, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mulmoclaude

## Pinned environment

- Project commit: `d7dadff432a4558b907b23c92e320bc5a4d1b277`
- Test commit: `d7dadff432a4558b907b23c92e320bc5a4d1b277`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 9.3 to 44.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 44.4 | 0 | 0 | [run](https://argusic.com/run/c8a0231c-d842-476b-a0e5-b26d7994bb5b) |
| 2 | pass | 100 | 9 | 9.3 | 4 | 4 | [run](https://argusic.com/run/b3e529f1-1592-4907-8461-989c5fe00f29) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18.19.1 is too old (project requires >=22.19)`
- 1 min: `yarn not found on system PATH`
- 2 min: `Workspace package dist/ missing (ERR_MODULE_NOT_FOUND @mulmoclaude/accounting-plugin)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
