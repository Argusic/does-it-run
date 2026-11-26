# mouse-mcp

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SonicloudTech/mouse-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/mouse-mcp

## Pinned environment

- Project commit: `279feeb486c40b6fa0fbfc1b816637f0a427c901`
- Test commit: `279feeb486c40b6fa0fbfc1b816637f0a427c901`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 3.3 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 3.7 | 1 | 1 | [run](https://argusic.com/run/f76cc3d0-bf42-4d06-988a-71d110644ac6) |
| 2 | pass with mocks | 92 | 1 | 3.3 | 1 | 1 | [run](https://argusic.com/run/cb28a274-3011-4496-9d97-4dea269f085f) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `T01 voice-typer test (voice-typer.test.mjs) failed on Linux: snapshotFocus() returns undefined on non-Windows platforms, but the test asserted entries[0].focus was truthy`

Attempt 2:

- 1 min: `T01 voice-typer.test.mjs asserted focus snapshot present on Linux where snapshotFocus() returns undefined (Windows-only via user32.dll)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
