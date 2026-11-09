# codex-app-mirror

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Wangnov/codex-app-mirror, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/codex-app-mirror

## Pinned environment

- Project commit: `b2439a30ee25690940ac0161107de37081c92110`
- Test commit: `b2439a30ee25690940ac0161107de37081c92110`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 16.5 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.5 | 27 | 6 | 6 | [run](https://argusic.com/run/f3f7d678-1388-4a4d-8855-f78162c5cd93) |
| 2 | pass with mocks | 92 | 4.5 | 16.5 | 7 | 7 | [run](https://argusic.com/run/4c30f680-dae2-42ae-9b0b-4d3c96f46574) |

## What was observed on a clean machine

Attempt 1:

- 3.5 min: `crypto global not available in Node.js 18 ESM module mode (CI uses Node 24)`
- 2.5 min: `Missing 'zip' and 'unzip' commands (no root to install packages)`
- 1.5 min: `Missing 'gpg'/'gpgv' commands for Linux Preview probe tests`
- 3.5 min: `Missing 'pwsh' (PowerShell) for Windows MSIX download and verification scripts`
- 0.5 min: `Missing .mirror-kit checkout (agents-mirror-kit repo)`
- 0.5 min: `Missing 'dotnet' SDK , cannot build StoreLink.csproj`

Attempt 2:

- 0.5 min: `zip command not found`
- 0.3 min: `gpg command not found (only gpgv installed)`
- 2 min: `pwsh command not found`
- 0.3 min: `unzip command not found`
- 0.5 min: `agents-mirror-kit .mirror-kit not checked out`
- 1 min: `secondary-sync core.js uses bare crypto but Node 18 test runner doesn't expose global crypto`
- `test-sync-secondary-s3.sh asserts --cli-connect-timeout 7 in aws log but mock CALL line lacks env-based aws CLI flags`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
