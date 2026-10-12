# figwright

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/awdr74100/figwright, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/figwright

## Pinned environment

- Project commit: `832b5a358bf4e32bdbc80400012cac9f52e73adf`
- Test commit: `832b5a358bf4e32bdbc80400012cac9f52e73adf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 5.6 | 1 | 1 | [run](https://argusic.com/run/e256a832-8793-472f-9746-00b74ae61b3b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `container Node is v18.19.1 but repo requires ^24.11.0 || >=26.0.0, and pnpm is not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
