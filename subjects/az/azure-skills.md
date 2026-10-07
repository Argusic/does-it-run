# azure-skills

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/azure-skills, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/azure-skills

## Pinned environment

- Project commit: `bff93703c0b9665feee3f128143d23da0f6083c3`
- Test commit: `bff93703c0b9665feee3f128143d23da0f6083c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.9 to 10 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 10 | 1 | 1 | [run](https://argusic.com/run/8d0b7090-dea2-4e72-81bb-a173e81ddeae) |
| 2 | fail | 80 | 2 | 3.9 | 2 | 2 | [run](https://argusic.com/run/5a6e4c3b-1d9c-4579-ad6c-50031fe9c6ce) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 incompatible with Astro 7 (requires >=22.12.0)`

Attempt 2:

- 1 min: `Node.js v18.19.1 not supported by Astro v7 (requires >=22.12.0)`
- 1 min: `rolldown native binding missing: @rolldown/binding-linux-x64-gnu not found after node 18 reinstall`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
