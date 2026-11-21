# jellyfin-webos

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jellyfin/jellyfin-webos, licensed MPL-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/jellyfin-webos

## Pinned environment

- Project commit: `ab4794046467cdb88212ccc29212300cf9112a43`
- Test commit: `ab4794046467cdb88212ccc29212300cf9112a43`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, no run possible
- Valid runs: 2; wall time 2.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 6.1 | 0 | 0 | [run](https://argusic.com/run/beebccdf-d7d6-41a5-bd78-c2ea809c57bd) |
| 2 | fail | 80 | 0.15 | 2.1 | 0 | 0 | [run](https://argusic.com/run/f4b3cd5c-a39b-4c78-aef7-6af698f3dbb8) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
