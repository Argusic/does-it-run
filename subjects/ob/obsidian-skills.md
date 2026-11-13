# obsidian-skills

**Verdict: runs with mocks.** Argusic Score 79.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/obsidianmd/obsidian-skills, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/obsidian-skills

## Pinned environment

- Project commit: `398127736bd4ba42d767b1419fee1a927508370b`
- Test commit: `398127736bd4ba42d767b1419fee1a927508370b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 1.5 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 78.67 | 5 | 5.1 | 3 | 1 | [run](https://argusic.com/run/1d914d5f-3a7d-4445-9aa8-0a0e6b12e1b8) |
| 2 | fail | 80 | 1 | 1.5 | 0 | 0 | [run](https://argusic.com/run/822d7674-fd11-4899-8cb3-e659bc13c5dd) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Defuddle CLI fails with 'Cannot find module 'linkedom'' on fresh install because the latest 'linkedom@0.18.15' depends on ESM-only 'css-select' but defuddle's CJS wrapper does 'require('linkedom')'`
- 2 min: `obsidian-headless (ob) fails to start: requires Node.js >=22, but container has Node.js v18.19.1`
- `obsidian-cli requires the Obsidian desktop app running with CLI enabled, which is not available in this headless container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
