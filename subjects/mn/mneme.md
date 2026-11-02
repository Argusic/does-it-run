# mneme

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/slow-stack/mneme, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mneme

## Pinned environment

- Project commit: `1e9ac51a83fffc6312eabd9936bf02314592afaf`
- Test commit: `1e9ac51a83fffc6312eabd9936bf02314592afaf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 30.9 to 30.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 30.9 | 2 | 2 | [run](https://argusic.com/run/217005b2-3787-47e9-899c-ba77170375ee) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `test 1777: libc filter could not find musl variants because npm lockfile v3 has no explicit libc field on linuxmusl packages`
- 2 min: `test 1778: committed runtime-manifest.json out of sync with package-lock.json after node version upgrade`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
