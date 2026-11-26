# jsoncrack.com

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AykutSarac/jsoncrack.com, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/jsoncrack-com

## Pinned environment

- Project commit: `c30e379df2c35af5f7d6e81476acf329d3980598`
- Test commit: `c30e379df2c35af5f7d6e81476acf329d3980598`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.7 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 5.7 | 0 | 0 | [run](https://argusic.com/run/561e1704-ada3-4d95-94a6-afd0ca7d0e07) |
| 2 | pass | 100 | 8 | 8.3 | 2 | 2 | [run](https://argusic.com/run/fc46a7b8-56a7-40e6-9e52-a7d3758cd6db) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js 18.19.1 in container is below required >=24`
- 1 min: `pnpm not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
