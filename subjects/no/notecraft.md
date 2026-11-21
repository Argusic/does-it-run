# notecraft

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AlienTechSoftware/notecraft, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/notecraft

## Pinned environment

- Project commit: `72c99d9f97a2106e006ace7bee1f48e9c268190b`
- Test commit: `72c99d9f97a2106e006ace7bee1f48e9c268190b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 30.4 to 41.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 30.4 | 0 | 0 | [run](https://argusic.com/run/9f10503b-c5ab-401c-9c2a-f5c0e5b9edba) |
| 2 | pass | 100 | 14 | 41.9 | 0 | 0 | [run](https://argusic.com/run/18db9e7b-6b59-43c4-bf6d-bee2a4d99ee7) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
