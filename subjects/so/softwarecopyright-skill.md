# SoftwareCopyright-Skill

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Fokkyp/SoftwareCopyright-Skill, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/softwarecopyright-skill

## Pinned environment

- Project commit: `947d5963194bfda8ce57b8b454b486f13359dee4`
- Test commit: `947d5963194bfda8ce57b8b454b486f13359dee4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.9 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 10 | 10.9 | 1 | 1 | [run](https://argusic.com/run/37167176-b197-4a1e-b595-127450f1d3c9) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_playwright_cli_uses_global_prefix_without_restart: test created .cmd file (Windows) on Linux; npm_global_candidates returns bin/playwright-cli on POSIX, causing test failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
