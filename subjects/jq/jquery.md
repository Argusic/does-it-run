# jquery

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jquery/jquery, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/jquery

## Pinned environment

- Project commit: `dc2b78f92c0e8939c80feb3311abdd535af0b55f`
- Test commit: `dc2b78f92c0e8939c80feb3311abdd535af0b55f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 3.4 | 2 | 2 | [run](https://argusic.com/run/5b88cba1-decd-49d3-ab1c-fbbffc67433d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `yargs-parser requires Node >= 20 (environments Node was 18)`
- 1 min: `Babel 8 plugin requires Node >= 22 for ESM loading`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
