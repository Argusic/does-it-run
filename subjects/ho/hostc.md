# hostc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/akazwz/hostc, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hostc

## Pinned environment

- Project commit: `8a840dac9220662a51c57eda1d21a9f221caf6fa`
- Test commit: `8a840dac9220662a51c57eda1d21a9f221caf6fa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.5 to 7.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.2 | 7.5 | 2 | 2 | [run](https://argusic.com/run/e6737d36-3a88-4051-9b4a-d9ab9b6ea589) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js v18.19.1 is too old; project requires >=22.22`
- 1.5 min: `pnpm not found in PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
