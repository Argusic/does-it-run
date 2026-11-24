# SkillEvaluator

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NVIDIA/SkillEvaluator, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/skillevaluator

## Pinned environment

- Project commit: `4f3a9a61676c00e988fae0400e1b8bdfbc3154dd`
- Test commit: `4f3a9a61676c00e988fae0400e1b8bdfbc3154dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 56.4 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/08b031a9-22e1-4b71-a3cc-2cc67fd09a29) |
| 2 | pass with mocks | 92 | 55 | 56.4 | 1 | 1 | [run](https://argusic.com/run/3b70f935-6dd5-4d7a-9a3e-1d560f28ccfc) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
