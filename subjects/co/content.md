# content

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nuxt/content, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/content

## Pinned environment

- Project commit: `75eff79a94b25a1e3f4f161efcbfc5d6b4ff3f5e`
- Test commit: `75eff79a94b25a1e3f4f161efcbfc5d6b4ff3f5e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 9.7 | 2 | 2 | [run](https://argusic.com/run/d2eb6a8e-f0ca-4245-9289-3db4650f4a96) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pnpm not in PATH; npm lacked permission to install globally`
- 1 min: `System Node.js v18 does not meet project requirement >=20.19.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
