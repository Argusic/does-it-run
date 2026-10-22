# chart-releaser-action

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/helm/chart-releaser-action, licensed Apache-2.0, written in Shell.

Evidence and recordings: https://argusic.com/subject/chart-releaser-action

## Pinned environment

- Project commit: `3e001cb8c68933439c7e721650f20a07a1a5c61e`
- Test commit: `3e001cb8c68933439c7e721650f20a07a1a5c61e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.6 to 16.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 16.6 | 2 | 2 | [run](https://argusic.com/run/b9af7853-ef3e-4061-b269-3dc91db05c27) |

## What was observed on a clean machine

Attempt 1:

- `chart-releaser v1.7.0 GetPushURL panics on non-HTTPS git remote URLs`
- `RUNNER_TOOL_CACHE env var not set when running cr.sh outside GitHub Actions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
