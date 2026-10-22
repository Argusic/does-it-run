# firestore-backup-restore

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dalenguyen/firestore-backup-restore, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/firestore-backup-restore

## Pinned environment

- Project commit: `0c2ed3ab1dff0cda9bdd741a6345a594ac60001c`
- Test commit: `0c2ed3ab1dff0cda9bdd741a6345a594ac60001c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.9 to 11.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 11.9 | 3 | 3 | [run](https://argusic.com/run/90db5c44-c4ec-46c0-a8c0-d065e2533aff) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing serviceAccountKey.json (gitignored, not shipped in repo)`
- 3 min: `No Java runtime , Firebase Emulator cannot start`
- 1 min: `vitest config missing setupFiles entry`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
