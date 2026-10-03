# re-start

**Verdict: runs.** Argusic Score 96.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/refact0r/re-start, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/re-start

## Pinned environment

- Project commit: `700fbc103a63754fba4ad363d99316830a179e41`
- Test commit: `700fbc103a63754fba4ad363d99316830a179e41`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.1 to 9.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 5.1 | 3 | 3 | [run](https://argusic.com/run/7d58ba22-4a9d-4ab8-886e-df12a68812af) |
| 2 | pass | 93.33 | 2 | 9.4 | 3 | 2 | [run](https://argusic.com/run/80874a15-bb7a-4d9a-b3ba-502c3ee98f94) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `System Node.js 18.19.1 is too old for Vite 8 (requires >=20.19). Vite crashed with ReferenceError: CustomEvent is not defined.`
- 1 min: `Rolldown native binding @rolldown/binding-linux-x64-gnu was missing because the initial npm install with Node 18 didn't install the correct optional dependency.`
- 1 min: `2 test failures: 'noon shortcut alone rolls when past' and 'midday shortcut rolls when past' , strict inequality (date < safeNow) failed to roll when time exactly equals current time in UTC.`

Attempt 2:

- 1 min: `Node.js v18.19.1 lacks 'styleText' from node:util required by Vite 8/rolldown, causing startup error in vitest and vite`
- 2 min: `2 date-matcher tests failed: 'noon shortcut alone rolls when past' and 'midday shortcut rolls when past' , strict '<' comparison meant exactly-noon didn't roll to tomorrow`
- `Chrome build zip step fails: 'zip' not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
