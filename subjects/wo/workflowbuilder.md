# workflowbuilder

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/synergycodes/workflowbuilder, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/workflowbuilder

## Pinned environment

- Project commit: `052c396cc90aeebe5b8a1055b7625ec43a88a38e`
- Test commit: `052c396cc90aeebe5b8a1055b7625ec43a88a38e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.6 to 21.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 21.6 | 3 | 3 | [run](https://argusic.com/run/5a9b8d24-fe6c-41f0-8327-20079c900b9d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Node v18.19.1 installed, project requires 22.12.0; pnpm not on PATH`
- 2 min: `Icon generator createIconEntry picked up index.ts as an icon key because generateKeys() only filtered by .tsx in filename, and readdirSync read index.ts (which has no .tsx suffix match)`
- 1 min: `Backend tests failed to resolve @workflowbuilder/temporal/client because the temporal package had no dist/`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
