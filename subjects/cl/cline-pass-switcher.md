# cline-pass-switcher

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/munmunjaklin458-afk/cline-pass-switcher, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/cline-pass-switcher

## Pinned environment

- Project commit: `02538a3137a08948a94f26f17dd4aeff8c029ed1`
- Test commit: `02538a3137a08948a94f26f17dd4aeff8c029ed1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12 to 12 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.1 | 12 | 1 | 1 | [run](https://argusic.com/run/8b0f6cb8-7d73-4dd3-8b7e-a6c9140967c8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Server crashes after first request when DATA_DIR is repo root without config.json/metadata.json (both in .gitignore)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
