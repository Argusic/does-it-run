# phantom

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ghostwright/phantom, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/phantom

## Pinned environment

- Project commit: `f8c7ab42d885936ee54abc785528000260f4acc5`
- Test commit: `f8c7ab42d885936ee54abc785528000260f4acc5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.9 to 33.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1.9 | 0 | 0 | [run](https://argusic.com/run/157e9281-d2b2-4202-ba20-c7a17bd688ae) |
| 2 | pass | 100 | 1 | 33.6 | 3 | 3 | [run](https://argusic.com/run/ac51bca0-4687-4fc6-9322-4c86152f78e3) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Bun treats 'process.env.VAR = undefined' as string "undefined" (9 chars) instead of removing the variable`
- 2 min: `Container has /.dockerenv file, causing false Docker detection in prompt-assembler test`
- 2 min: `afterEach env restore leaked undefined across test files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
