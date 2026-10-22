# airAnime

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/txperl/airAnime, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/airanime

## Pinned environment

- Project commit: `bb0f9cceb0b5919c3632cedfd01bf50053b9ab95`
- Test commit: `bb0f9cceb0b5919c3632cedfd01bf50053b9ab95`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.3 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 6 | 6.3 | 2 | 1 | [run](https://argusic.com/run/b4c47190-35d7-452c-8465-b934a1e1eb94) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `vercel dev server was started under a 90s timeout and died mid-test, causing 502 Bad Gateway from /fetch during the first browser run`
- 1 min: `'vercel build' requires a valid Vercel login token; rejected with 'The specified token is not valid'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
