# docker-headless-shell

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/chromedp/docker-headless-shell, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/docker-headless-shell

## Pinned environment

- Project commit: `4132c9245bb5d9a1eff62d31af80a92039dc3fd4`
- Test commit: `4132c9245bb5d9a1eff62d31af80a92039dc3fd4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 9 to 9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 9 | 3 | 3 | [run](https://argusic.com/run/c8ee9f06-7b8e-4a32-9f4a-e1120e188d8d) |

## What was observed on a clean machine

Attempt 1:

- `systemctl daemon-reload --user fails in container: "Failed to connect to bus: No medium found"`
- 5 min: `Missing required tools: podman, buildah, go, git-lfs, socat`
- 2 min: `build-headless-shell.sh attempts git clone of depot_tools and fetch of chromium source tree (~30GB+), which would take hours/days. Script also has an edge case where LAST variable (line 53) can contain unexpected content if out/last is malf`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
