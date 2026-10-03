# skill-recorder

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/skill-recorder, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/skill-recorder

## Pinned environment

- Project commit: `b05d59036182e897e1a60e90651e775cf5f97e8d`
- Test commit: `b05d59036182e897e1a60e90651e775cf5f97e8d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 2.9 | 2 | 2 | [run](https://argusic.com/run/370b164d-2058-48a4-86a4-59febb4e1a40) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js was v18 but project requires >=24.19.0`
- `Electron SUID sandbox helper not running as root (expected in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
