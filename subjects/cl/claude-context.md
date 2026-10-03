# claude-context

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zilliztech/claude-context, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/claude-context

## Pinned environment

- Project commit: `6fc318b4e3ce58e2898b00a9c3538ead9e24dee5`
- Test commit: `6fc318b4e3ce58e2898b00a9c3538ead9e24dee5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 13.4 to 15.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 14.1 | 3 | 3 | [run](https://argusic.com/run/568800f0-6e99-452e-8f7f-5794f288d7f5) |
| 2 | pass with mocks | 92 | 13 | 13.4 | 3 | 3 | [run](https://argusic.com/run/dd91afa9-5f8c-4d12-9e98-d15b30a6f6ad) |
| 3 | pass with mocks | 92 | 18 | 15.4 | 4 | 4 | [run](https://argusic.com/run/0afa4fd8-937e-459e-ab22-bdb257aa16ca) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node.js version 18 is below the required >=20`
- 3 min: `pnpm not available on PATH`
- 3 min: `pnpm-workspace.yaml had deprecated allowBuilds format with placeholder strings, causing ERR_PNPM_IGNORED_BUILDS`

Attempt 2:

- 10 min: `Node.js 18 installed but project requires >=20`
- 3 min: `pnpm not installed in container`
- 5 min: `pnpm install failed with ERR_PNPM_IGNORED_BUILDS for 17 native packages`

Attempt 3:

- 2 min: `Node.js v18 (project requires >=20)`
- 1 min: `pnpm not found in PATH`
- 5 min: `pnpm install blocked by ERR_PNPM_IGNORED_BUILDS (18 packages with unapproved build scripts)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
