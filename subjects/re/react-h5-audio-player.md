# react-h5-audio-player

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lhz516/react-h5-audio-player, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/react-h5-audio-player

## Pinned environment

- Project commit: `d93969e30aaba9d41c1c93aeea40e371d3f7993d`
- Test commit: `d93969e30aaba9d41c1c93aeea40e371d3f7993d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 9 | 2.4 | 1 | 1 | [run](https://argusic.com/run/f1fa7c6f-46fe-41ed-af73-6cf99a161d2d) |

## What was observed on a clean machine

Attempt 1:

- 9 min: `System Node is v18.19.1, below the project's engines >=20; Node 20 then failed because @testing-library/jest-dom requires node >=22`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
