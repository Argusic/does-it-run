# delegate-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amElnagdy/delegate-skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/delegate-skills

## Pinned environment

- Project commit: `6826b363085dcc80875372315fe7d208c4bf733f`
- Test commit: `6826b363085dcc80875372315fe7d208c4bf733f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 29.9 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/3ef87235-208f-4348-804f-debdb685eda8) |
| 2 | pass | 100 | 12 | 29.9 | 2 | 2 | [run](https://argusic.com/run/2613a79b-5096-4071-83e2-dc73dbde8986) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `The npx skills CLI command requires Node >=22.20.0 but the container ships Node 18.19.1`
- 1 min: `POSIX fake-CLI shim in test/harness/install-shim.mjs used external dirname command which fails when PATH is stripped in grok Git-unavailable test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
