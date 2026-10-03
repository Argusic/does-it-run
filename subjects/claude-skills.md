# claude-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Jeffallan/claude-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-skills

## Pinned environment

- Project commit: `882ef55e377dbf9a4dbe496bb41ac6ccd0e555cf`
- Test commit: `882ef55e377dbf9a4dbe496bb41ac6ccd0e555cf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 6.1 | 5 | 5 | [run](https://argusic.com/run/71b39742-8965-497e-bccd-f6ca1d1e7aca) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `python command not found; Makefile and test script used bare python`
- 1 min: `pyyaml not installed; validate-skills.py fell back to broken simple parser producing 17 false errors`
- 1 min: `pyright and ruff not on PATH`
- 2 min: `site/scripts/sync-content.mjs uses import.meta.dirname (Node 21+) but container has Node 18`
- 1 min: `astro requires Node >=20 but container ships Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
