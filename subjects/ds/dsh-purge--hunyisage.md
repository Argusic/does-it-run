# dsh-purge

**Verdict: runs.** Argusic Score 58.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HunYiSage/dsh-purge, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/run/33183bca-d951-4a48-ae55-e436b25442de

## Pinned environment

- Project commit: `4c3369a945701598275dcabbe958b7b815570ed5`
- Test commit: `4c3369a945701598275dcabbe958b7b815570ed5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 0.4 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.14 | 16 | 17.5 | 7 | 6 | [run](https://argusic.com/run/33183bca-d951-4a48-ae55-e436b25442de) |
| 2 | fail | 20 | n/a | 0.4 | 0 | 0 | [run](https://argusic.com/run/77437390-f2a6-4a13-8b3f-a893bfa93a72) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm test exits 1: Missing script: "test"`
- 4 min: `Official DSH 0.2.1-rc.2 fails under bundled Node 18 with SyntaxError: node:util does not export parseEnv`
- 2 min: `dsh plugin add returned 127: pnpm was not found`
- 5 min: `Fresh dsh plugin add exits 0 but pnpm skips postinstall, leaving the dsh-purge profile insert absent`
- 3 min: `Documented ensure-profile-bundle repair silently does nothing for linked checkout because symlinked argv[1] fails the entrypoint check`
- 8 min: `Apply rewrites host lib/bin.js from mode 0775 to 0664, causing subsequent dsh commands to fail with Permission denied`
- 2 min: `dsh-purge --status printed undefined for every patch when no host was configured`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
