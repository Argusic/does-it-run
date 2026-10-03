# gitea

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-gitea/gitea, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gitea

## Pinned environment

- Project commit: `231ee19cff64e0872247c8ac4e45176bb918bc3f`
- Test commit: `231ee19cff64e0872247c8ac4e45176bb918bc3f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 10.4 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11.8 | 10.4 | 5 | 5 | [run](https://argusic.com/run/af3b8bb2-0940-4370-a26d-4af90d348576) |
| 2 | pass | 100 | 13.2 | 14.5 | 5 | 5 | [run](https://argusic.com/run/4354201e-0813-4157-a695-c548a06ee265) |
| 3 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/e32e5624-d201-4ac4-aeeb-bc7665707e76) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.1 not found (required by go.mod)`
- 1 min: `Node.js v18.19.1 too old (need >=22.18.0)`
- 0.5 min: `pnpm not found`
- 0.5 min: `Git LFS not found`
- `Python/uv not found (optional dep)`

Attempt 2:

- 1 min: `Go 1.27 not found on system`
- 1 min: `pnpm not installed; npm install -g pnpm failed with EACCES`
- 1.5 min: `Node.js v18 too old (needs >=22.18.0)`
- 0.5 min: `rolldown native binding missing after Node upgrade`
- 1 min: `Test TestGitDiffTreeRespectsDiffOrderFile/GlobalDiffOrderFile failed: git config set --global syntax requires Git >=2.45 (system has 2.43)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
