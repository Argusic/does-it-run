# archify

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tt-a1i/archify, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/archify

## Pinned environment

- Project commit: `5de7275fe87a66a19d52a4d9b0b3a4f2a5a90115`
- Test commit: `5de7275fe87a66a19d52a4d9b0b3a4f2a5a90115`
- Worker image digest: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.5 to 17.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 34 | 17.5 | 1 | 1 | [run](https://argusic.com/run/8388ff71-9731-4015-99ca-5afe6fef7e3b) |

## What was observed on a clean machine

Attempt 2:

- `Test 151: spawnSync unzip ENOENT , unzip command not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
