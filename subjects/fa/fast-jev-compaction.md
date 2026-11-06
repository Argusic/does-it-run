# fast-jev-compaction

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tamaratran/fast-jev-compaction, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/fast-jev-compaction

## Pinned environment

- Project commit: `e3f262a7f4d42bd8dd32ced30d26176f7cb545b0`
- Test commit: `e3f262a7f4d42bd8dd32ced30d26176f7cb545b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 1.9 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.06 | 3.8 | 1 | 1 | [run](https://argusic.com/run/8c6b80c3-7d2f-4811-8284-cdca7a1cd5d2) |
| 2 | pass | 100 | 0.1 | 1.9 | 0 | 0 | [run](https://argusic.com/run/df0cb9bb-caee-43fe-9da2-b65c9881a22d) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
