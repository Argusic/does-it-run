# yett

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elbywan/yett, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/yett

## Pinned environment

- Project commit: `e2bc2a7ce2a5a14ca4bf481a2e1d38d549610258`
- Test commit: `e2bc2a7ce2a5a14ca4bf481a2e1d38d549610258`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 30.7 to 30.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 22 | 30.7 | 2 | 1 | [run](https://argusic.com/run/33e61850-4f59-452b-b03f-9370a7c5ba58) |

## What was observed on a clean machine

Attempt 1:

- 20 min: `No browser binaries (Chrome/Firefox) available in container , Karma tests cannot run`
- 5 min: `Rollup build is slow (~55s per bundle) due to container CPU constraints`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
