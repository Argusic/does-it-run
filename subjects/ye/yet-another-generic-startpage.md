# yet-another-generic-startpage

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PrettyCoffee/yet-another-generic-startpage, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/yet-another-generic-startpage

## Pinned environment

- Project commit: `b611c2ae039520349e4a71edb1cc9bfa3df71cfe`
- Test commit: `b611c2ae039520349e4a71edb1cc9bfa3df71cfe`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 2.9 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3 | 3.2 | 0 | 0 | [run](https://argusic.com/run/bc5db715-8550-4cb9-8b8c-0791d1068dd4) |
| 2 | fail | 80 | 10 | 2.9 | 2 | 2 | [run](https://argusic.com/run/c4c77fe2-ab0e-43d2-9dac-5ace25feb12d) |

## What was observed on a clean machine

Attempt 2:

- 4 min: `pnpm not available and npm install -g pnpm failed due to EACCES (no root)`
- 2 min: `pnpm-workspace.yaml missing packages field causing ERR_PNPM_INVALID_WORKSPACE_CONFIGURATION`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
