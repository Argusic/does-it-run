# claude-code-hooks

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/karanb192/claude-code-hooks, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/claude-code-hooks

## Pinned environment

- Project commit: `888ef0827f121d583fb3a07c6253a297787946dc`
- Test commit: `888ef0827f121d583fb3a07c6253a297787946dc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.3 to 4.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.3 | 2 | 2 | [run](https://argusic.com/run/41ac9ef1-277f-4d7f-9494-d0c8641e0367) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `ruff not installed, causing 4 format-code test failures`
- 1 min: `uv not on PATH, npx prettier unavailable via npm -g, format-code tests would need prettier`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
