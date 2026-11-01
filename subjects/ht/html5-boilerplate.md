# html5-boilerplate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/h5bp/html5-boilerplate, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/html5-boilerplate

## Pinned environment

- Project commit: `b6597338e695dc4a8165c5abcb2bfffa586c3ee5`
- Test commit: `b6597338e695dc4a8165c5abcb2bfffa586c3ee5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.1 to 2.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.09 | 2.6 | 0 | 0 | [run](https://argusic.com/run/d8f67ca2-bbcd-4e50-97bb-dc410be98f80) |
| 2 | pass | 100 | 0.1 | 1.1 | 1 | 1 | [run](https://argusic.com/run/65dd64e6-c1c0-4fa2-b5fd-fc0a14d70eac) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `mocha 12 requires Node >=22 (container has Node 18.19) , 'with { type: "json" }' syntax error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
