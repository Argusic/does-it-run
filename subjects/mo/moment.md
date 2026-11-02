# moment

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moment/moment, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/moment

## Pinned environment

- Project commit: `c2a703a4d84aa57ee2722ff8fb4a8016279fb3c4`
- Test commit: `c2a703a4d84aa57ee2722ff8fb4a8016279fb3c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.2 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.4 | 3.2 | 2 | 2 | [run](https://argusic.com/run/8863ce67-942a-481f-9d92-7ccf00655612) |
| 2 | pass | 100 | 3 | 5.8 | 2 | 2 | [run](https://argusic.com/run/a75752de-fa7b-42c9-9f21-64110e930a06) |

## What was observed on a clean machine

Attempt 1:

- 3.6 min: `Container had only Node v18.19.1 but package.json devEngines requires Node ^22.22.2 or >=26 for tooling, and pnpm was not installed.`
- 2 min: `Focused run 'pnpm test -- --only=moment/parse' failed with RollupError 'Could not resolve entry module src/test/moment/parse.js' because no such test file exists.`

Attempt 2:

- 1 min: `Container has Node v18.19.1, but package.json devEngines requires Node >=22 (the pnpm 11 and lint tooling need it)`
- 0.5 min: `npm EACCES on global install , /usr/local not writable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
