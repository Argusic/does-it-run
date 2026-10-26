# bim

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/toaruos/bim, licensed ISC, written in C.

Evidence and recordings: https://argusic.com/subject/bim

## Pinned environment

- Project commit: `8ece591fbec5e8445bed9cfe44bc2f6a5b5506c8`
- Test commit: `8ece591fbec5e8445bed9cfe44bc2f6a5b5506c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 5.4 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 8.7 | 0 | 0 | [run](https://argusic.com/run/c219fbde-475c-43d8-bcec-77fc9630f0ed) |
| 2 | pass | 100 | 8 | 5.4 | 1 | 1 | [run](https://argusic.com/run/1424efde-be82-4c53-8063-b801a864b24b) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Kuroko make failed on first attempt because shared-library modules (.so) were not built yet, so generated codec scripts (gen_sbencs/gen_dbdata) failed importing 'fileio'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
