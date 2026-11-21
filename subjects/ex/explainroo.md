# explainroo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vincentsch/explainroo, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/explainroo

## Pinned environment

- Project commit: `9ad2881d02eacfa07b10d1b7ff34195243b05fd7`
- Test commit: `9ad2881d02eacfa07b10d1b7ff34195243b05fd7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7 to 28.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 28.5 | 3 | 3 | [run](https://argusic.com/run/318994c3-f74b-4dc4-8a39-3f097836fede) |
| 2 | pass | 100 | 7 | 7 | 4 | 4 | [run](https://argusic.com/run/c2bf2f5a-d3a3-48d7-a52c-491ee2182a0c) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Node.js v18.19.1 is below the required >=20.11`
- 10 min: `No Chrome or Chromium found on the system`
- `ONNX runtime prints hundreds of pthread_setaffinity_np EPERM errors`

Attempt 2:

- 2 min: `Node.js v18.19.1 below required >=20.11`
- 12 min: `Chrome/Chromium not found`
- 1 min: `sharp binary built for Node 18 rejects Node 20`
- 9 min: `speech/voice models not downloaded`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
