# codex-app-mirror

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Wangnov/codex-app-mirror, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/codex-app-mirror

## Pinned environment

- Project commit: `b2439a30ee25690940ac0161107de37081c92110`
- Test commit: `b2439a30ee25690940ac0161107de37081c92110`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27 to 27 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12.5 | 27 | 6 | 6 | [run](https://argusic.com/run/f3f7d678-1388-4a4d-8855-f78162c5cd93) |

## What was observed on a clean machine

Attempt 1:

- 3.5 min: `crypto global not available in Node.js 18 ESM module mode (CI uses Node 24)`
- 2.5 min: `Missing 'zip' and 'unzip' commands (no root to install packages)`
- 1.5 min: `Missing 'gpg'/'gpgv' commands for Linux Preview probe tests`
- 3.5 min: `Missing 'pwsh' (PowerShell) for Windows MSIX download and verification scripts`
- 0.5 min: `Missing .mirror-kit checkout (agents-mirror-kit repo)`
- 0.5 min: `Missing 'dotnet' SDK , cannot build StoreLink.csproj`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
