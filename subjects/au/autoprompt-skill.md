# autoprompt-skill

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Spielewoy/autoprompt-skill, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/autoprompt-skill

## Pinned environment

- Project commit: `b6516cf52a7891d797621fdd2a8ca0311e1ae0a9`
- Test commit: `b6516cf52a7891d797621fdd2a8ca0311e1ae0a9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31 to 31 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 31 | 4 | 4 | [run](https://argusic.com/run/09fbec39-3c69-4edc-8bf4-3193f79a3adb) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Node.js v18 unmet engine requirement (needs >=20)`
- 1 min: `PyYAML not found in system site-packages; per-user install skipped by test HOME override`
- 1 min: `python command not on PATH (only python3 exists)`
- 1 min: `test 109: packed global package configure command failed because subprocess with overridden HOME could not find PyYAML`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
