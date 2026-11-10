# yet-another-media-player

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jianyu-li/yet-another-media-player, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/yet-another-media-player

## Pinned environment

- Project commit: `0e5336b7cfd5389359d708ae9ad8285546123441`
- Test commit: `0e5336b7cfd5389359d708ae9ad8285546123441`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.7 to 16.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 16.7 | 3 | 3 | [run](https://argusic.com/run/473490e5-0d6f-4e27-8d78-23cbc62d18f0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 test runner glob expansion failed: 'tests/**/*.test.js' not expanded by node --test`
- 3 min: `Lyrics controller test: clock.enable({ apis: ["setTimeout"] }) uses object format not supported in Node v18 MockTimers`
- 8 min: `Volume hold controller test: mock.timers.tick(RELEASE_LINGER_MS) fails to fire timers created inside _end() on Node v18.19.1 (MockTimers bug)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
