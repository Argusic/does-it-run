# nightshift

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/orwa-mahmoud/nightshift, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/nightshift

## Pinned environment

- Project commit: `8eb6fc1ef0ea598cf1a89196d6cdd90bdcbac06f`
- Test commit: `8eb6fc1ef0ea598cf1a89196d6cdd90bdcbac06f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.6 to 35.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 0.15 | 35.6 | 3 | 0 | [run](https://argusic.com/run/2093fc08-c18a-4f94-b118-0d8b031c2f63) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `github-templates.bats: ruby not installed for YAML schema validation`
- 1 min: `lint-shell.sh: shellcheck not found on PATH`
- 1 min: `pwsh not installed: Windows PowerShell parity tests skipped (27 tests across ~15 files)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
