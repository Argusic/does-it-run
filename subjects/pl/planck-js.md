# planck.js

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/piqnt/planck.js, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/planck-js

## Pinned environment

- Project commit: `93dd64df0fd2e5388551b159bebc6306e7af580a`
- Test commit: `93dd64df0fd2e5388551b159bebc6306e7af580a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.4 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 4.2 | 0 | 0 | [run](https://argusic.com/run/c8332695-7395-4802-a585-95e45ebb3366) |
| 2 | pass | 100 | 1 | 2.4 | 2 | 2 | [run](https://argusic.com/run/13257ad6-de07-4406-8c49-bdf39cd391a9) |

## What was observed on a clean machine

Attempt 2:

- `npm EBADENGINE warnings: node v18 < node>=24 requirement in package.json engines field`
- `vite dev server fails with EMFILE (inotify limit) in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
