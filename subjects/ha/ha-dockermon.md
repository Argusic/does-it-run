# ha-dockermon

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/philhawthorne/ha-dockermon, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ha-dockermon

## Pinned environment

- Project commit: `044d7470f40a3ca36fb3f2afe64dda095146d476`
- Test commit: `044d7470f40a3ca36fb3f2afe64dda095146d476`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.3 | 8.1 | 3 | 3 | [run](https://argusic.com/run/7dff45c6-7bde-4e83-814a-bd53daf24223) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No Docker daemon available in container`
- 2 min: `Mock server needed threading to handle concurrent connections`
- 2 min: `Docker exec endpoint requires two-step API (create exec then start it)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
