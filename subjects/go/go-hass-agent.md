# go-hass-agent

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/joshuar/go-hass-agent, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/go-hass-agent

## Pinned environment

- Project commit: `5905f31725345023c5f71ff69c727303e0b070f2`
- Test commit: `5905f31725345023c5f71ff69c727303e0b070f2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.2 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.2 | 1 | 1 | [run](https://argusic.com/run/a05fc5a9-b2bd-445b-a68f-1fca76a7490e) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `@tailwindcss/oxide native binding missing for linux-x64-gnu`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
