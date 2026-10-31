# compartment

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/compartmentdev/compartment, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/d15d0fd0-233a-4da0-b2c0-932b7b31fc65

## Pinned environment

- Project commit: `15373e704de52f3700f0f4f67c2eacbb85023a99`
- Test commit: `15373e704de52f3700f0f4f67c2eacbb85023a99`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.8 to 17.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 17.8 | 3 | 3 | [run](https://argusic.com/run/d15d0fd0-233a-4da0-b2c0-932b7b31fc65) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Node v18.19.1 present but repo requires v24.15.0`
- 0.5 min: `helm not in PATH for worker tests`
- 2 min: `Helm 3.16.1 compiled-in kubeVersion v1.31.0 conflicts with chart kubeVersion >=1.33.0-0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
