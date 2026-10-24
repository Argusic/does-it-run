# shopnex

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/shopnex-ai/shopnex, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/shopnex

## Pinned environment

- Project commit: `4f791764dec7824dcc422d34bab1ff37ff35bd76`
- Test commit: `4f791764dec7824dcc422d34bab1ff37ff35bd76`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 66.2 to 66.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 66.2 | 5 | 5 | [run](https://argusic.com/run/caf8a554-a23d-4c6f-ac65-b34cebc330ff) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pnpm not found in PATH`
- 1 min: `Build scripts (esbuild, @swc/core, etc.) not executed`
- 5 min: `ReferenceError: File is not defined (Node 18 lacks File global)`
- 10 min: `Build killed by OOM during static page generation (8GB cgroup limit)`
- 2 min: `The build:generate step fails when chained with && after compile in the same script`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
