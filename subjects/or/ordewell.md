# ordewell

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ordewell/ordewell, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ordewell

## Pinned environment

- Project commit: `551f05ac81545bfe850524b860ff421a59c933a8`
- Test commit: `551f05ac81545bfe850524b860ff421a59c933a8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 73.7 to 73.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 73.7 | 3 | 3 | [run](https://argusic.com/run/1e44c453-6695-42af-96ac-20a8ef0bcfbd) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `Node.js v18.19.1 bundled, project requires >=20.3 (package.json engines). Caused all workspace engine warnings, broke bench/lib/data-dir.mjs (import.meta.dirname undefined before Node 22), caused tsc --noEmit OOM (heap exhausted at default`
- `No Docker engine in container. Two SettingsService tests fail: 'changes from what the file holds, and comes off it whole when the change answers nothing' and 'is read, as written whatever it holds, where ORDEWELL_CONTAINERS=1 is set…'. Both`
- `TypeScript typecheck (npx tsc --noEmit) OOM on Node 18 with default 4GB heap limit at ~86s. Compiled ~2700+ test files.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
