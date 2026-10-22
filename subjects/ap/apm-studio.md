# apm-studio

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apm-studio/apm-studio, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/apm-studio

## Pinned environment

- Project commit: `ed94fa66081f255bd68087b4def58f5e93c18ece`
- Test commit: `ed94fa66081f255bd68087b4def58f5e93c18ece`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.6 to 1.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 1.6 | 1 | 1 | [run](https://argusic.com/run/42f95e0d-f15d-490b-b229-270d024333cd) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18.19.1 installed but project requires >=20.19.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
