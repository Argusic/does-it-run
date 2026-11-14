# read-aloud

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Read-Aloud/read-aloud, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/1262f42f-f713-4cfa-b9ae-53816be2c37b

## Pinned environment

- Project commit: `1f5fe8e3e3b64f69ff4227c0fb7222ca99f1f1e4`
- Test commit: `1f5fe8e3e3b64f69ff4227c0fb7222ca99f1f1e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.4 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.02 | 3.4 | 1 | 1 | [run](https://argusic.com/run/1262f42f-f713-4cfa-b9ae-53816be2c37b) |
| 2 | pass | 100 | 0 | 7 | 1 | 1 | [run](https://argusic.com/run/c6174598-c386-46ec-bf2e-f150b387b2df) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `timing-dependent test failure in offscreen.test.js: test 'waits for listener readiness after existence becomes visible' consistently failed when all test files ran concurrently (15ms timeout and 1ms poll interval were too tight under event-`

Attempt 2:

- 12 min: `offscreen.test.js: test 7 ('waits for listener readiness after existence becomes visible') failed with 'Offscreen document did not become ready'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
