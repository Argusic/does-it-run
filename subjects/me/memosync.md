# MemoSync

**Verdict: runs.** Argusic Score 86.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SLEEPYBQ/MemoSync, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/memosync

## Pinned environment

- Project commit: `dfa8d4d7f613f0f6480f436950c57bdf6fd613ec`
- Test commit: `dfa8d4d7f613f0f6480f436950c57bdf6fd613ec`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 14 | 14 | 3 | 1 | [run](https://argusic.com/run/016e1906-70a7-41ee-99f8-c2c7dcb67e59) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `bun not installed in container , downloaded via npm with --prefix to user home`
- `4 DiffStore tests fail with 'fatal: invalid reference: main' , detached HEAD at FETCH_HEAD, no local main branch`
- `6 client tests fail , 5 require Playwright browser binaries (chromium not installed), 1 is a race condition in mounted component test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
