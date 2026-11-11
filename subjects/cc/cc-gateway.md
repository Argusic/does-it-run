# cc-gateway

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/motiful/cc-gateway, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/cc-gateway

## Pinned environment

- Project commit: `447fad19b2b98602058951cad53895ed56e5ea84`
- Test commit: `447fad19b2b98602058951cad53895ed56e5ea84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3.4 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 5.2 | 0 | 0 | [run](https://argusic.com/run/3a24e428-a584-4cc8-9e1a-7ecd6e284f5f) |
| 2 | pass with mocks | 92 | 2 | 3.4 | 2 | 2 | [run](https://argusic.com/run/6bc2ee95-6420-4ed9-bc08-10555fab1ac6) |

## What was observed on a clean machine

Attempt 2:

- `Node.js v18 is installed but project requires v22+ (EBADENGINE warnings on agent-base, https-proxy-agent)`
- `setTimeout overflow warning: expires_at value 8205693747804 exceeds 32-bit signed integer max (2147483647)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
