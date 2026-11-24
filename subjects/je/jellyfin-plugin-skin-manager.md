# jellyfin-plugin-skin-manager

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/danieladov/jellyfin-plugin-skin-manager, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/jellyfin-plugin-skin-manager

## Pinned environment

- Project commit: `0e68847fff7770f769eb22f81c164362b29d7e8b`
- Test commit: `0e68847fff7770f769eb22f81c164362b29d7e8b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.4 to 13.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 13.7 | 3 | 3 | [run](https://argusic.com/run/8bb16b1c-004e-4679-9cb4-54df25e39d54) |
| 2 | pass with mocks | 92 | 8 | 3.4 | 3 | 3 | [run](https://argusic.com/run/823e217e-73f1-439e-a0ab-884be851bb06) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `.NET SDK 8.0 not installed in container`
- 3 min: `Missing embedded resource jquery.fontpicker.min.css - Plugin.cs references it but file doesn't exist`
- 1 min: `Stale MediaBrowser.Api assembly reference in .csproj pointing to non-existent Windows C:\ path`

Attempt 2:

- 6 min: `Missing .NET SDK (dotnet command not found)`
- `Stale MediaBrowser.Api file reference in csproj , warning MSB3245, unused in code`
- `build.yaml references wrong plugin (TMDb Box Sets instead of SkinManager)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
