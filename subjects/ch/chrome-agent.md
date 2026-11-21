# chrome-agent

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/captivus/chrome-agent, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/chrome-agent

## Pinned environment

- Project commit: `1dd4a60c43da15d950131216147e6e3a4121a3d2`
- Test commit: `1dd4a60c43da15d950131216147e6e3a4121a3d2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.2 to 12.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 12.2 | 4 | 4 | [run](https://argusic.com/run/fb9986a8-f188-4d46-baea-23743b2ae03f) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Chrome binary not found in container`
- 6 min: `Chrome requires --no-sandbox in this container (no user namespaces)`
- 3 min: `lsof not installed in container`
- 1 min: `Viewport height assertion too tight for Chrome 157 headless`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
